# Using Claude Code

## 📖 Simple English Explanation

Once Claude Code is installed, you mainly interact with it by **giving prompts and using keyboard shortcuts/commands**.

These shortcuts help you control Claude Code quickly without typing everything manually.

The main things to understand are:

* Keyboard shortcuts
* Slash commands `/`
* `!` for shell commands
* `@` for adding file/folder context
* `\` for escaping / multiline input

---

## 🌊 Basic Flow

```text
Start Claude Code
       ↓
Give a prompt
       ↓
Claude understands the task
       ↓
Claude uses tools
       ↓
You review the result
       ↓
Continue / modify / stop
```

---

# ⌨️ Keyboard Shortcuts

## `Ctrl + C`

**Stop the current operation** or cancel the current input.

```text
Claude is working
      ↓
Ctrl + C
      ↓
Stop / cancel
```

---

## `Ctrl + R`

**Search through your previous input/history.**

Useful when you want to reuse something you typed earlier instead of typing it again.

---

## `Esc`

**Cancel or interrupt the current action/input.**

Useful when you want to stop what you are currently doing without exiting Claude Code.

---

## `Esc + Esc`

Press **Esc twice** to go back through previous conversation state / undo recent changes in the interaction.

Think:

```text
Esc
 ↓
Interrupt

Esc + Esc
 ↓
Go back / undo recent interaction
```

---

## `Shift + Tab`

Used to **change the permission/interaction mode** while working with Claude Code.

For example, you can switch between modes that control how much Claude can do automatically.

```text
Shift + Tab
     ↓
Change mode
     ↓
Claude's permissions change
```

---

# `/` Slash Commands

Slash commands are **special commands that start with `/`**.

They provide built-in actions or information.

Example:

```text
/help
```

You can use `/` and then explore the available commands.

Think:

```text
/command
   ↓
Claude Code built-in action
```

---

# `!` Shell Commands

`!` lets you run a **shell command directly** from Claude Code.

Example:

```text
! npm test
```

This means:

```text
Claude Code
    ↓
!
    ↓
Run shell command
    ↓
npm test
```

This is useful when you already know the command you want to execute.

---

# `@` Add Context

`@` can be used to **reference files or directories** in your prompt.

For example:

```text
Explain @src/auth.js
```

You are telling Claude:

> "Use this file as context."

This is useful when you want Claude to focus on a particular file or directory.

---

# `\` Multiline Input

The backslash can be used when you need to enter **multiline input**.

For example:

```text
\
Explain this API.

Also check:
- Error handling
- Validation
- Security
```

This is useful when your prompt is longer and you want to structure it across multiple lines.

---

# 💻 Example

Imagine you are working on a MERN project.

You can do:

```text
@src/controllers/userController.js
Explain this file and find possible bugs.
```

Then, if you want to run your tests:

```text
! npm test
```

If Claude starts doing something you don't want:

```text
Esc
```

If you want to change the current mode:

```text
Shift + Tab
```

And for Claude Code's built-in commands:

```text
/help
```

---

## 🎯 Simple Understanding

Think of Claude Code like this:

```text
Keyboard Shortcuts
        ↓
Control Claude Code

/       → Built-in Claude commands
!       → Run shell commands
@       → Add file/folder context
\       → Multiline input
```

The goal is not to memorize every shortcut.

**Understand what each symbol is used for, then practice using it while working on a real project.**
