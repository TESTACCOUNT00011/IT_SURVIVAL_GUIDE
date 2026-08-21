---
tags: [prerequisite, git, version-control, github]
aliases: [Git Basics, Version Control Fundamentals]
difficulty: 2
---

# Git and Version Control

## What is Git?
Git is a tool that saves snapshots of your code over time. Imagine playing a video game where you can save your progress at any point. If you make a mistake later, you can load an older save file. That is Git.

## Why Use It?
- **Undo Mistakes**: Broke something? Revert to yesterday's version.
- **Collaboration**: Multiple people can work on the same project without overwriting each other.
- **Portfolio**: Employers expect to see your code on GitHub (a website that hosts Git projects).

## Key Terms
- **Repository (Repo)**: The folder containing your project and its history.
- **Commit**: A saved snapshot of your changes.
- **Push**: Sending your commits to the cloud (GitHub).
- **Pull**: Downloading updates from the cloud.
- **Branch**: A parallel version of your project. You create a branch to try new ideas safely.
- **Merge**: Combining changes from two branches.

## Basic Workflow

```text
1. git init          # Start tracking a folder
2. git add .         # Stage all changes for saving
3. git commit -m "message"  # Save with a note
4. git push          # Send to GitHub
```

## Visualizing the Process

```text
[Your Computer]                  [GitHub Cloud]
     |                                 ^
     |--- git add (stage)              |
     |--- git commit (save)            |
     |--- git push (upload) ---------->+
                                       |
                                       +--- git pull (download) ---> [Your Computer]
```

> [!WARNING] Commit Messages Matter
> Do not write "fix" or "update". Write clear messages like "Added login button" or "Fixed crash on startup". Your future self will thank you.

## Micro-Challenge
1. Create a free account on [GitHub.com](https://github.com).
2. Install Git on your computer (search "Install Git").
3. Create a folder named `test-repo`.
4. Open terminal in that folder and run `git init`.
5. Create a text file, run `git add .`, then `git commit -m "First commit"`.

You have now used version control.
