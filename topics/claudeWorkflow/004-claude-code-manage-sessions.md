# Claude Code — Manage Sessions

## 1. 📖 Simple English Explanation

A **Session** is a conversation/work session with Claude Code.

Two useful ways to manage sessions are:

* **Resume** → Continue a previous session
* **Rewind** → Go back to an earlier point in a session

---

## 2. 🔄 Resume

**Resume** means:

> Continue a previous Claude Code session from where you stopped.

### Example

```text
Monday
  ↓
You ask Claude to build a login feature
  ↓
Claude works on it
  ↓
You stop
  ↓
Tuesday
  ↓
Resume the session
  ↓
Continue from the previous session
```

### 🧠 Remember

> **Resume = Continue where you left off**

---

## 3. ⏪ Rewind

**Rewind** means:

> Go back to an earlier point in the session and undo changes made after that point.

### Example

```text
Start
  ↓
A → File A changed
  ↓
B → File B changed
  ↓
C → File C changed
  ↓
Something went wrong ❌
```

You can choose an earlier point to rewind to.

### Rewind to A

```text
Start
  ↓
A → File A changed ✅
```

Changes made after A are undone:

```text
A → Keep ✅
B → Undo ❌
C → Undo ❌
```

### Rewind to B

```text
A → Keep ✅
B → Keep ✅
C → Undo ❌
```

### Rewind to C

```text
A → Keep ✅
B → Keep ✅
C → Keep ✅
```

---

## 4. 🔄 Resume vs ⏪ Rewind

| Feature    | Meaning                     |
| ---------- | --------------------------- |
| **Resume** | Continue an old session     |
| **Rewind** | Go back to an earlier point |
| **Resume** | "Continue from here"        |
| **Rewind** | "Take me back to there"     |

---

## 5. 🌊 Simple Flow

```text
                    Claude Code Session
                           ↓
              ┌────────────┴────────────┐
              ↓                         ↓
           Resume                    Rewind
              ↓                         ↓
     Continue previous         Go to earlier point
          session                     ↓
                                Undo later changes
```

---

## 6. 🧠 Remember

```text
RESUME  → Continue ▶️

REWIND  → Go back ⏪
```

> **Resume = Continue**

> **Rewind = Go back to an earlier point and undo later changes**
