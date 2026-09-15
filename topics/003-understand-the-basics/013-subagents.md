# Subagents

## 📖 Simple English Explanation

**Subagents** are separate Claude Code agents that are created by a main Claude Code session to handle **specific tasks**.

Instead of making the main Claude handle everything, it can delegate a task to a subagent.

```text
Main Claude
    ↓
Creates / delegates to Subagent
    ↓
Subagent works on specific task
    ↓
Result comes back to Main Claude
```

---

## 🤔 Why is it Needed?

Subagents are useful when a task can be **split into smaller independent tasks**.

For example, instead of asking one Claude to:

```text
Review code
Write tests
Research a library
```

you can delegate:

```text
Main Claude
   ├──→ Code Review Subagent
   ├──→ Testing Subagent
   └──→ Research Subagent
```

This keeps each task focused.

---

## 🌊 Simple Flow

```text
                 Main Claude
                     ↓
              Breaks the task
                     ↓
        ┌────────────┼────────────┐
        ↓            ↓            ↓
   Subagent 1   Subagent 2   Subagent 3
   Code Review    Testing      Research
        ↓            ↓            ↓
        └────────────┼────────────┘
                     ↓
                Main Claude
                     ↓
                Final Result
```

---

## 💻 Example

Suppose you have a MERN application and ask:

```text
Review the application and improve it.
```

The main Claude can delegate different tasks:

```text
Main Claude
     ↓
┌──────────────┬──────────────┬──────────────┐
↓              ↓              ↓
Backend        Frontend       Testing
Subagent       Subagent       Subagent
↓              ↓              ↓
Review API     Review UI      Check tests
└──────────────┴──────────────┴──────────────┘
                     ↓
                Main Claude
```

The main Claude can then use those results to complete the larger task.

---

## 🔑 Agent vs Subagent

These terms are closely related.

**Agent** is the general concept of an AI worker with a particular role.

**Subagent** specifically means an agent that works as a **helper/delegate under another agent or main Claude session**.

```text
Agent
  ↓
General concept

Subagent
  ↓
Agent working under a main agent
```

---

## 🎯 Simple Understanding

> **Subagent = A separate Claude worker that the main Claude delegates a specific task to.**

Think:

```text
Main Claude = Manager
Subagents   = Team members
```

The manager gives each team member a focused task, receives the results, and uses them to complete the overall work.
