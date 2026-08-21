---
tags: [template, obsidian, note-structure]
aliases: [Note Template, Daily Note Template, Project Template]
difficulty: 1
status: active
---

# Obsidian Templates

Copy these templates into your Obsidian templates folder and use them with the Templates plugin.

## Daily Learning Note Template

Save as `Templates/Daily-Learning.md`:

```markdown
---
date: {{date}}
tags: [daily-log]
difficulty: 1
status: active
---

# Learning Log - {{date:YYYY-MM-DD}}

## Focus Area
- 

## What I Learned
- 

## Challenges Faced
- 

## Questions to Research
- 

## Time Spent
- Total: ___ minutes
- Deep work: ___ minutes

## Mood/Energy
- [ ] High
- [ ] Medium
- [ ] Low

## Tomorrow's Priority
- 

---
**Resources Used:**
- 

**Wins Today:**
- 
```

## Concept Note Template

Save as `Templates/Concept-Note.md`:

```markdown
---
tags: [concept, topic]
aliases: []
related: []
difficulty: 2
status: learning
---

# {{title}}

## Summary
One sentence explanation of this concept.

## Why It Matters
Explain why this concept is important in IT/CS.

## Key Points
- Point 1
- Point 2
- Point 3

## Simple Explanation (ELI5)
Explain like I'm 12. Use analogies.

## Technical Details
Deeper dive into how it works.

## Examples
```language
// Code example or configuration
```

## Common Mistakes
- Mistake 1 and how to avoid it
- Mistake 2 and how to avoid it

## Related Concepts
- [[Related Concept 1]]
- [[Related Concept 2]]

## Practice Exercises
- [ ] Exercise 1
- [ ] Exercise 2

## Resources
- Link to documentation
- Link to tutorial
- Link to video

## Flashcards (Anki)
Question::Answer
Question::Answer
```

## Project Note Template

Save as `Templates/Project-Note.md`:

```markdown
---
project-name: {{title}}
start-date: {{date:YYYY-MM-DD}}
end-date: 
tags: [project, portfolio]
technologies: []
status: planning
difficulty: 3
---

# Project: {{title}}

## Overview
What are you building and why?

## Features
### MVP (Must Have)
- [ ] Feature 1
- [ ] Feature 2

### Nice to Have
- [ ] Feature 3
- [ ] Feature 4

## Tech Stack
- Language: 
- Framework: 
- Database: 
- Tools: 

## Timeline
- [ ] Planning (Date)
- [ ] Setup (Date)
- [ ] Core Features (Date)
- [ ] Polish (Date)
- [ ] Deploy (Date)

## Learning Goals
What do you want to learn from this project?
- 

## Challenges
What obstacles do you anticipate?
- 

## Resources
- Documentation links
- Tutorial links
- Inspiration projects

## Deployment
- Hosting platform: 
- Domain: 
- Status: 

## Post-Mortem (After Completion)
What went well?
- 

What would you do differently?
- 

What did you learn?
- 
```

## Meeting Notes Template

Save as `Templates/Meeting-Notes.md`:

```markdown
---
date: {{date:YYYY-MM-DD}}
time: {{time}}
attendees: []
tags: [meeting, notes]
---

# Meeting: {{title}}

## Agenda
1. 
2. 
3. 

## Discussion Notes
- 

## Decisions Made
- [ ] Decision 1
- [ ] Decision 2

## Action Items
- [ ] Task - Assignee - Due Date
- [ ] Task - Assignee - Due Date

## Questions to Follow Up
- 

## Next Meeting
Date: 
Agenda items:
- 
```

## How to Use Templates

1.  Go to Obsidian Settings > Core Plugins > Templates
2.  Enable the Templates plugin
3.  Set template folder location to `99-Templates`
4.  Use Ctrl/Cmd + T to insert a template
5.  Customize templates to fit your workflow

> [!TIP]
> Install the "Templater" community plugin for advanced features like automatic date formatting, cursor positioning, and JavaScript execution in templates.

## See Also
- [[00-TRACKERS/README|Progress Trackers]] - Use daily notes for tracking
- [[00-PROFESSIONALISM/README|Professionalism Guide]] - Use meeting notes for work
- [[README|Dashboard]] - Return to main guide
