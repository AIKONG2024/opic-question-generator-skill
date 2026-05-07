# OPIcU(오피쿠)

![OPIc Question Generator](assets/cover.png)

> 한국인을 위한 **OPIc 영어 모의고사 코치** — Background Survey → 15문항 → 한국어 피드백 → 한 문장씩 재연습.
> ChatGPT · Claude · Gemini 어디서나 **10초 안에 시작**합니다.

[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-compatible-brightgreen?style=flat-square)](https://agentskills.io)

---

## ⚡ 10초 만에 시작 — 이 한 줄을 복사해서 챗봇에 붙여넣으세요

ChatGPT, Claude, Gemini 어디든 새 채팅에 **이것만 붙여넣고 Enter**:

```
다음 URL의 SKILL.md 내용을 그대로 따라서, 너는 지금부터 OPIc 모의고사 코치로 동작해줘. 준비되면 한국어로 "오픽 모의고사 시작할까요?"라고 물어봐.

https://raw.githubusercontent.com/AIKONG2024/opicu/main/SKILL.md
```

AI가 알아서 위 URL을 읽고 OPIc 코치로 변신합니다. **터미널, 설치, 폴더 같은 건 전혀 필요 없습니다.**

> 모바일 ChatGPT 앱 사용자라면 [👉 이 링크](https://chatgpt.com/?q=%EB%8B%A4%EC%9D%8C%20URL%EC%9D%98%20SKILL.md%20%EB%82%B4%EC%9A%A9%EC%9D%84%20%EA%B7%B8%EB%8C%80%EB%A1%9C%20%EB%94%B0%EB%9D%BC%EC%84%9C%2C%20%EB%84%88%EB%8A%94%20%EC%A7%80%EA%B8%88%EB%B6%80%ED%84%B0%20OPIc%20%EB%AA%A8%EC%9D%98%EA%B3%A0%EC%82%AC%20%EC%BD%94%EC%B9%98%EB%A1%9C%20%EB%8F%99%EC%9E%91%ED%95%B4%EC%A4%98.%20%EC%A4%80%EB%B9%84%EB%90%98%EB%A9%B4%20%ED%95%9C%EA%B5%AD%EC%96%B4%EB%A1%9C%20%22%EC%98%A4%ED%94%BD%20%EB%AA%A8%EC%9D%98%EA%B3%A0%EC%82%AC%20%EC%8B%9C%EC%9E%91%ED%95%A0%EA%B9%8C%EC%9A%94%3F%22%EB%9D%BC%EA%B3%A0%20%EB%AC%BC%EC%96%B4%EB%B4%90.%0A%0Ahttps%3A%2F%2Fraw.githubusercontent.com%2FAIKONG2024%2Fopicu%2Fmain%2FSKILL.md)을 누르면 미리 작성된 프롬프트로 ChatGPT가 열립니다. Enter만 누르세요.

준비되면 그냥 말하면 됩니다:

```
오픽 모의고사 시작해줘. 난이도 5-6.
```

---

## 매일 쓰고 싶다면 — Project / Gem에 등록 (1분, 한 번만)

매번 위 한 줄을 붙여넣는 게 귀찮다면 본인 챗봇에 "전용 봇"으로 만들어 두세요. 한 번 만들면 영원히 그 안에서 OPIc 모드로 동작합니다.

### ChatGPT (Projects)
1. ChatGPT 좌측 메뉴 → **Projects → New Project**
2. 이름: `OPIc 모의고사`
3. **Instructions**에 위의 "마법의 한 줄"을 그대로 붙여넣기
4. 저장 후 그 Project 안에서 채팅 시작

### Claude (Projects)
1. Claude 좌측 메뉴 → **Projects → Create Project**
2. **Project instructions**에 위의 "마법의 한 줄" 붙여넣기 (Claude는 URL을 알아서 읽습니다)
3. 저장 후 사용

### Gemini (Gems)
1. Gemini → **Gems → New Gem**
2. **Instructions**에 위의 "마법의 한 줄" 붙여넣기
3. 저장 후 그 Gem과 대화

> 💡 **음성 연습:** 위 방식으로 만든 Project/Gem을 ChatGPT Voice 또는 Gemini Live에서 그대로 열면 음성으로 OPIc 연습이 됩니다. 별도 설정 없습니다.

---

## 자주 쓰는 명령어

| 입력 | 동작 |
|---|---|
| `오픽 모의고사 시작해줘` | 모의고사 시작 (난이도 묻기) |
| `난이도 5-6으로 시작해줘` | 난이도 지정해서 바로 시작 |
| `next` | 다음 문제로 넘어가기 |
| `question again` | 같은 문제 다시 듣기 |
| `이 답변을 한 문장씩 연습하자` | 마지막 답변을 문장 단위로 교정 |
| `피드백 짧게 해줘` | 짧은 교정만 받기 (Voice 모드 추천) |
| `목표는 IH야` / `목표는 IM3야` | 목표 등급에 맞춰 답변 난이도 조정 |

---

## 핵심 기능

- 난이도 선택: `3-4`, `5-6`
- 실제 시험형 Background Survey 자동 출력
- Q1–Q15 모의고사 (롤플레이 Q11–Q13, 고난도 비교/이슈/의견 Q14–Q15 포함)
- 한국어 피드백 + 모범 답변 + 표현 교정
- "next"라고 말하기 전까지 다음 문제로 넘어가지 않음
- 한 문장씩 끊어서 말하기 연습 모드

---

## 개발자용 — Agent Skill 표준 설치

Claude Code, Codex CLI, Cursor, Gemini CLI를 쓰는 개발자라면 이 레포를 표준 Agent Skill로 설치할 수 있습니다.

```bash
# 자동 설치 (Vercel skills CLI)
npx skills add AIKONG2024/opicu

# 수동 설치 — Claude Code 예시
git clone https://github.com/AIKONG2024/opicu.git
cp -r opicu ~/.claude/skills/
```

도구별 설치 경로:

| 도구 | 경로 |
|---|---|
| Claude Code | `~/.claude/skills/` (전역) 또는 `.claude/skills/` (프로젝트) |
| Codex CLI | `~/.codex/skills/` |
| Cursor | `.cursor/skills/` |
| Gemini CLI | `.gemini/skills/` |

새 세션을 시작하면 자동으로 활성화됩니다. "오픽 모의고사 시작해줘"라고 입력하면 됩니다.

---

## 이게 왜 잘 되나요?

이 Skill은 **두 가지 표준**을 동시에 만족하도록 만들어졌습니다:

1. **Agent Skills 표준** — `SKILL.md` 파일이 YAML frontmatter를 갖춘 정식 Skill 포맷이라, Claude Code/Codex/Cursor 등에서 자동 인식됩니다.
2. **AI-readable README** — `SKILL.md`가 GitHub raw URL로 직접 접근 가능해서, ChatGPT/Claude/Gemini가 URL 한 줄로 읽고 자기 자신을 설정할 수 있습니다.

덕분에 일반 사용자는 "복붙 한 번"만, 개발자는 "표준 설치"를 선택할 수 있습니다.

---

## 주의사항

- 공식 OPIc 시험을 대체하지 않습니다. AI 생성 질문/피드백은 실제 시험과 완전히 같지는 않습니다.
- 음성 인식은 종종 틀립니다. 중요한 답변은 텍스트로도 확인하세요.
- 이 레포 외부의 출처 불분명한 SKILL.md는 신중히 검토 후 사용하세요.

---

## License

MIT — 학습/공개용으로 자유롭게 수정해서 사용하세요.
