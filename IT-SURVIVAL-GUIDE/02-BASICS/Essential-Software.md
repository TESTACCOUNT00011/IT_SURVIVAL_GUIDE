# 🛠️ Essential Software Installation Guide

Get your development environment set up with these essential tools. Follow the installation guides for your operating system.

---

## 📋 Quick Setup Checklist

### Everyone Needs These
- [ ] Web Browser (Chrome or Firefox)
- [ ] Text Editor / IDE (VS Code)
- [ ] Password Manager (Bitwarden)
- [ ] Cloud Storage (Google Drive, OneDrive, or Dropbox)
- [ ] Communication Tools (Discord, Slack)

### Path-Specific Tools
See sections below for your career path requirements.

---

## 🌐 Universal Tools (All Paths)

### 1. Web Browser
**Recommended**: Google Chrome or Mozilla Firefox

**Why**: Modern web development and IT work require a reliable, standards-compliant browser.

**Install**:
- **Windows/Mac**: Download from [chrome.google.com](https://www.google.com/chrome/) or [firefox.com](https://www.mozilla.org/firefox/)
- **Linux**: `sudo apt install chromium-browser` or `sudo apt install firefox`

**Essential Extensions**:
- uBlock Origin (ad blocking)
- LastPass or Bitwarden (password management)
- JSON Viewer (data formatting)

---

### 2. Code Editor: Visual Studio Code (VS Code)
**Recommended**: VS Code (free)

**Why**: Industry-standard editor with excellent extensions and debugging tools.

**Install**:
- **All Platforms**: Download from [code.visualstudio.com](https://code.visualstudio.com/)

**Essential Extensions**:
- Prettier - Code formatter
- ESLint - JavaScript linting
- Python (if using Python)
- GitLens - Git integration
- Live Server - Local web server
- Auto Rename Tag - HTML/XML tag renaming
- Path Intellisense - Autocomplete file paths

---

### 3. Password Manager
**Recommended**: Bitwarden (free)

**Why**: Security is critical in IT. Never reuse passwords!

**Install**:
- Download from [bitwarden.com](https://bitwarden.com/)
- Install browser extension
- Create strong master password
- Enable two-factor authentication

---

### 4. Git & GitHub
**Recommended**: Git + GitHub Desktop (beginner-friendly)

**Why**: Version control is essential for all IT paths.

**Install Git**:
- **Windows**: Download from [git-scm.com](https://git-scm.com/)
- **Mac**: `brew install git` or download from website
- **Linux**: `sudo apt install git`

**Install GitHub Desktop** (Optional but helpful):
- Download from [desktop.github.com](https://desktop.github.com/)

**Basic Setup**:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

### 5. Terminal/Command Line Tools

#### Windows Users:
**Install Windows Terminal** (recommended over Command Prompt):
- Download from Microsoft Store
- Or: `winget install Microsoft.WindowsTerminal`

**Install WSL2** (Windows Subsystem for Linux):
```powershell
wsl --install
```
This gives you a real Linux environment on Windows!

#### Mac Users:
- Terminal app is pre-installed (Applications > Utilities > Terminal)
- Optional: Install iTerm2 for enhanced features

#### Linux Users:
- Terminal is pre-installed
- Try different shells: bash, zsh, fish

---

## 🖥️ IT Support Path

### Additional Software:
- [ ] **PuTTY** - SSH client (Windows)
- [ ] **WinSCP** - File transfer (Windows)
- [ ] **VirtualBox** - Virtual machines
- [ ] **Wireshark** - Network analysis
- [ ] **Nmap** - Network scanning

**Install Commands**:
```bash
# Ubuntu/Debian
sudo apt install putty winscp virtualbox wireshark nmap

# macOS (with Homebrew)
brew install --cask virtualbox wireshark nmap
```

---

## 🌐 Web Development Path

### Additional Software:
- [ ] **Node.js & npm** - JavaScript runtime
- [ ] **Git** - Version control (see above)
- [ ] **Browser DevTools** - Built into Chrome/Firefox
- [ ] **Postman** - API testing
- [ ] **Docker** - Containerization (optional for beginners)

**Install Node.js**:
- Download from [nodejs.org](https://nodejs.org/) (LTS version recommended)
- Verify: `node --version` and `npm --version`

**Install Postman**:
- Download from [postman.com](https://www.postman.com/)

**Install Docker** (when ready):
- Download from [docker.com](https://www.docker.com/products/docker-desktop)

---

## 🔒 Cybersecurity Path

### Additional Software:
- [ ] **Kali Linux** - Security testing OS (run in VM)
- [ ] **VirtualBox/VMware** - Virtual machines
- [ ] **Wireshark** - Network analysis
- [ ] **Nmap** - Network scanning
- [ ] **Burp Suite Community** - Web security testing
- [ ] **John the Ripper** - Password cracking (educational)

**Important**: Only use security tools on systems you own or have permission to test!

**Install Kali in VirtualBox**:
1. Download VirtualBox from [virtualbox.org](https://www.virtualbox.org/)
2. Download Kali ISO from [kali.org](https://www.kali.org/)
3. Create new VM and install Kali

---

## 📊 Data Analysis Path

### Additional Software:
- [ ] **Python** - Programming language
- [ ] **Anaconda** - Python distribution for data science
- [ ] **Jupyter Notebook** - Interactive coding (comes with Anaconda)
- [ ] **R & RStudio** - Statistical computing (optional)
- [ ] **SQLite Browser** - Database viewer
- [ ] **Tableau Public** - Data visualization (free version)

**Install Anaconda** (Recommended for beginners):
- Download from [anaconda.com](https://www.anaconda.com/)
- Includes: Python, Jupyter, pandas, NumPy, matplotlib, and more!

**Install Python** (Alternative):
- Download from [python.org](https://www.python.org/)
- Install pip packages: `pip install pandas numpy matplotlib jupyter`

**Install R & RStudio**:
- Download R from [cran.r-project.org](https://cran.r-project.org/)
- Download RStudio from [rstudio.com](https://posit.co/download/rstudio-desktop/)

---

## ☁️ Cloud Computing Path

### Additional Software:
- [ ] **AWS CLI** - Amazon Web Services command line
- [ ] **Azure CLI** - Microsoft Azure command line
- [ ] **Terraform** - Infrastructure as code
- [ ] **Docker** - Containerization
- [ ] **kubectl** - Kubernetes command line
- [ ] **VS Code Extensions**: AWS Toolkit, Azure Tools

**Install AWS CLI**:
```bash
# macOS
brew install awscli

# Windows
# Download installer from aws.amazon.com/cli

# Linux
sudo apt install awscli
```

**Install Azure CLI**:
```bash
# macOS
brew install azure-cli

# Windows
# Download from docs.microsoft.com/cli/azure

# Linux
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

**Install Terraform**:
```bash
# macOS
brew install terraform

# Windows
choco install terraform

# Linux
wget https://releases.hashicorp.com/terraform/1.0.0/terraform_1.0.0_linux_amd64.zip
unzip terraform_1.0.0_linux_amd64.zip
sudo mv terraform /usr/local/bin/
```

---

## ✅ Verification Checklist

After installation, verify everything works:

```bash
# Check versions of installed software
git --version
node --version
npm --version
python --version
python3 --version
java --version  # If installed
docker --version  # If installed

# Test VS Code
code --version

# Test terminal
echo "Terminal is working!"
```

---

## 🔧 Troubleshooting Common Issues

### "Command not found" errors
**Solution**: The software isn't installed or not in your PATH. Restart your terminal/computer after installation.

### Permission denied errors
**Solution** (Mac/Linux): Add `sudo` before commands or fix permissions:
```bash
sudo chown -R $(whoami) /path/to/directory
```

### Windows: Scripts won't run
**Solution**: Open PowerShell as Administrator and run:
```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### Port already in use
**Solution**: Kill the process using the port or use a different port:
```bash
# Find process using port 8080
lsof -i :8080

# Kill it
kill -9 [PID]
```

---

## 💡 Pro Tips

1. **Keep software updated** - Set reminders to check for updates monthly
2. **Use package managers** - Homebrew (Mac), Chocolatey (Windows), apt (Linux)
3. **Organize your projects** - Create a `/projects` or `/code` folder
4. **Backup your configs** - Save your dotfiles (.bashrc, .vimrc, etc.) to GitHub
5. **Learn keyboard shortcuts** - They save hours over time!

---

## 🔗 Related Resources

- [[../01-START-HERE/Day-1-Checklist|Day 1 Checklist]] - Get started today
- [[../00-TEMPLATES/Code-Snippet|Code Snippet Template]] - Store useful commands
- [[../99-RESOURCES/README|Resources Hub]] - More tools and utilities
- [[../02-BASICS/GLOSSARY/README|Glossary]] - Understand technical terms

---

*Last updated: {{date}}*  
*Tags: #setup #software #tools #installation #beginner*

**Need help?** Check the [[../01-START-HERE/FAQ/README|FAQ]] or ask in community forums!
