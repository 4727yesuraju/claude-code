# Claude Code — Usage Best Practices

## 1. 📖 Simple English Explanation

**Usage Best Practices** are simple habits that help you use Claude Code **effectively, safely, and efficiently**.

---

## 2. 🎯 Give Clear Instructions

Give Claude a clear task and explain what you expect.

```text
❌ "Fix this."

✅ "Fix the login API error.
   Check the backend first and explain the cause
   before making changes."
```

> **Clear input → Better output**

---

## 3. 🧩 Break Large Tasks into Smaller Tasks

Instead of giving Claude one huge task, break it into smaller steps.

```text
Large Task
    ↓
1. Setup
    ↓
2. Authentication
    ↓
3. Backend API
    ↓
4. Frontend UI
    ↓
5. Testing
```

This makes complex tasks easier to understand and manage.

---

## 4. 🧠 Use Plan Mode for Complex Tasks

For large or risky tasks, use **Plan Mode** first.

```text
Plan Mode
    ↓
Understand
    ↓
Analyze
    ↓
Create Plan
    ↓
Review
    ↓
Implement
```

> **Think first → Plan → Execute**

---

## 5. 👀 Review Changes

Don't blindly accept every change Claude makes.

```text
Claude changes code
        ↓
Review changes
        ↓
Run tests
        ↓
Check result
```

Make sure the changes actually solve the problem.

---

## 6. 🔄 Use Resume & Rewind

### Resume

Continue a previous session.

> **Resume = Continue where you left off**

### Rewind

Return to an earlier point when something goes wrong.

> **Rewind = Go back and undo later changes**

```text
Good State
    ↓
Changes
    ↓
Something goes wrong ❌
    ↓
Rewind ⏪
```

---

## 7. 🛡️ Use Permissions Carefully

Choose the permission mode based on how much freedom you want to give Claude.

```text
Plan
  ↓
Planning only

Default
  ↓
Ask when permission is needed

Accept Edits
  ↓
Automatically accept file edits

Don't Ask
  ↓
More actions happen automatically
```

For unfamiliar or risky tasks, use more controlled permissions.

---

## 8. 🧪 Test Your Changes

After Claude makes changes:

```text
Code Change
    ↓
Run Tests
    ↓
Check Errors
    ↓
Verify Result
```

Don't assume that code is correct just because Claude generated it.

---

## 9. 🧠 Simple Rule to Remember

```text
Clear Task
    ↓
Break into Steps
    ↓
Plan
    ↓
Implement
    ↓
Review
    ↓
Test
```

> **Clear task → Small steps → Plan → Implement → Review → Test**
