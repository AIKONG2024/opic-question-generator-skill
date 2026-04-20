---
name: opic-question-generator
description: Use when the user wants realistic OPIc mock questions, survey-based combo sets, answer correction, natural expression rewrites, or level-styled examples such as IM, IH, and AL. Generates question sets using public OPIc structure, and can also correct user answers and rewrite them into clearer and more natural OPIc-style versions.
---

# OPIc Question Generator

Use this skill when the user asks for:

- OPIc mock test questions
- survey-based OPIc question bundles
- realistic 5-5 or 6-6 style OPIc practice
- role-play question generation
- 14-15 style hard follow-up questions
- question typing such as Description, Habit, Past Experience, Comparison, Role Play, or IHU-style follow-up
- correction of OPIc answers
- more natural OPIc phrasing
- level-styled rewrites for IM, IH, and AL
- difficulty-specific mock generation across 1-2, 3-4, and 5-6 bands

## Core Rules

1. Do not claim to know the exact live OPIc question bank.
2. Separate official public information from prediction or reconstruction.
3. Prefer realistic OPIc-style wording over overly simple prompts.
4. Build question sets around survey topics in bundles of three when possible.
5. For higher difficulty mocks, place role-play late and place harder follow-up questions at the end.

## Public Structure to Follow

Officially public:

- Background Survey
- Self Assessment
- 1st Session about 7 questions
- Difficulty adjustment
- 2nd Session about 5 to 8 questions
- Total about 12 to 15 questions

Public prep pattern often used for 5-5 and 6-6 mocks:

- Q1 self-introduction
- Q2 to Q4 combo set 1
- Q5 to Q7 combo set 2
- Q8 to Q10 combo set 3
- Q11 to Q13 role-play block
- Q14 to Q15 hard follow-up block

Treat this numbering pattern as a public test-prep convention, not an official fixed rule.

## Difficulty Model

This skill should treat difficulty in two layers.

### 1. Primary control: `difficulty_band`

Use one of:

- `1-2`
- `3-4`
- `5-6`

This is the main generation control.

### 2. Secondary preference: `difficulty_detail`

Use one of:

- `1-1`, `1-2`, `2-1`, `2-2`
- `3-3`, `3-4`, `4-3`, `4-4`
- `5-5`, `5-6`, `6-5`, `6-6`

Use this only as a fine adjustment, not as a completely different question engine.

## Difficulty Band Behavior

### `1-2`

Use a simpler question profile:

- fewer questions if the user wants realistic low-difficulty simulation
- more Description and Habit
- little or no Past Experience emphasis
- simpler role-play
- no advanced late follow-up block

### `3-4`

Use a standard mid profile:

- 15-question mock is acceptable
- combo sets should include Description, Habit, and Past Experience or Comparison
- role-play should be included
- late questions can be harder, but should not be too abstract

### `5-6`

Use a high-difficulty profile:

- full combo structure
- role-play late in the test
- hard Q14 and Q15 style follow-up prompts
- stronger Comparison, change, issue, or problem-handling prompts
- more Past Experience pressure than lower bands

## Main Question Types

Use these labels when helpful:

- `Description`
- `Habit`
- `Past Experience`
- `Comparison`
- `Role Play`
- `Hard Follow-up`

## How to Build a Combo Set

A realistic combo set usually follows one of these shapes:

### Combo Shape A

1. Description
2. Habit
3. Past Experience

### Combo Shape B

1. Habit
2. Past Experience
3. Comparison

### Combo Shape C

1. Description
2. Habit
3. Harder follow-up

## Role-Play Pattern

When generating role-play questions, use this order:

1. Ask questions to make a plan
2. Ask more detailed follow-up questions
3. Explain a problem and suggest alternatives

The prompt should sound like:

- `I'd like to give you a situation and ask you to act it out.`
- `Call your friend and ask three or four questions ...`
- `Explain the situation and suggest two or three alternatives.`

## Hard Follow-Up Pattern

The final questions should sound harder than normal routine questions.

Good late-question patterns:

- compare past and present
- describe a memorable, unusual, or disappointing experience
- explain what changed and why
- explain how a problem was handled

## Wording Style

Prefer question wording like:

- `You indicated in the survey that ...`
- `Tell me about ...`
- `What is it like?`
- `Why do you like it?`
- `Tell me in detail.`
- `What happened?`
- `What did you like about it?`
- `Please give me as many details as possible.`

Avoid reducing every prompt to one short sentence unless the user explicitly asks for simplified prompts.

## Survey Topics

Common public survey topic families include:

- Housing
- Family / Friend / Neighbors
- Cafe
- SNS / video apps
- Movies
- Game
- Technology
- Item Purchase
- Travel / vacation
- Cancelling Appointment

If the user provides a survey profile, build question sets from that profile first.

## Difficulty Guidance

### For `1-2`

- keep prompts short and direct
- avoid requiring long past-experience storytelling
- prefer simple description and routine prompts
- keep role-play practical and short

### For `3-4`

- keep questions realistic, but not too abstract
- make combo 3 and role-play slightly harder
- use one hard comparison or memorable-experience question at the end

### For `5-6`

- use full combo structure
- make role-play block explicit
- make Q14 and Q15 clearly harder than regular habit questions
- include comparison, change, or problem-handling prompts

## Output Formats

Choose based on the user request:

- single question
- 3-question combo for one survey topic
- full 15-question mock test
- only role-play block
- only hard follow-up block
- question list with type labels
- answer correction only
- answer correction plus natural rewrite
- answer correction plus IM/IH/AL-style rewrites

## Answer Correction Mode

When the user provides an English answer and wants correction, use this workflow.

### Step 1

Identify the likely question type if possible:

- Self-Introduction
- Description
- Habit
- Past Experience
- Comparison
- Role Play
- Hard Follow-up

If the original question is known, use it. If not, infer it from the answer.

### Step 2

Provide a short diagnosis:

- what the answer is trying to say
- what sounds unclear, unnatural, repetitive, or overly direct

### Step 3

Provide a corrected base version.

This version should:

- preserve the user's meaning
- fix major grammar and wording
- stay easy enough to say aloud

### Step 4

Provide a more natural version.

This version should:

- sound smoother and more connected
- still be realistic for spoken OPIc
- avoid overly academic wording unless the user wants high-level phrasing

### Step 5

If requested, provide three style levels:

- `IM version`
- `IH version`
- `AL version`

Use these principles:

- `IM`: simple, direct, easy to say, lower sentence complexity
- `IH`: more connected, clearer reasons, stronger detail, better flow
- `AL`: more polished, controlled, specific, and nuanced while still sounding spoken

Do not present these as official scoring guarantees. Present them as style targets.

## Natural Expression Guidance

When the user asks "how do I say this naturally," prefer this format:

1. simplest version
2. natural spoken version
3. higher-level spoken version if helpful

Keep the phrasing usable in speech. Avoid bookish or overly formal English unless the user clearly wants that.

## Preferred Correction Output

For correction requests, prefer this structure:

- `Meaning`
- `Quick notes`
- `Corrected version`
- `More natural version`
- `IM / IH / AL versions` if requested

Keep the notes short and practical.

## Difficulty Examples

Use examples like these when the user asks for difficulty-specific generation.

### Example: `1-2`

- Tell me about your home.
- What do you usually do at home?
- Tell me about a cafe you like.
- Call your friend and ask a few questions about meeting.

### Example: `3-4`

- Tell me about the place where you live. What is it like?
- What do you usually do at home after work? Tell me in detail.
- Tell me about the last time you stayed home and relaxed.
- Call your friend and ask questions to make a plan.

### Example: `5-6`

- How is your life these days different from your life in the past?
- Tell me about a memorable or unusual experience and how you handled it.
- Explain the situation and suggest two or three alternatives.
- Give me as many details as possible.

## References

If you need the deeper research summary, read:

- [opic_66_research.md](../opic_66_research.md)
