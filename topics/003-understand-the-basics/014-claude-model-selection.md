# Model Selection: Opus, Sonnet, Haiku

## 📖 Simple English Explanation
**Model selection** means picking *which* Claude model answers your request.
Every model has a fixed set of trained weights — its "knowledge and skill level" — and that doesn't change no matter what you type.
```text
You send a prompt
    ↓
Pick a model (Haiku / Sonnet / Opus / Fable)
    ↓
That model's fixed weights process your request
    ↓
Answer comes back
```
Model choice is separate from **effort level** (low/medium/high/xhigh/max), which controls *how much work* the model does — files read, verification, steps taken — not how smart it is.

---

## 🤔 Why is it Needed?
Not every task deserves the same model.
```text
Simple lookup / formatting  → doesn't need a big model
Everyday coding / writing   → needs a solid all-rounder
Hard, ambiguous, novel bug  → needs the most capable model
```
Using the biggest model for everything wastes money and time. Using the smallest model for everything means it struggles on hard problems no matter how long you let it try.

---

## 🌊 Simple Flow
```text
                Incoming Task
                     ↓
              How hard / routine is it?
                     ↓
     ┌───────────────┼───────────────┐
     ↓                ↓               ↓
   Haiku           Sonnet           Opus
 (fast, cheap,   (daily driver,   (hardest problems,
  simple tasks)   most tasks)     deep reasoning)
     ↓                ↓               ↓
     └────────────────┼───────────────┘
                     ↓
                 Result returned
```

---

## 💻 Example
Suppose you're working on a coding project and ask:
```text
Fix this typo, refactor this messy auth module,
and figure out why this intermittent race condition
only shows up in production.
```
Instead of running everything on one model:
```text
Task
   ↓
┌────────────┬──────────────────┬───────────────────────┐
↓            ↓                  ↓
Fix typo    Refactor module    Diagnose race condition
Haiku       Sonnet             Opus (or Fable)
↓            ↓                  ↓
└────────────┴──────────────────┴───────────────────────┘
                     ↓
                Combined Result
```

---

## 🔑 Model vs Effort Level
These are two *different* dials, often confused.
```text
Model
  ↓
WHICH weights answer you (capability ceiling)
Effort
  ↓
HOW HARD those weights work this turn (thinking, tool calls, verification)
```
A small model at high effort still can't "know" what it was never trained on. A large model at low effort still "knows" more, it just won't dig as deep. Most real tasks benefit from tuning *both*.

---

## 🎯 The Three (Four) Models

> **Haiku = the speed runner.** Fast, cheap, best for simple, well-defined, repetitive work.

> **Sonnet = the daily driver.** A strong generalist — the right default for most everyday coding, writing, and multi-step tasks.

> **Opus = the expert.** The most capable "standard" model — reach for it on genuinely hard, ambiguous, or high-stakes problems (tricky bugs, architecture decisions, unfamiliar domains).

> **Fable = the specialist** *(where available)*. Suited to the hardest, longest-running, most ambiguous tasks — it sustains long autonomous sessions and can finish jobs the others can't, at any effort level, but costs the most.

```text
Haiku  ──────  Sonnet  ──────  Opus  ──────  Fable
cheap, fast    daily driver    hardest        longest & most
                                problems       ambiguous work
```

---

## 🧭 Practical Guidance

| Use this model | When the task looks like... |
|---|---|
| **Haiku** | Quick lookups, simple edits, formatting, well-specified mechanical changes |
| **Sonnet** | Most day-to-day coding, writing, documentation, reviews — the default for ~90% of work |
| **Opus** | Subtle bugs, architecture decisions, unfamiliar domains, ambiguous problems where a smaller model is "confidently wrong" |
| **Fable** *(if available to you)* | Long, multi-step, highly ambiguous work that needs sustained investigation across a whole session |

**Rule of thumb for diagnosing a bad answer:**
```text
Claude had full context, clearly tried, and still got it wrong
    ↓
→ Pick a BIGGER MODEL (it didn't know enough)

Claude skipped a file, didn't run tests, or bailed early
    ↓
→ Raise the EFFORT LEVEL (it didn't try hard enough)
```

Start with each model's **default effort level** and only adjust as a general preference for your kind of work — not task by task.

---

## 🎯 Simple Understanding
> **Model = how capable the worker is. Effort = how hard that worker works on this particular task.**
Think:
```text
Haiku  = a fast junior who's great at clear, small jobs
Sonnet = a strong all-around teammate you hand most work to
Opus   = the expert you call in for the genuinely hard stuff
Fable  = the specialist you save for the longest, gnarliest problems
```
Pick the smallest model that can reliably do the job — and only go bigger when the task itself, not just more time, is what's missing.

*(For exact current model names, aliases, and how to switch with `/model` in Claude Code, see code.claude.com/docs/en/model-config — model lineups and default versions do shift over time.)*