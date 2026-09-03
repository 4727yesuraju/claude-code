# CLAUDE.md

## 📖 Simple English Explanation

`CLAUDE.md` is a **special instruction file for Claude Code**.

You put information about your project inside this file so Claude can understand **how your project works and how you want Claude to work**.

Claude Code reads this information when working on your project.

---

## 🤔 Why is it Needed?

Without `CLAUDE.md`, you may need to repeatedly tell Claude things like:

* Which technologies the project uses
* How the project is structured
* How to run the project
* How to run tests
* Coding rules to follow
* Important project-specific instructions

With `CLAUDE.md`, you can write these instructions **once**.

```text
CLAUDE.md
    ↓
Project rules + instructions
    ↓
Claude Code understands them
```

---

## 💻 Example

Suppose you have a MERN project.

You can create:

```text
my-project/
├── src/
├── package.json
└── CLAUDE.md
```

Inside `CLAUDE.md`:

```md
# Project Instructions

## Tech Stack

- React
- Node.js
- Express
- MongoDB

## Rules

- Use JavaScript
- Use functional React components
- Use async/await
- Write tests for new features

## Commands

- npm run dev
- npm test
```

Now Claude Code has this project-specific context when working on your code.

---

## 🌊 How It Works

```text
You create CLAUDE.md
        ↓
Add project instructions
        ↓
Claude Code reads the instructions
        ↓
Claude works according to them
```

---

## 📍 Where Can It Be?

A `CLAUDE.md` file can provide instructions at different levels, such as:

```text
Global instructions
       ↓
Project instructions
       ↓
Subdirectory instructions
```

This allows instructions to be specific to different parts of your development environment.

---

## 🎯 Simple Understanding

> **`CLAUDE.md` = A project instruction file for Claude Code.**

Think of it as:

```text
CLAUDE.md
    =
"How Claude should understand and work with my project"
```
