# Modes

## 📖 Simple English Explanation

**Modes** control **how Claude Code works with you and your code**.

Different modes give Claude different levels of freedom when performing tasks.

For example, Claude may only suggest changes in one mode, while another mode can allow Claude to make changes and run commands.

---

## 🤔 Why is it Needed?

Modes help you control **how much Claude can do automatically**.

You can choose a safer mode when you want to review everything yourself, or a more automatic mode when you trust Claude to perform the task.

---

## 🌊 Simple Flow

```text
You give a task
      ↓
Choose / use a mode
      ↓
Claude follows the mode's permissions
      ↓
Claude performs the task
      ↓
You review the result
```

---

## 💻 Example

Suppose you ask:

```text
Add authentication to my API.
```

Depending on the mode, Claude may:

```text
Mode A
→ Suggest what files should change
→ Wait for your approval

Mode B
→ Make the code changes
→ Run tests
→ Show you the result
```

The exact available modes and permissions can vary by Claude Code version and configuration.

---

## 🔑 Important Idea

**Mode = How much freedom Claude has while working.**

Think:

```text
More restrictions
      ↓
More control / safety

More permissions
      ↓
More automation
```

---

## 🎯 Simple Understanding

> **Modes control what Claude Code is allowed to do while working on your project.**
