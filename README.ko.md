# OPIc Question Generator Skill

[English](README.md) | [한국어](README.ko.md)

![OPIc Question Generator](assets/cover.png)

> **An AI agent skill for OPIc English practice — question generation, answer correction, and level coaching, all in plain language.**

[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)
[![Works with Claude Code](https://img.shields.io/badge/works%20with-Claude%20Code-blueviolet?style=flat-square)](https://claude.ai/code)
[![Works with Codex](https://img.shields.io/badge/works%20with-Codex-green?style=flat-square)](https://openai.com/codex)
[![OPIc English](https://img.shields.io/badge/OPIc-English%20Only-orange?style=flat-square)](https://www.actfl.org/opic)

---

## What Is This Skill?

This repository contains a **`SKILL.md` file** — a set of instructions that turns any compatible AI agent into a dedicated **OPIc English practice coach**.

Load it once, and your agent gains the following abilities:

| Ability | What it does |
|---|---|
| 📝 **Generate Questions** | Create OPIc-style questions from any topic, or from your actual survey topics |
| 🎯 **Build Mock Tests** | Generate full 15-question mock tests that mirror the real exam format |
| ✏️ **Correct Answers** | Fix grammar, naturalness, and fluency in your spoken-style answers |
| 🔄 **Level Rewriting** | Rewrite the same answer in IM, IH, and AL styles so you can see the difference |
| 🤝 **Interactive Coaching** | Simulate a real practice session — one question at a time, with instant feedback |

No special commands needed. Just talk to your agent naturally.

---

## Usage

### 🎲 Random practice

Warm up with random questions at any time.

```
Give me a random OPIc English question.
```

```
Make a random 15-question OPIc mock test.
```

---

### 📋 Practice with your survey topics

Tell the agent your topics and it will generate questions that match the real exam format.

```
My survey topics are movies, YouTube, cafes, and technology.
Make a 15-question OPIc mock test based on these topics.
```

```
Use only movies and cafes.
Make a 3-question combo (description + routine + past experience).
```

> 💡 **Tip:** In the real OPIc exam, questions often come in a "combo" of 3 — describing something, talking about your routine, and recalling a past experience, all on the same topic. Ask for combo drills to practice this format.

---

### ✏️ Correct your answer

Paste an answer you wrote or said, and ask for corrections.

```
Here is my answer:

"I usually go to cafe on weekend. I like to drink americano and read book.
Last week, I went to new cafe near my house. It was very cozy and quiet."

Correct it and make it sound more natural.
```

---

### 🤝 Interactive coaching session

Ask the agent to coach you one question at a time, just like a real practice partner.

```
Coach me like an OPIc practice partner.
Give me one question at a time, wait for my answer, then correct it and move on.
```

---

### 📈 Level up your answer

See what your answer looks like at different OPIc levels — IM, IH, and AL — so you know exactly what to aim for.

```
Here is my answer. Rewrite it in IM, IH, and AL styles.
```

```
Rewrite this answer in easier spoken English (Intermediate Mid style).
```

---

## Setup

### ✅ Option A — Skill-compatible tools (Claude Code, Codex)

These tools can read `SKILL.md` automatically.

1. Clone this repository:
   ```bash
   git clone https://github.com/AIKONG2024/opic-question-generator-skill.git
   ```
2. Make sure your agent tool can access the `SKILL.md` file in the repository root.
3. Start practicing:
   ```
   Load this skill and help me practice OPIc English.
   ```

---

### 🛠️ Option B — Tools without native skill support (ChatGPT, Gemini, Claude.ai)

1. Open [`SKILL.md`](SKILL.md) in this repository and copy the entire contents.
2. Paste it into your tool's **System Prompt**, **Custom Instructions**, or **Project Instructions** field.
3. Start practicing:
   ```
   Make a random OPIc mock test.
   ```

**Claude.ai:** Go to **Projects** → create a new project → paste `SKILL.md` into **Project Instructions**.  
**ChatGPT:** Go to **Settings → Personalization → Custom Instructions**.

| Tool | Support | Where to paste |
|---|---|---|
| **Claude Code** | ✅ Native | Load from repo |
| **Codex** | ✅ Native | Load from repo |
| **Claude.ai** | Manual | Project Instructions |
| **ChatGPT** | Manual | Custom Instructions |
| **Gemini** | Manual | System Prompt |

---

## Notes

- This skill is for **OPIc English only** — OPIc Korean (OPIc-K) is not supported.
- This is an **unofficial** practice tool, not affiliated with ACTFL or any test provider.
- It does not contain or reproduce official OPIc exam questions.

---

*Good luck on your test! 🎯*
