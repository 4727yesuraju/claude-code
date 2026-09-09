# Tools

## 📖 Simple English Explanation

**Tools** are the actions Claude Code can use to work with your project.

Claude itself generates the answer, but **tools allow Claude to actually do things** such as read files, search code, edit files, and run commands.

Think of tools as **Claude's hands** for working with your computer.

---

## 🤔 Why is it Needed?

Without tools, Claude could only give you suggestions.

With tools, Claude can actually interact with your project.

For example, Claude can:

* Read your files
* Search your code
* Create files
* Edit files
* Run commands
* Run tests
* Check the results

---

## 🌊 How It Works

```text
You
 ↓
Give Claude a task
 ↓
Claude decides which tool is needed
 ↓
Tool performs the action
 ↓
Claude sees the result
 ↓
Claude continues the task
```

---

## 💻 Example

You ask:

```text
Find the bug in the customer API and fix it.
```

Claude may do something like:

```text
Read relevant files
      ↓
Search customer API code
      ↓
Find the problem
      ↓
Edit the file
      ↓
Run tests
      ↓
Check the result
```

Claude uses different tools to perform these steps.

---

## 🔑 Common Types of Tools

### 📖 Read

Used to read files and understand code.

```text
Read → Understand the code
```

### 🔍 Search

Used to find files, functions, variables, or text.

```text
Search → Find relevant code
```

### ✏️ Edit

Used to modify existing files.

```text
Edit → Change the code
```

### ➕ Create

Used to create new files.

```text
Create → Add new code/files
```

### ▶️ Run

Used to execute commands, tests, or scripts.

```text
Run → Check / execute something
```

---

## 🎯 Simple Understanding

> **Tools = Actions Claude Code can use to interact with your project.**

Think:

```text
Claude = Brain 🧠
Tools  = Hands 🛠️
Project = Where Claude works
```

Claude uses its **reasoning + tools** to complete coding tasks.
