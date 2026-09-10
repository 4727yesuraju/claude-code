# Hooks

## 📖 Simple English Explanation

**Hooks** are automatic actions that Claude Code runs when **specific events happen**.

Instead of manually telling Claude to do something every time, you can configure a hook to do it automatically.

Think of a hook as:

> **"When X happens → automatically do Y."**

---

## 🤔 Why is it Needed?

Hooks help you **automate repetitive tasks** and enforce project rules.

For example:

* Automatically run a formatter after code changes
* Run tests after certain actions
* Check files before Claude uses them
* Block an action that violates a rule
* Run cleanup or logging tasks

---

## 🌊 How It Works

```text
Claude Code performs an action
          ↓
       Event occurs
          ↓
       Hook triggers
          ↓
   Automatic action runs
```

---

## 💻 Example

Suppose you want your JavaScript files to be formatted automatically after Claude edits them.

You can configure a hook like:

```text
When Claude changes a JavaScript file
            ↓
       Hook triggers
            ↓
      Run formatter
            ↓
      Code is formatted
```

So you don't need to manually run the formatter after every change.

---

## 🔑 Common Hook Events

Hooks can be associated with different points in Claude Code's workflow, such as:

```text
Before an action
       ↓
   Action happens
       ↓
After an action
```

For example:

```text
Before tool use → Validate something

After tool use → Run formatter
```

---

## 🎯 Simple Understanding

> **Hooks = Automatic actions triggered by specific events in Claude Code.**

Remember:

```text
Event → Hook → Automatic Action
```

**Skill** teaches Claude *how to perform a task*.

**Hook** automatically *runs something when an event happens*.
