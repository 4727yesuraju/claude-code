# Skills

## 📖 Simple English Explanation

**Skills** are reusable instructions that teach Claude Code **how to perform a specific type of task**.

Instead of giving Claude the same detailed instructions every time, you can create a skill once and reuse it whenever needed.

For example, you could have skills for:

* Code review
* Testing
* Documentation
* Creating API endpoints
* Database work

---

## 🤔 Why is it Needed?

Without skills, you may repeatedly explain the same process to Claude.

With a skill:

```text
Create Skill
     ↓
Define how to do a task
     ↓
Claude follows those instructions
     ↓
Reuse the skill whenever needed
```

This makes your workflow **more consistent and faster**.

---

## 💻 Example

Suppose you frequently ask Claude to review code.

You can create a **code-review skill** that tells Claude:

```text
1. Check readability
2. Check bugs
3. Check security issues
4. Check performance
5. Suggest improvements
```

Then, when you use that skill, Claude follows the same review process each time.

---

## 🌊 Skills vs CLAUDE.md

These two are related but have different purposes.

| `CLAUDE.md`                              | Skills                                        |
| ---------------------------------------- | --------------------------------------------- |
| General project instructions             | Instructions for a specific task              |
| Tells Claude how to work in your project | Tells Claude how to perform a particular task |
| Usually applies broadly                  | Can be reused when needed                     |

### Simple Example

```text
CLAUDE.md
    ↓
"Use TypeScript and follow our project coding rules."

Skill
    ↓
"When reviewing code, check security,
performance, readability, and tests."
```

---

## 🎯 Simple Understanding

> **Skills = Reusable instructions for specific tasks.**

Think:

```text
CLAUDE.md → How Claude should work in my project

Skills → How Claude should perform a specific task
```
