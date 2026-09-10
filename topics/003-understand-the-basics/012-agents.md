# Agents

## 📖 Simple English Explanation

An **Agent** is a Claude Code instance that can work on a **specific task or role**.

Instead of asking one Claude session to handle everything, you can give a specialized agent a particular responsibility.

For example:

```text
Main Claude
    ↓
Assigns task
    ↓
Specialized Agent
    ↓
Works on the task
    ↓
Returns result
```

---

## 🤔 Why is it Needed?

Agents are useful when a task is **large, specialized, or easier to separate into smaller tasks**.

For example, you could have:

* **Code Review Agent** → reviews code
* **Testing Agent** → writes/runs tests
* **Research Agent** → researches something
* **Debugging Agent** → investigates errors

This helps organize complex work.

---

## 🌊 How It Works

```text
Main Task
    ↓
Break into smaller tasks
    ↓
┌──────────────┬──────────────┐
↓              ↓              ↓
Agent 1       Agent 2        Agent 3
Code Review   Testing        Research
↓              ↓              ↓
Results       Results        Results
       \        |        /
        \       |       /
          Main Claude
              ↓
         Final Result
```

---

## 💻 Example

Suppose you ask:

```text
Review the authentication feature,
find security issues,
and add tests.
```

The work could be separated into:

```text
Main Claude
    ↓
┌───────────────┬────────────────┐
↓               ↓
Security Agent  Testing Agent
↓               ↓
Find issues     Create tests
└───────┬───────┘
        ↓
   Final result
```

Each agent focuses on its own responsibility.

---

## 🔑 Agent vs Skill vs Hook

These three are easy to confuse:

| Feature   | Purpose                                           |
| --------- | ------------------------------------------------- |
| **Skill** | Teaches Claude how to perform a specific task     |
| **Agent** | Gives Claude a specialized role to work on a task |
| **Hook**  | Automatically runs an action when an event occurs |

Simple example:

```text
Skill → "How should I do this task?"

Agent → "Who/which Claude should handle this task?"

Hook → "When should this action happen automatically?"
```

---

## 🎯 Simple Understanding

> **Agent = A specialized Claude that works on a particular task or role.**

Think:

```text
Main Claude
     ↓
Specialized Agent
     ↓
Specific Task
     ↓
Result
```
