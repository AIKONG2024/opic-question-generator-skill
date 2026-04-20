# OPIc Question Generator Skill

English | [한국어](README.ko.md)

![OPIc Question Generator](assets/cover.png)

## What This Is

This repository contains a simple skill for **OPIc English** practice.

It helps an AI agent do three things:

- make OPIc-style practice questions
- correct spoken answers
- rewrite answers in more natural English

## Why It Is Useful

- you can use it in plain language
- you do not need a strict command format
- it works for question practice, correction, and coaching
- it can be reused across different AI tools

## Quick Start

Just ask naturally.

Examples:

```text
Make a 15-question OPIc mock test.
```

```text
Correct my answer and make it sound more natural.
```

```text
Rewrite this answer in IM, IH, and AL styles.
```

You can give extra details if you want, but you do not need to.

## Setup

### If your AI tool supports skills

1. install or copy this skill folder
2. make sure the tool can read `SKILL.md`
3. start asking in plain language

### If your AI tool does not support skills natively

1. open `SKILL.md`
2. copy the core rules into your instructions or project prompt
3. ask in plain language

If you are not sure how to start, use one of these:

### 1. Random practice

```text
Give me a random OPIc English question.
```

```text
Make a random 15-question OPIc mock test.
```

### 2. Practice with your survey topics

```text
My survey topics are movies, YouTube, cafes, and technology.
Make a 15-question OPIc mock test.
```

```text
Use movies and cafes only.
Make a 3-question combo.
```

### 3. Fix what I already wrote

```text
Here is my answer. Correct it and make it sound more natural.
```

### 4. Ask for coaching

```text
Coach me like an OPIc practice partner.
Give me one question at a time and correct my answer.
```

### 5. Ask for easier or higher-level versions

```text
Rewrite this answer in IM, IH, and AL styles.
```

```text
Rewrite this answer in easier spoken English.
```

## Compatibility

Best used with skill-compatible agents such as:

- Codex
- Claude Code

It can also be adapted to tools like:

- ChatGPT
- Gemini

For tools without native skill support, reuse the rules in `SKILL.md` as instructions.

## Files

- `SKILL.md`: main behavior rules
- `agents/openai.yaml`: metadata
- `README.md`: English guide
- `README.ko.md`: Korean guide

## Notes

- This is for **OPIc English only**
- This is an unofficial practice tool
- It does not provide official live test questions
