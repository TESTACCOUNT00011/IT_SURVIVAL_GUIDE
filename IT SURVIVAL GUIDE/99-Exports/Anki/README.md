---
tags: [anki, flashcards, spaced-repetition, export]
aliases: [Flashcards, SRS Decks]
difficulty: 1
status: active
---

# Anki Flashcard Exports

This folder contains Comma Separated Value (CSV) files ready to be imported into Anki or any compatible Spaced Repetition System (SRS).

## How to Use These Files

1.  **Install Anki**: Download from [apps.ankiweb.net](https://apps.ankiweb.net).
2.  **Import**:
    - Open Anki.
    - Click "File" -> "Import".
    - Select the CSV file (e.g., `basics-vocabulary.csv`).
    - Ensure "Field separator" is set to **Comma** or **Semicolon** as noted in the file header.
3.  **Study**: Aim for 10-15 minutes daily. Consistency matters more than volume.

## Available Decks

| File Name | Topic | Difficulty | Count |
| :--- | :--- | :--- | :--- |
| `basics-vocabulary.csv` | IT Basics & Terminology | Beginner | 50 |
| `linux-commands.csv` | Essential Linux Commands | Beginner | 40 |
| `networking-basics.csv` | IP, DNS, Ports, OSI Model | Intermediate | 60 |
| `security-concepts.csv` | Security Fundamentals | Intermediate | 50 |
| `web-dev-basics.csv` | HTML, CSS, JS Concepts | Beginner | 70 |

> [!WARNING] Do Not Memorize Blindly
> Flashcards are for reinforcing concepts you have already encountered. If a card makes no sense, stop and read the relevant documentation first. Context is key.

## Creating Your Own Cards
As you learn, create your own cards for things you forget. The act of creating the card is often more valuable than reviewing it.

Format: `Front,Back,Tags,Difficulty`
Example: `What does DNS do?,Translates domain names to IP addresses,#networking #basics,1`
