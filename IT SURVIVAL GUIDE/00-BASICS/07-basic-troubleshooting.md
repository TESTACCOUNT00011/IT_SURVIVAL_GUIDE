# 07 - Basic Troubleshooting: Fix It Yourself

## 🎯 The IT Mindset

**Most computer problems have simple solutions.**

You don't need to be a genius. You need a SYSTEM for figuring things out.

---

## 🔧 The Universal Troubleshooting Flowchart

```
Something's broken
       ↓
1. Restart the thing
       ↓
Still broken?
       ↓
2. Google the exact error message
       ↓
Found solution? → Try it!
       ↓
Still broken?
       ↓
3. Check for updates
       ↓
Still broken?
       ↓
4. Undo recent changes
       ↓
Still broken?
       ↓
5. Ask for help (with details!)
```

---

## Step 1: Have You Tried Turning It Off and On Again?

**This fixes more than 50% of problems.** Seriously.

### Why Restarting Works

- Clears temporary glitches
- Resets stuck processes
- Applies pending updates
- Fresh start = fewer conflicts

### What to Restart (In Order)

1. **The program** - Close and reopen it
2. **Your browser** - Close all tabs, reopen
3. **Your computer** - Full restart (not sleep!)
4. **Your router** - Unplug for 30 seconds, plug back in
5. **The device** - Phone, tablet, printer, etc.

**Try ALL of these before moving to step 2.**

---

## Step 2: Google the Error

Remember your Google-fu from earlier? Use it!

### How to Search for Problems

**Copy the EXACT error message** (screenshot if needed)

Good search formats:
```
"[exact error message]" fix
[program name] [what you were doing] not working
[program name] [error code] solution site:reddit.com
```

### Where to Look for Answers

| Source | Best For | Reliability |
|--------|----------|-------------|
| **Official support pages** | Common issues, official fixes | ⭐⭐⭐⭐⭐ |
| **Stack Overflow** | Technical errors, coding | ⭐⭐⭐⭐⭐ |
| **Reddit** | Real user experiences | ⭐⭐⭐⭐ |
| **YouTube** | Visual step-by-step guides | ⭐⭐⭐⭐ |
| **Forum threads** | Older/niche problems | ⭐⭐⭐ |

### Red Flags in Solutions

❌ Avoid solutions that:
- Ask you to download random software
- Tell you to edit registry (Windows) without clear explanation
- Are from 10+ years ago (for fast-changing software)
- Have zero upvotes/comments confirming they work
- Sound too good to be true

---

## Step 3: Check for Updates

**Outdated software = bugs + security holes**

### What to Update

1. **The problematic program** - Check Help → Check for Updates
2. **Your operating system** - Windows Update / macOS Software Update
3. **Your browser** - Usually automatic, but check
4. **Drivers** (for hardware issues) - Device Manager (Windows)

### How to Update

**Windows:**
```
Settings → Update & Security → Windows Update → Check for updates
```

**Mac:**
```
System Preferences → Software Update
```

**Programs:**
```
Help menu → Check for Updates
OR
File → Preferences → Updates
```

---

## Step 4: Undo Recent Changes

**Did it work before? What changed?**

### Common Culprits

| Change | How to Undo |
|--------|-------------|
| New program installed | Uninstall it |
| Windows update | Uninstall update or use System Restore |
| New setting changed | Change it back |
| New hardware added | Disconnect it |
| File moved/deleted | Restore from backup or Recycle Bin |

### Windows System Restore (Magic Button!)

If something broke recently:

1. Search for **"Create a restore point"**
2. Click **System Restore**
3. Choose a date BEFORE the problem started
4. Let it work (takes 10-30 minutes)
5. Computer restarts, hopefully fixed!

**Note:** This doesn't affect your files, just system settings and programs.

---

## 🐛 Common Problems & Quick Fixes

### Problem: Computer Is Slow

**Quick fixes (try in order):**
1. Restart computer
2. Close unnecessary programs (check Task Manager)
3. Delete temporary files (Disk Cleanup on Windows)
4. Check storage space (need at least 10-15% free)
5. Scan for malware (Windows Defender scan)
6. Disable startup programs (Task Manager → Startup)

**Long-term fix:** Add more RAM or upgrade to SSD

### Problem: Internet Not Working

**Quick fixes:**
1. Turn WiFi off and on
2. Restart router (unplug 30 seconds)
3. Restart computer
4. Try a different website (maybe just one site is down)
5. Run network troubleshooter (Windows: Settings → Network → Troubleshoot)
6. Forget network and reconnect

**Check:** Is it just you? Ask family/neighbors or check phone

### Problem: Program Keeps Crashing

**Quick fixes:**
1. Restart the program
2. Restart computer
3. Update the program
4. Uninstall and reinstall
5. Check if file you're opening is corrupted (try a different file)
6. Run as administrator (right-click → Run as Administrator)

### Problem: Can't Print

**Quick fixes:**
1. Restart printer (turn off/on)
2. Check printer is connected (USB or same WiFi network)
3. Check ink/toner levels
4. Check for paper jams
5. Remove and re-add printer
6. Update printer drivers

### Problem: Blue Screen (Windows)

**Don't panic!** Windows will restart automatically.

**After it restarts:**
1. Note the error code (take a picture)
2. Google the error code
3. Think: What changed recently?
4. Run Windows Memory Diagnostic (search for it)
5. If frequent: Could be hardware issue (RAM, hard drive)

### Problem: Computer Won't Start

**Try these:**
1. Check it's plugged in (sounds obvious, happens often!)
2. Try a different power outlet
3. For laptops: Remove battery, hold power 30 sec, reinsert battery
4. Listen for fans/hard drive (any signs of life?)
5. Check monitor is on and connected
6. Try safe mode (restart, press F8 repeatedly)

**If nothing works:** Might be hardware failure → professional help needed

---

## 🛠️ Essential Troubleshooting Tools

### Built Into Windows

| Tool | What It Does | How to Access |
|------|--------------|---------------|
| **Task Manager** | See running programs, force close | Ctrl+Shift+Esc |
| **Event Viewer** | Detailed error logs | Search "Event Viewer" |
| **Disk Cleanup** | Free up space | Search "Disk Cleanup" |
| **System Restore** | Roll back to earlier state | Search "Create a restore point" |
| **Troubleshooters** | Automated fixers | Settings → Update & Security → Troubleshoot |

### Built Into Mac

| Tool | What It Does | How to Access |
|------|--------------|---------------|
| **Activity Monitor** | See running programs | Applications → Utilities |
| **Console** | Error logs | Applications → Utilities |
| **Disk Utility** | Fix disk problems | Applications → Utilities |
| **Safe Mode** | Boot with minimal stuff | Hold Shift during startup |

### Free Tools Worth Having

| Tool | What It Does | Get It At |
|------|--------------|-----------|
| **Malwarebytes Free** | Malware scanner | malwarebytes.com |
| **CrystalDiskInfo** | Check hard drive health | crystalmark.info |
| **HWMonitor** | Check temperatures | cpuid.com |
| **Recuva** | Recover deleted files | ccleaner.com/recuva |

---

## 📞 When to Ask for Help

### Try Everything First

Before asking for help, be able to answer:
1. What exactly is the problem?
2. When did it start?
3. What were you doing when it happened?
4. What have you tried already?
5. What's the exact error message?

### How to Ask for Help (Properly)

❌ **Bad:**
> "My computer is broken. Help!"

✅ **Good:**
> "Windows 11 laptop won't connect to WiFi. Started yesterday after Windows update. 
> I've tried: restarting router, restarting laptop, forgetting/reconnecting to network.
> Error says: 'Can't connect to this network'
> Phone connects fine to same WiFi.
> Any ideas?"

### Where to Ask

- **Reddit:** r/techsupport, r/computerhelp
- **Forums:** Tom's Hardware, SevenForums
- **Official support:** Microsoft, Apple, manufacturer
- **Local:** Friends, family, local repair shop

---

## ✅ Quick Checklist

- [ ] I always try restarting first
- [ ] I know how to search for error messages effectively
- [ ] I check for updates when something breaks
- [ ] I can identify what changed before a problem started
- [ ] I know basic tools (Task Manager, etc.)
- [ ] I can describe problems clearly when asking for help

---

## 🏃 What's Next?

Congratulations! You've completed the BASICS section!

Now open **`08-completed-basics.md`** to learn what to do next and which path to choose!
