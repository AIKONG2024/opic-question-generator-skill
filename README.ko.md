# OPIc Question Generator Skill

[English](README.md) | [한국어](README.ko.md)

![OPIc Question Generator](assets/cover.png)

> **AI 에이전트용 OPIc English 연습 Skill — 문제 생성, 답변 교정, 레벨 코칭을 자연어로.**

[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)
[![Works with Claude Code](https://img.shields.io/badge/works%20with-Claude%20Code-blueviolet?style=flat-square)](https://claude.ai/code)
[![Works with Codex](https://img.shields.io/badge/works%20with-Codex-green?style=flat-square)](https://openai.com/codex)
[![OPIc English](https://img.shields.io/badge/OPIc-English%20Only-orange?style=flat-square)](https://www.actfl.org/opic)

---

## 이 Skill이 뭔가요?

이 저장소는 **`SKILL.md` 파일** 하나를 포함하고 있습니다. 이 파일은 호환되는 AI 에이전트를 **OPIc English 전용 연습 코치**로 만들어주는 행동 규칙 모음입니다.

한 번 로드하면, 에이전트가 아래 능력을 갖추게 됩니다:

| 기능 | 설명 |
|---|---|
| 📝 **문제 생성** | 어떤 주제로든 OPIc 스타일 문제 생성 (내 서베이 주제 포함) |
| 🎯 **모의고사 생성** | 실제 시험 형식의 15문항 모의고사 생성 |
| ✏️ **답변 교정** | 문법, 자연스러움, 유창성 교정 |
| 🔄 **레벨별 리라이팅** | 같은 답변을 IM, IH, AL 수준으로 변환해 차이 비교 |
| 🤝 **인터랙티브 코칭** | 문제 1개씩 출제 → 답변 → 즉시 피드백의 실전 연습 |

특별한 명령어 불필요. 그냥 자연스럽게 말하면 됩니다.

---

## 사용법

### 🎲 랜덤 문제 연습

주제 없이 바로 시작하고 싶을 때.

```
오픽 영어 문제 랜덤으로 하나 내줘.
```

```
오픽 모의고사 15문항 랜덤으로 만들어줘.
```

---

### 📋 내 서베이 주제로 연습하기

실제 시험에서 나올 주제로 연습하세요.

```
내 서베이 주제는 movies, youtube, cafe, technology야.
이걸로 오픽 모의고사 15문항 만들어줘.
```

```
movies, cafe 주제로만 3문항 콤보 만들어줘.
(묘사 + 루틴 + 과거 경험 형식으로)
```

> 💡 **팁:** 실제 OPIc에서는 같은 주제를 3연속으로 다르게 묻는 **콤보 문제**가 출제됩니다 (묘사 → 루틴 → 과거 경험). 콤보 드릴로 이 패턴을 미리 익혀두세요.

---

### ✏️ 내 답변 교정받기

작성했거나 말한 답변을 붙여넣고 교정을 요청하세요.

```
내 답변이야:

"I usually go to cafe on weekend. I like to drink americano and read book.
Last week, I went to new cafe near my house. It was very cozy and quiet."

교정해주고 더 자연스럽게 바꿔줘.
```

---

### 🤝 인터랙티브 코칭 세션

실제 연습처럼 문제 하나씩 풀고 즉시 피드백 받기.

```
오픽 연습 파트너처럼 진행해줘.
문제 하나씩 내고, 내 답변을 기다렸다가 교정하고 다음 문제로 넘어가줘.
```

---

### 📈 레벨업 리라이팅

내 답변이 IM, IH, AL 수준에서 어떻게 달라지는지 직접 비교해보세요.

```
내 답변이야. IM, IH, AL 스타일로 각각 바꿔줘.
```

```
이 답변을 더 쉬운 spoken English(IM 수준)로 바꿔줘.
```

---

## 설정 방법

### ✅ 방법 A — Skill 지원 도구 (Claude Code, Codex)

이 도구들은 `SKILL.md`를 자동으로 읽습니다.

1. 저장소를 클론합니다:
   ```bash
   git clone https://github.com/AIKONG2024/opic-question-generator-skill.git
   ```
2. 에이전트 도구가 저장소 루트의 `SKILL.md`에 접근할 수 있게 설정합니다.
3. 연습 시작:
   ```
   이 skill을 불러오고 OPIc English 연습을 도와줘.
   ```

---

### 🛠️ 방법 B — Skill을 지원하지 않는 도구 (ChatGPT, Gemini, Claude.ai)

1. 이 저장소에서 [`SKILL.md`](SKILL.md)를 열고 전체 내용을 복사합니다.
2. 사용 중인 도구의 **System Prompt** / **Custom Instructions** / **Project Instructions** 필드에 붙여넣습니다.
3. 연습 시작:
   ```
   오픽 모의고사 랜덤으로 만들어줘.
   ```

**Claude.ai:** **Projects** → 새 프로젝트 생성 → **Project Instructions**에 붙여넣기.  
**ChatGPT:** **설정 → 개인화 → Custom Instructions**에 붙여넣기.

| 도구 | 지원 방식 | 설정 위치 |
|---|---|---|
| **Claude Code** | ✅ 네이티브 | 저장소에서 바로 로드 |
| **Codex** | ✅ 네이티브 | 저장소에서 바로 로드 |
| **Claude.ai** | 수동 | Project Instructions |
| **ChatGPT** | 수동 | Custom Instructions |
| **Gemini** | 수동 | System Prompt |

---

## 참고

- **OPIc English 전용**입니다 — OPIc Korean(한국어)은 지원하지 않습니다.
- **비공식** 연습용 도구로, ACTFL 또는 시험 기관과 무관합니다.
- 공식 OPIc 시험 문제를 포함하거나 재현하지 않습니다.

---

*시험 잘 보세요! 🎯*
