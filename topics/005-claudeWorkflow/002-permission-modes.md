# Claude Code Permission Modes

## 1. 📖 Simple English Explanation

**Permission Modes** control **what Claude Code can do automatically** and **when Claude needs to ask for your permission**.

Think of them as **different levels of access** given to Claude Code.

---

## 2. 🤔 Why is it Needed?

Permission modes help you control Claude's actions.

For example, Claude may want to:

* Edit a file
* Create a file
* Run a command
* Delete something
* Make other changes

Depending on the mode, Claude may:

* Ask you first
* Do it automatically
* Only create a plan

---

## 3. 🌊 Simple Flow

```text
Claude wants to perform an action
              ↓
       Check Permission Mode
              ↓
    ┌─────────┼─────────┐
    ↓         ↓         ↓
   Ask      Allow     Plan Only
    ↓         ↓         ↓
  User     Execute    Analyze
 decides    action     only
```

---

## 4. 🔐 Common Permission Modes

| Mode             | What Claude can do                                          |
| ---------------- | ----------------------------------------------------------- |
| **Default**      | Asks for permission when an action requires approval        |
| **Plan**         | Analyzes the task and creates a plan without making changes |
| **Accept Edits** | Automatically accepts file edits                            |
| **Don't Ask**    | Automatically performs actions without asking               |

---

## 5. 💻 Example

Suppose you ask:

> "Create a login page."

### Plan Mode

```text
Claude
  ↓
Analyzes the project
  ↓
Creates a plan
  ↓
Waits for you
```

Claude focuses on **planning**, not making changes.

### Accept Edits Mode

```text
Claude
  ↓
Analyzes the project
  ↓
Creates/edits files
  ↓
Continues working
```

Claude can **automatically accept file edits**.

### Default Mode

```text
Claude
  ↓
Analyzes the project
  ↓
Needs permission for certain actions
  ↓
Asks you
  ↓
You approve
  ↓
Claude continues
```

---

## 6. 🧠 Remember

> **Permission Mode = How much freedom Claude Code has to perform actions automatically.**

```text
Plan
  ↓
Think & plan

Default
  ↓
Ask when permission is needed

Accept Edits
  ↓
Automatically accept edits

Don't Ask
  ↓
Automatically perform actions
```
