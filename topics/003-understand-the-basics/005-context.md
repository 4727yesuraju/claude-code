# Context

## 📖 Simple English Explanation

**Context** is the information Claude Code can see and use while working on your task.

It helps Claude understand **what you are working on, what you already discussed, and what files or instructions are relevant**.

For example, if you ask:

```text
Fix the bug in the customer API.
```

Claude needs context about the project, the API, related files, and your instructions to make a good change.

---

## 🤔 Why is it Needed?

Without enough context, Claude may not fully understand your project or task.

With good context, Claude can:

* Understand your code better
* Give more relevant answers
* Make better code changes
* Follow your project instructions
* Avoid asking unnecessary questions

---

## 🌊 How Context Works

```text
Your Task
   ↓
Project Context
   ↓
CLAUDE.md Instructions
   ↓
Relevant Files / Code
   ↓
Claude understands the situation
   ↓
Response / Code Changes
```

---

## 💻 Example

Suppose your project has:

```text
src/
├── controllers/
├── services/
├── repositories/
└── routes/
```

You ask:

```text
Add a customer search API.
```

Claude needs to understand things such as:

```text
Which route structure do we use?
Which service handles customers?
How are repositories written?
What coding rules should I follow?
```

This information becomes part of the **context** Claude uses to complete the task.

---

## 🔑 Important Idea

Claude Code does not simply look at one file.

It can use relevant information from the project and instructions to understand the task.

But **more context is not always better**.

You want to give Claude the **right context**:

```text
Too little context → Claude may misunderstand

Right context → Better result

Too much unnecessary context → Can make the task harder
```

---

## 🎯 Simple Understanding

> **Context = Information Claude needs to understand and complete your task correctly.**

Think:

```text
Context
   =
"Everything relevant Claude needs to know"
```
