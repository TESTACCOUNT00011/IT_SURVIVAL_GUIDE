---
tags: [troubleshooting, errors, common-issues]
difficulty: 1
---

# Troubleshooting Wiki

Common errors and their solutions. **Search this page before posting questions in communities.**

Use Ctrl+F (Cmd+F on Mac) to search for your error message.

---

## Installation & Setup Errors

### "Command not found" / "[command] is not recognized"

**Cause:** Software isn't installed or not in system PATH

**Solutions:**
1. Verify installation: `which [command]` (Mac/Linux) or `where [command]` (Windows)
2. Reinstall the software
3. Add to PATH:
   - **Windows:** System Properties → Environment Variables → Path → Add installation directory
   - **Mac:** Edit `~/.zshrc` or `~/.bash_profile`: `export PATH="/path/to/software:$PATH"`
   - **Linux:** Edit `~/.bashrc`: `export PATH="/path/to/software:$PATH"`
4. Restart terminal/command prompt

---

### "Permission denied" errors

**Cause:** Insufficient user permissions

**Solutions:**
- **Mac/Linux:** Add `sudo` before command (use sparingly)
- **Better approach:** Fix ownership: `sudo chown -R $USER:$USER /path/to/directory`
- **Windows:** Right-click → Run as Administrator
- **NPM specific:** Don't use sudo. Fix npm permissions: https://docs.npmjs.com/resolving-eacces-permissions-errors

---

### "Port already in use" / "EADDRINUSE"

**Cause:** Another application is using that port

**Solutions:**
1. Find what's using the port:
   - **Mac/Linux:** `lsof -i :PORT_NUMBER` or `netstat -tulpn | grep PORT_NUMBER`
   - **Windows:** `netstat -ano | findstr :PORT_NUMBER`
2. Kill the process:
   - **Mac/Linux:** `kill -9 PROCESS_ID`
   - **Windows:** `taskkill /PID PROCESS_ID /F`
3. Or use a different port in your application config

---

### "No space left on device"

**Cause:** Disk is full

**Solutions:**
1. Check disk space: `df -h` (Mac/Linux) or check Properties (Windows)
2. Clean up:
   - Empty trash/recycle bin
   - Remove old downloads
   - Clear package caches: `npm cache clean --force`, `pip cache purge`
   - Remove unused Docker images: `docker system prune`
3. Consider upgrading storage if recurring

---

## Git Errors

### "fatal: remote origin already exists"

**Solution:** 
```bash
git remote set-url origin NEW_URL
```

---

### "error: failed to push some refs"

**Cause:** Remote has commits you don't have locally

**Solutions:**
```bash
# Option 1: Pull first (recommended)
git pull origin main
# Resolve any merge conflicts
git push origin main

# Option 2: Force push (DANGEROUS - overwrites remote)
git push -f origin main
```

---

### "fatal: Authentication failed"

**Cause:** Wrong credentials or token expired

**Solutions:**
1. Generate new GitHub/GitLab personal access token
2. Update stored credentials:
   - **Mac:** Keychain Access → find github.com → edit password
   - **Windows:** Credential Manager → Windows Credentials → edit git:https://github.com
   - **Linux:** `git credential reject` then re-enter
3. Use SSH keys instead: https://docs.github.com/en/authentication/connecting-to-github-with-ssh

---

### "merge conflict" 

**Solution:**
1. Open conflicted files in editor
2. Look for conflict markers:
   ```
   <<<<<<< HEAD
   your changes
   =======
   their changes
   >>>>>>> branch-name
   ```
3. Edit to keep desired code, remove markers
4. Stage resolved files: `git add filename`
5. Complete merge: `git commit`

---

## Web Development Errors

### CORS Error: "Access-Control-Allow-Origin"

**Cause:** Browser blocking cross-origin requests for security

**Solutions:**
1. **For development:** Use proxy in your dev server config
2. **For production:** Backend must send proper headers:
   ```javascript
   // Node.js/Express example
   app.use((req, res, next) => {
     res.header('Access-Control-Allow-Origin', 'https://your-frontend.com');
     next();
   });
   ```
3. **Quick fix for learning:** Use browser extension (not for production!)

---

### "Cannot read property of undefined"

**Cause:** Trying to access property on null/undefined value

**Solutions:**
1. Check if value exists before accessing:
   ```javascript
   // Bad
   const name = user.profile.name;
   
   // Good
   const name = user?.profile?.name;  // Optional chaining
   // OR
   const name = user && user.profile ? user.profile.name : 'default';
   ```
2. Initialize objects with default values
3. Use debugging: `console.log()` to check what's actually in the variable

---

### React: "Too many re-renders"

**Cause:** State update inside render without condition

**Solution:**
```javascript
// Bad - causes infinite loop
function Component() {
  const [count, setCount] = useState(0);
  setCount(count + 1); // Never do this in render!
  return <div>{count}</div>;
}

// Good - use useEffect for side effects
function Component() {
  const [count, setCount] = useState(0);
  useEffect(() => {
    setCount(count + 1); // Only runs when dependencies change
  }, [dependency]);
  return <div>{count}</div>;
}
```

---

### CSS: Styles not applying

**Checklist:**
- [ ] Is CSS file linked correctly? `<link rel="stylesheet" href="./style.css">`
- [ ] Is there a typo in class names? (case-sensitive!)
- [ ] Is specificity too low? (check DevTools)
- [ ] Is `!important` overriding elsewhere?
- [ ] Did you save the file?
- [ ] Hard refresh browser: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)

---

## Python Errors

### "ModuleNotFoundError: No module named 'X'"

**Solutions:**
1. Install the package: `pip install package-name`
2. Check you're using correct Python environment:
   ```bash
   which python  # Should point to where packages are installed
   pip list      # See installed packages
   ```
3. If using virtualenv, activate it: `source venv/bin/activate` (Mac/Linux) or `venv\Scripts\activate` (Windows)

---

### "IndentationError"

**Cause:** Inconsistent indentation (mixing tabs/spaces)

**Solution:**
- Configure editor to use spaces only (PEP 8 recommends 4 spaces)
- Select all and convert tabs to spaces
- Be consistent throughout file

---

### "TypeError: 'X' object is not iterable"

**Cause:** Trying to loop over something that can't be looped

**Solution:**
```python
# Bad
for num in 5:  # int is not iterable
    print(num)

# Good
for num in range(5):
    print(num)
```

---

## Database Errors

### "Connection refused" / "Can't connect to server"

**Checklist:**
- [ ] Is database service running? `sudo systemctl status mysql` or `pg_isready`
- [ ] Is it listening on correct port? (MySQL: 3306, PostgreSQL: 5432)
- [ ] Firewall blocking connection?
- [ ] Wrong hostname? Use `localhost` or `127.0.0.1` for local
- [ ] Credentials correct? (username, password, database name)

---

### "Duplicate entry for key 'PRIMARY'"

**Cause:** Trying to insert record with existing primary key

**Solutions:**
1. Use different ID
2. Use `INSERT IGNORE` or `ON DUPLICATE KEY UPDATE`
3. Check if record already exists before inserting
4. If auto-increment, ensure column is set to AUTO_INCREMENT

---

### SQL Injection vulnerability warnings

**Solution:** ALWAYS use parameterized queries

```python
# BAD - vulnerable to SQL injection
cursor.execute(f"SELECT * FROM users WHERE username = '{username}'")

# GOOD - parameterized
cursor.execute("SELECT * FROM users WHERE username = %s", (username,))
```

---

## Cloud & Deployment Errors

### AWS: "Access Denied" / "UnauthorizedOperation"

**Solutions:**
1. Check IAM permissions for your user/role
2. Verify you're using correct region
3. Check policy attachments in IAM console
4. Use AWS Policy Generator to create minimal required permissions

---

### "Build failed" on Vercel/Netlify/Render

**Checklist:**
- [ ] Check build logs for specific error
- [ ] Ensure all dependencies in package.json
- [ ] Verify build command is correct
- [ ] Check Node.js version matches locally and on platform
- [ ] Test build locally: `npm run build`
- [ ] Check environment variables are set in platform dashboard

---

### Docker: "Container exited immediately"

**Cause:** Container's main process finished

**Solutions:**
1. Keep container running:
   ```dockerfile
   CMD ["tail", "-f", "/dev/null"]  # For debugging
   # OR ensure your app runs in foreground
   ```
2. Check logs: `docker logs CONTAINER_ID`
3. Run interactively to debug: `docker run -it IMAGE_NAME /bin/bash`

---

## General Debugging Strategy

When encountering ANY error:

1. **Read the full error message** carefully (most people skip this!)
2. **Copy exact error** into Google/search engine
3. **Check Stack Overflow** - likely someone had same issue
4. **Reproduce consistently** - note exact steps
5. **Isolate the problem** - create minimal reproduction
6. **Check documentation** for the tool/library
7. **Add logging/debug statements** to understand flow
8. **Ask for help** with context (what you tried, error message, code snippet)

---

## When to Ask for Help

Before posting in communities, ensure you have:

- [ ] Searched for existing answers
- [ ] Googled the error message
- [ ] Read relevant documentation
- [ ] Tried at least 2 solutions
- [ ] Prepared:
  - Exact error message (full text)
  - What you were trying to do
  - What you've tried so far
  - Code snippet (minimal, reproducible)
  - Your environment (OS, versions)

**Template for asking:**
```
I'm trying to: [goal]
Expected: [what should happen]
Actual: [what's happening]

Error message:
[paste full error]

What I've tried:
1. [solution 1] - result
2. [solution 2] - result

My setup:
- OS: [version]
- Language/Framework: [version]
- Relevant code: [snippet]
```

---

## Contributing to This Wiki

Found an error and solution not listed? 

1. Document it in your [[../../00-TEMPLATES/Troubleshooting-Log|Troubleshooting Log]]
2. Submit addition to this wiki via GitHub PR or community contribution
3. Help others by sharing knowledge!

---

**See Also:**
- [[../02-BASICS/04-Google-Fu|Google-Fu Guide]] - Learn to search effectively
- [[../../00-TEMPLATES/Troubleshooting-Log|Troubleshooting Log Template]] - Track your own issues
- [[Soft-Skills|Soft Skills Module]] - How to ask good questions
