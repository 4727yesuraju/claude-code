# Skills

## 📖 Simple English Explanation

**Skills** are reusable instructions that teach Claude Code **how to perform a specific type of task**.

You create a skill by putting instructions in a `SKILL.md` file. Claude Code can then use that skill when the task matches its purpose.

---

## 🤔 Why is it Needed?

Instead of explaining the same process every time, you can define it once.

```text
Create Skill
     ↓
Write Instructions
     ↓
Claude uses the Skill
     ↓
Same task → Same workflow
```

---

## 🛠️ How to Create a Skill

### 1. Create a Skills Folder

For a project skill:

```text
.claude/
└── skills/
    └── code-review/
        └── SKILL.md
```

### 2. Create `SKILL.md`

Example:

```md
---
name: code-review
description: Review code for bugs, security, and readability.
---

# Code Review

When reviewing code:

1. Check for bugs
2. Check security issues
3. Check readability
4. Check performance
5. Suggest improvements
```

The `description` helps Claude understand **when the skill is relevant**.

---

## ▶️ How to Use a Skill

Once the skill is available, ask Claude to perform the task it was created for.

Example:

```text
Review this code using the code-review skill.
```

Claude can use the instructions from the skill to perform the review.

You can also make the skill **automatically relevant** by giving it a clear description of when it should be used.

---

## 📍 Skill Location

Skills can be created at different levels.

### Project Skill

```text
.claude/skills/
```

Useful when the skill is specific to one project.

### Personal Skill

```text
~/.claude/skills/
```

Useful when you want to reuse the skill across your projects.

---

## 💻 Real Example

Suppose you always want API code reviewed in the same way.

Create:

```text
.claude/
└── skills/
    └── api-review/
        └── SKILL.md
```

`SKILL.md`:

```md
---
name: api-review
description: Review API code for validation, errors, security, and performance.
---

# API Review

Check:

1. Request validation
2. Error handling
3. Authentication and authorization
4. Security
5. Performance
6. Code quality
```

Now when you need an API review:

```text
Review this API using the API review skill.
```

Claude follows the defined workflow.

---

## 🌊 Simple Flow

```text
Create .claude/skills/
          ↓
Create skill folder
          ↓
Create SKILL.md
          ↓
Add instructions
          ↓
Claude discovers the skill
          ↓
Use it for matching tasks
```

---

## 🎯 Simple Understanding

> **Skill = A reusable `SKILL.md` file that teaches Claude how to perform a specific task.**

Think:

```text
CLAUDE.md
    ↓
General project instructions

SKILL.md
    ↓
Specific task instructions
```
