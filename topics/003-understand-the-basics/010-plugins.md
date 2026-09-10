# Plugins

## 📖 Simple English Explanation

**Plugins** are packages that extend Claude Code with **additional capabilities**.

A plugin can bundle things like:

* Skills
* Commands
* Agents
* Hooks
* MCP servers

So instead of setting up each part separately, a plugin can provide a complete set of functionality.

---

## 🤔 Why is it Needed?

Plugins are useful when you want to **extend Claude Code** for a particular workflow or development need.

For example, a plugin could provide everything needed for:

```text
Code Review
    ↓
Skill + Commands + Agents
    ↓
One Plugin
```

You can then reuse that functionality instead of building everything from scratch.

---

## 🌊 How It Works

```text
Claude Code
     ↓
Install Plugin
     ↓
Plugin adds capabilities
     ↓
Claude Code can use them
```

A plugin can contain multiple components:

```text
Plugin
 ├── Skills
 ├── Commands
 ├── Agents
 ├── Hooks
 └── MCP integrations
```

---

## 💻 Example

Imagine you want Claude Code to follow your team's code-review process.

Instead of creating everything manually, you could use a plugin that provides:

```text
Code Review Plugin
       ↓
   ┌───┼────┐
   ↓   ↓    ↓
 Skill  Command  Agent
       ↓
 Team's review workflow
```

After installing the plugin, Claude Code gets those additional capabilities.

---

## 🔑 Plugin vs Skill vs MCP

These can be confusing, so remember:

| Feature    | Simple meaning                                            |
| ---------- | --------------------------------------------------------- |
| **Skill**  | Instructions for a specific task                          |
| **MCP**    | Connect Claude Code to external tools/services            |
| **Plugin** | A package that can bundle multiple Claude Code extensions |

For example:

```text
Plugin
 ├── Skill → How to perform a task
 ├── MCP   → Connect to an external service
 └── Command → Provide a reusable action
```

---

## 🎯 Simple Understanding

> **Plugin = A package that adds extra capabilities to Claude Code.**

Think:

```text
Claude Code
     +
  Plugins
     ↓
More capabilities
```
