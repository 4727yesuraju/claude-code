# Claude Code Command Cheatsheet

Simple explanation of each command shown in the cheatsheet image.

## 1. Keyboard Shortcuts

| Shortcut | What it does |
|---|---|
| `Ctrl+C` | Cancel the current action or exit |
| `Ctrl+R` | Search through your command history |
| `Esc` | Stop Claude while it is responding |
| `Esc + Esc` (double tap) | Open the rewind menu — go back to an earlier point in the session |
| `Shift+Tab` | Switch permission mode (e.g. normal → auto-accept edits → plan mode) |

## 2. Slash Commands & Prefixes

| Symbol | Meaning |
|---|---|
| `/` | Start a slash command (e.g. `/help`, `/clear`) |
| `!` | Run a shell command directly (e.g. `!npm test`) |
| `\` | Line break — continue typing on a new line without submitting |
| `@` | Reference a file or folder (e.g. `@src/app.js`) |

## 3. `claude` CLI Commands (used in your terminal, not inside a session)

| Command | What it does |
|---|---|
| `claude` | Start a new Claude Code session in the current folder |
| `claude -r` | Resume/reopen a previous session |
| `claude "query"` | Start a session and immediately send it a question |
| `claude -p` | "Print mode" — get one answer and exit, no interactive session |
| `claude -c` | Continue your most recent conversation |
| `claude --add-dir` | Give Claude access to an extra folder outside the current one |

## 4. Session Commands (used inside a running session)

| Command | What it does |
|---|---|
| `/help` | Show a list of all available commands |
| `/usage` | Show your plan's usage limits and rate-limit status |
| `/clear` | Erase the current conversation and start fresh |
| `/cost` | Show how many tokens/money this session has used |
| `/exit` | Close the session |
| `/export` | Save the conversation to a file |
| `/status` | Show version, model, account, and connection info |
| `/rewind` | Go back to an earlier point in the conversation or code |
| `/plan` | Turn on "plan mode" — Claude explains its plan before making changes |
| `/doctor` | Check if Claude Code is installed and set up correctly |

## 5. Context & Memory Commands

| Command | What it does |
|---|---|
| `/context` | Show how full your context window (conversation memory) is |
| `/compact` | Summarize the conversation so far to free up space |
| `/init` | Create a `CLAUDE.md` file that gives Claude info about your project |
| `/memory` | View or edit Claude's saved project memory (`CLAUDE.md`) |

## 6. Configuration Commands

| Command | What it does |
|---|---|
| `/config` | Open general settings |
| `/permissions` | Control what Claude is allowed to do without asking first |
| `/model` | Switch between models (e.g. Sonnet, Opus, Haiku) |
| `/agents` | Manage subagents (helper agents for specific tasks) |
| `/hooks` | Set up automation that runs at certain points in a session |
| `/mcp` | Manage MCP connections (external tools/services Claude can use) |

## 7. Hooks (automation triggers, set up in configuration)

| Hook | Runs when... |
|---|---|
| `SessionStart` | A new session begins |
| `SessionEnd` | A session ends |
| `PreToolUse` | Right before Claude uses a tool |
| `PostToolUse` | Right after Claude uses a tool |
| `UserPromptSubmit` | You send a message |
| `Stop` | Claude finishes responding |