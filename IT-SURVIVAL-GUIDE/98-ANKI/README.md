# 🧠 Anki Flashcard Guide

Boost your IT learning with spaced repetition! This guide shows you how to use Anki flashcards effectively with the IT Survival Guide.

## 📚 What is Anki?

**Anki** is a free, open-source flashcard app that uses **spaced repetition** to help you remember information long-term. It's perfect for:
- Memorizing IT terminology
- Learning commands and syntax
- Preparing for certifications (CompTIA A+, Network+, Security+, etc.)
- Retaining coding concepts

## 🚀 Getting Started

### Step 1: Install Anki
1. Download from [ankiweb.net](https://apps.ankiweb.net/)
2. Install on your computer (Windows/Mac/Linux)
3. Optional: Install **AnkiDroid** (Android) or **AnkiMobile** (iOS) for mobile study

### Step 2: Import Flashcard Decks
This guide provides pre-made decks for each career path:

#### Available Decks

All decks are ready to import! Each CSV file contains 25-30 essential terms for that career path:

- [[decks/IT-Support-Basics|IT Support Fundamentals]] - Hardware, networking, troubleshooting (25 cards)
- [[decks/Web-Dev-Basics|Web Development Basics]] - HTML, CSS, JS, React, backend (30 cards)
- [[decks/Cybersecurity-Basics|Cybersecurity Fundamentals]] - CIA triad, attacks, tools, cryptography (30 cards)
- [[decks/Data-Analysis-Basics|Data Analysis Basics]] - Excel, SQL, Python, statistics, visualization (30 cards)
- [[decks/Cloud-Computing-Basics|Cloud Computing Basics]] - AWS/Azure, service models, containers, serverless (30 cards)
- [[decks/General-IT-Terms|General IT Terminology]] - Universal concepts across all paths (40+ cards)

#### How to Import
1. Download the `.apkg` file from the deck folder
2. Open Anki on your computer
3. Click **File → Import**
4. Select the downloaded `.apkg` file
5. Choose the deck name and click **Import**

### Step 3: Start Studying
1. Select a deck in Anki
2. Click **Study Now**
3. Review cards daily (aim for 10-20 minutes)
4. Let Anki schedule reviews automatically

## 📝 Creating Your Own Cards

### From Your Notes
Use the [[../../00-TEMPLATES/Learning-Summary|Learning Summary Template]] to identify key concepts, then:

1. **Front of Card**: Question or term
   - Example: "What does CPU stand for?"
   
2. **Back of Card**: Answer or definition
   - Example: "Central Processing Unit - the brain of the computer"

### Best Practices for IT Cards
✅ **Do:**
- Keep cards simple (one concept per card)
- Use cloze deletions for commands: `The command to list files in Linux is {{c1::ls}}`
- Add context: "In Windows PowerShell, what command...?"
- Include examples on the back
- Tag cards by topic: `#networking`, `#linux`, `#security`

❌ **Don't:**
- Put multiple facts on one card
- Make cards too vague
- Forget to add tags
- Create cards without understanding the concept first

### Card Types

#### Basic Card
```
Front: What port does HTTPS use?
Back: Port 443
```

#### Cloze Deletion (Fill-in-the-blank)
```
Text: The {{c1::ping}} command tests network connectivity using {{c2::ICMP}} packets.
```

#### Reversal Card (Learn both directions)
```
Front: What does DNS stand for?
Back: Domain Name System

(Reverse also generated)
Front: What system translates domain names to IP addresses?
Back: DNS (Domain Name System)
```

## 📅 Study Routine

### Daily Practice (Recommended)
- **Morning**: Review due cards (10-15 min)
- **During Study Sessions**: Create 3-5 new cards from what you learn
- **Evening**: Quick review if you have many due cards

### Weekly Review
- Check your stats in Anki
- Identify difficult cards (low retention)
- Edit or delete poorly written cards
- Add new cards from weekly learnings

### Before Exams
- Increase daily review time (20-30 min)
- Create exam-specific decks
- Focus on weak areas identified in stats

## 🏷️ Tagging System

Organize your cards with tags for easy filtering:

```
#it-support      #web-dev      #cybersecurity
#networking      #linux        #windows
#comptia-a+      #security+    #ccna
#commands        #definitions  #troubleshooting
```

## 📊 Tracking Progress

### Anki Stats to Watch
- **Retention Rate**: Aim for 80-90%
- **Cards Due Today**: Keep manageable (20-50 cards)
- **New Cards per Day**: 5-15 new cards is sustainable
- **Time Spent**: 10-30 minutes daily

### Linking to Your Notes
In Obsidian, link Anki cards to detailed notes:
```
See full explanation in [[Network-Protocols]]
Related lab: [[../../05-PATHS/01-IT-Support/Labs/Packet-Tracer-Basics]]
```

## 🔌 Useful Add-ons

Install these Anki add-ons for enhanced functionality:

1. **Image Occlusion Enhanced** - Hide parts of diagrams (great for network topologies)
2. **Cloze Overlapper** - Create overlapping cloze cards
3. **Review Heatmap** - Visualize your study consistency
4. **Card Browser Go** - Advanced card search and filtering

## 🆘 Troubleshooting

### Common Issues

**Problem**: Too many cards due every day  
**Solution**: Reduce new cards/day limit in deck options (start with 5-10)

**Problem**: Forgetting cards quickly  
**Solution**: 
- Simplify the card (one fact per card)
- Add mnemonics or images
- Understand the concept before making the card

**Problem**: Don't know where to start  
**Solution**: Begin with the [[decks/General-IT-Terms|General IT Terms]] deck, then branch into your career path

## 📦 Contributing Decks

Want to create a deck for the community?
1. Follow the card best practices above
2. Tag cards appropriately
3. Export as `.apkg` file
4. Submit to the [[../../99-RESOURCES/README|Resources Index]] or community forums

---

## 🔗 Quick Links
- [[decks|Browse All Decks]]
- [[../../00-TEMPLATES/Learning-Summary|Learning Summary Template]] - Create cards from your notes
- [[../../02-BASICS/GLOSSARY/README|IT Glossary]] - Source material for cards
- [[../../99-RESOURCES/README|Resources Hub]] - More learning tools

**Ready to start?** Download your first deck below! 👇
