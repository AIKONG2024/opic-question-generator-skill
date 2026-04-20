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
