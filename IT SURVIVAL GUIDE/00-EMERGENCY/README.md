---
tags: [emergency, troubleshooting, recovery, broken]
aliases: [I Broke It, Disaster Recovery]
difficulty: 1
---

# Emergency Recovery Guide

When things go wrong, do not panic. Most problems are reversible. Follow these steps before assuming the worst.

## Immediate Actions

### 1. Did You Just Install Something?
- **Action**: Uninstall it immediately.
- **Windows**: Settings > Apps > Installed Apps > Uninstall.
- **Mac**: Drag from Applications to Trash.
- **Linux**: `sudo apt remove [package-name]` or `sudo dnf remove [package-name]`.

### 2. Is Your Computer Running Slow or Acting Weird?
- **Action**: Restart in Safe Mode.
- **Windows**: Hold Shift while clicking Restart > Troubleshoot > Advanced Options > Startup Settings > Restart > Press 4 for Safe Mode.
- **Mac**: Shut down, then turn on and immediately hold Shift until login window appears.
- **Why**: Safe Mode loads only essential drivers. If the problem disappears, a recently installed program is the cause.

### 3. Did You Click a Suspicious Link?
- **Action**: Disconnect from the internet immediately (unplug Ethernet or turn off Wi-Fi).
- **Next**: Run a full antivirus scan.
    - **Windows**: Windows Defender (built-in) > Full Scan.
    - **Mac**: Malwarebytes (free version).
    - **Linux**: ClamAV.
- **Change Passwords**: From a different, safe device (like your phone), change your email and banking passwords.

### 4. Did You Delete Something Important?
- **Action**: Check the Recycle Bin / Trash immediately.
- **If Empty**: Stop using the computer immediately. Every new file saved might overwrite the deleted data.
- **Recovery Tools**: Recuva (Windows), TestDisk (Cross-platform). Success is not guaranteed but worth trying.

### 5. Is the Screen Blue / Black / Frozen?
- **Blue Screen (Windows)**: Note the error code (e.g., `CRITICAL_PROCESS_DIED`). Google this code on your phone.
- **Black Screen**: Try `Ctrl + Alt + Del`. If Task Manager opens, the display driver might be crashed. Restart Explorer.exe.
- **Frozen**: Hold the power button for 10 seconds to force shutdown. Wait 30 seconds, then turn back on.

## Common Error Messages Explained

| Error Message | What It Means | Quick Fix |
|---------------|---------------|-----------|
| "DLL Missing" | A required file is gone | Reinstall the program. Do not download DLLs from random sites. |
| "Permission Denied" | You don't have rights to edit this | Right-click > Run as Administrator (Windows) or use `sudo` (Linux/Mac). |
| "No Boot Device Found" | Computer can't find the hard drive | Check cables. BIOS might need to reset boot order. |
| "404 Not Found" | Website page doesn't exist | Typo in URL or page was deleted. Nothing wrong with your computer. |
| "500 Internal Server Error" | Website's server is broken | Wait and try again later. Not your fault. |

## When to Ask for Help

If you have tried the above and still cannot fix it:
1.  **Google the exact error message**. Add your OS version (e.g., "Windows 11 blue screen critical_process_died").
2.  **Check Reddit**: r/techsupport or r/computerhelp.
3.  **Provide Details**: When asking, include:
    - What you were doing when it broke.
    - The exact error message.
    - Your operating system.
    - What you have already tried.

> [!TIP] Prevention
> Create a "System Restore Point" (Windows) or use "Time Machine" (Mac) before installing major updates or new software. This lets you roll back time if something breaks.
