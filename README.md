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

## How People Can Use It

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

## How To Use It With AI Tools

### Codex

Use this repository as a skill source.

- install or copy the skill folder
- let Codex read `SKILL.md`
- ask in plain language

### Claude Code

Use this repository as an instruction source.

Practical method:

- copy the skill folder into your local workflow area, or
- give Claude Code the repository and ask it to follow `SKILL.md`

Then use normal requests such as:

```text
Generate OPIc practice questions for movies and cafes.
```

### ChatGPT

ChatGPT does not normally read `SKILL.md` as a native skill file.

Practical method:

- open this repository
- copy the important rules from `SKILL.md`
- place them into your custom instructions or project instructions
- then chat normally

### Gemini

Gemini also usually works better with copied instructions than with raw skill files.

Practical method:

- use this repository as a reference
- copy the core rules into your working instructions
- then ask in plain language

## Files

- `SKILL.md`: main behavior rules
- `agents/openai.yaml`: metadata
- `README.md`: English guide
- `README.ko.md`: Korean guide

## Notes

- This is for **OPIc English only**
- This is an unofficial practice tool
- It does not provide official live test questions

