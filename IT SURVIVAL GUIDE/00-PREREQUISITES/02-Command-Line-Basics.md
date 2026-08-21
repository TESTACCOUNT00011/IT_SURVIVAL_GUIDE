---
tags: [prerequisite, cli, terminal, command-line]
aliases: [Terminal Basics, CLI Fundamentals]
difficulty: 2
---

# Command Line Basics

## What is the Command Line?
The Command Line Interface (CLI) is a text-based way to control your computer. Instead of clicking icons, you type commands. It feels scary at first, but it is incredibly powerful.

## Why Learn It?
- **Speed**: Typing `mkdir project` is faster than right-click -> new folder -> name it.
- **Automation**: You can run 100 commands in one line.
- **Remote Control**: Servers often have no mouse interface. You MUST use the command line to manage them.
- **Developer Standard**: Every programmer uses the terminal daily.

## Basic Commands (Work on Mac, Linux, and Windows PowerShell)

| Command | Meaning | Example |
|---------|---------|---------|
| `pwd` | Print Working Directory (Where am I?) | `pwd` |
| `ls` | List files (What is here?) | `ls` |
| `cd` | Change Directory (Move) | `cd Documents` |
| `mkdir` | Make Directory (Create folder) | `mkdir my_project` |
| `touch` | Create empty file | `touch index.html` |
| `cp` | Copy | `cp file.txt backup.txt` |
| `mv` | Move or Rename | `mv old.txt new.txt` |
| `rm` | Remove (Delete) | `rm file.txt` |
| `cat` | Show file content | `cat file.txt` |

## Navigation Logic
Think of folders as a tree structure.
- `.` means "current folder".
- `..` means "parent folder" (one level up).
- `/` or `\` separates folders (e.g., `Documents/Projects/Code`).

### Examples
- Go home: `cd ~`
- Go up one level: `cd ..`
- Go to specific folder: `cd Documents/Projects`

> [!WARNING] The Danger of `rm`
> In the terminal, there is no Recycle Bin. If you type `rm important_file.txt`, it is gone forever. Double-check before pressing Enter.

## Micro-Challenge
1. Open your Terminal (Search "Terminal" on Mac/Linux, "PowerShell" on Windows).
2. Type `pwd` to see where you are.
3. Type `mkdir practice_folder`.
4. Type `cd practice_folder`.
5. Type `touch test.txt`.
6. Type `ls` to see the file.
7. Type `cd ..` to go back.
8. Type `rm -r practice_folder` to delete it.

You just used the command line like a pro.
