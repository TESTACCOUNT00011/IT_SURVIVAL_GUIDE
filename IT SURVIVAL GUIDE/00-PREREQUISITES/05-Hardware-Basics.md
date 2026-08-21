---
tags: [prerequisite, hardware, computer-science]
aliases: [Hardware Fundamentals, Computer Components]
difficulty: 2
---

# Hardware Basics

## The Big Four Components
Every computer, from a smartphone to a supercomputer, has these four main parts.

### 1. CPU (Central Processing Unit)
- **What it is**: The brain of the computer.
- **Job**: Executes instructions and performs calculations.
- **Analogy**: The chef in a kitchen. The faster the chef, the quicker the meal.
- **Key Spec**: Cores and Clock Speed (GHz). More cores = multitasking. Higher GHz = faster single tasks.

### 2. RAM (Random Access Memory)
- **What it is**: Short-term memory.
- **Job**: Holds data for programs currently running.
- **Analogy**: The kitchen counter. A bigger counter lets you prepare more dishes at once. If the counter is full, you have to put things away (slow) to make space.
- **Key Fact**: RAM is wiped when the computer turns off.

### 3. Storage (SSD/HDD)
- **What it is**: Long-term memory.
- **Job**: Stores your files, OS, and programs permanently.
- **Analogy**: The pantry or fridge. Holds ingredients until you need them on the counter (RAM).
- **Types**:
    - **SSD**: Fast, silent, expensive. (Get this one).
    - **HDD**: Slow, noisy, cheap. (Avoid for OS).

### 4. GPU (Graphics Processing Unit)
- **What it is**: Specialized processor for images.
- **Job**: Renders video games, video editing, and AI tasks.
- **Analogy**: A specialized pastry chef. The main chef (CPU) can do it, but the pastry chef (GPU) does it much faster.

## How They Work Together

```text
[Storage] --loads--> [RAM] --feeds--> [CPU] --outputs--> [Monitor]
                           ^
                           |
                       [GPU]
```

1. You open a program (stored on **SSD**).
2. It loads into **RAM** so it runs fast.
3. The **CPU** processes your clicks and logic.
4. The **GPU** draws the windows and images on your screen.

## Bottlenecks
A bottleneck is when one slow component holds back the fast ones.
- Fast CPU + Slow RAM = Computer waits for data.
- Fast CPU + Old HDD = Computer feels sluggish loading apps.

> [!TIP] Buying Advice
> For learning IT: Prioritize RAM (16GB minimum) and an SSD. A slightly older CPU with lots of RAM is better than a new CPU with only 4GB RAM.

## Micro-Challenge
1. On Windows: Press `Ctrl+Shift+Esc` to open Task Manager. Click "Performance".
2. On Mac: Press `Cmd+Space`, type "Activity Monitor".
3. Identify your CPU name, RAM amount, and Disk type.
