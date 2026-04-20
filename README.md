# OPIc Question Generator Skill

[한국어 README 보기](README.ko.md)

> Unofficial practice skill for **OPIc English only**

![OPIc Question Generator](assets/cover.png)

## Overview

This skill helps users practice **OPIc English** by generating practice prompts and improving spoken answers.

It can:

- generate OPIc-style practice questions
- build survey-based question bundles
- generate role-play and late hard follow-up questions
- correct user answers
- suggest more natural spoken expressions
- show `IM / IH / AL` style rewrites for practice

It does **not**:

- provide official live test questions
- reproduce proprietary course materials
- guarantee any official OPIc score

## Scope

This skill supports:

- **OPIc English**

This skill does not target:

- OPIc in other languages
- general English conversation beyond OPIc-style practice

## How To Use

### For AI Agents

Use this skill when the user asks for:

- OPIc mock questions
- survey-based practice sets
- answer correction for OPIc speaking
- natural spoken rewrites
- IM / IH / AL style answer examples

Recommended workflow:

1. identify the user's survey topics if provided
2. identify the requested difficulty band if provided
3. choose one output mode
4. generate only what the user asked for

Preferred output modes:

- questions only
- questions + types
- questions + MP
- questions + sample answers
- answer correction
- answer correction + natural rewrite
- answer correction + IM/IH/AL versions

### For Human Users

You can use this skill by asking in plain language.

Examples:

```text
Generate a 15-question OPIc English mock test.
survey_topics: movies, youtube, cafe
difficulty_band: 3-4
language: English
```

```text
Correct my answer and explain what sounds unnatural.
Show a more natural spoken version too.
```

```text
Rewrite my answer in IM, IH, and AL speaking styles.
```

## Input Options

You can provide these options directly in your request.

- `survey_topics`
  Example: `movies, youtube, cafe, technology`
- `difficulty_band`
  Example: `1-2`, `3-4`, `5-6`
- `difficulty_detail`
  Example: `3-3`, `4-4`, `5-5`, `6-6`
- `question_count`
  Example: `1`, `3`, `15`
- `output_mode`
  Example: `questions only`, `questions + MP`, `answer correction`
- `language`
  Example: `Korean`, `English`, `mixed`
- `include_roleplay`
  Example: `yes`, `no`
- `include_hard_followups`
  Example: `yes`, `no`
- `answer_style`
  Example: `corrected only`, `natural rewrite`, `IM/IH/AL`

## Difficulty Model

This skill uses two layers for difficulty.

### 1. `difficulty_band`

Main generation control:

- `1-2`
  simpler prompts, lighter past-experience pressure
- `3-4`
  standard combo structure with role-play
- `5-6`
  harder follow-up questions and stronger comparison / problem handling

### 2. `difficulty_detail`

Fine preference only:

- `1-1`, `1-2`, `2-1`, `2-2`
- `3-3`, `3-4`, `4-3`, `4-4`
- `5-5`, `5-6`, `6-5`, `6-6`

The skill should not treat every detail value as a completely separate engine.

## Main Output Types

### 1. Question Generation

- single prompt
- 3-question combo
- 15-question mock test
- role-play block
- hard follow-up block

### 2. Answer Correction

- correct grammar and wording
- preserve the original meaning
- make the answer easier to say aloud

### 3. Natural Spoken Rewrite

- suggest simpler spoken expressions
- suggest smoother OPIc-style phrasing

### 4. Level-Styled Rewrite

When requested, the skill may show:

- `IM version`
- `IH version`
- `AL version`

These are **practice style examples**, not official scoring guarantees.

## Notes For Public Use

- This is an **unofficial practice skill**.
- It is based on publicly available OPIc structure and common practice patterns.
- It does not claim to reproduce the official live question bank.
- It is intended for practice and coaching only.

## Repository Structure

```text
opic-question-generator/
├── SKILL.md
├── README.md
├── README.ko.md
├── agents/
│   └── openai.yaml
└── assets/
    └── cover.png
```

## Before Publishing

Before uploading to GitHub, confirm:

- the image file is placed at `assets/cover.png`
- the project is described as **OPIc English only**
- no proprietary course text has been copied
- no official live question claim is made

