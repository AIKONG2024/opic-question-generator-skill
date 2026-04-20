# OPIc Question Generator Skill

[English](README.md) | 한국어

![OPIc Question Generator](assets/cover.png)

## 이게 뭔가요?

이 저장소는 **OPIc English** 연습용 skill입니다.

AI가 아래 3가지를 하도록 도와줍니다.

- 오픽 스타일 문제 생성
- 답변 교정
- 더 자연한 영어로 다시 써주기

## 왜 좋은가요?

- 자연어로 바로 사용할 수 있습니다
- 복잡한 명령 형식이 필요 없습니다
- 문제 연습, 교정, 코칭에 모두 쓸 수 있습니다
- 여러 AI 도구에서 재사용할 수 있습니다

## 사람은 어떻게 쓰나요?

그냥 자연스럽게 요청하면 됩니다.

예:

```text
오픽 모의고사 15문항 만들어줘.
```

```text
내 답변을 교정해주고 더 자연하게 바꿔줘.
```

```text
이 답변을 IM, IH, AL 느낌으로 바꿔줘.
```

원하면 세부 조건을 더 붙일 수 있지만, 꼭 그럴 필요는 없습니다.

## AI 도구에서 어떻게 쓰나요?

### Codex

이 저장소를 skill source처럼 사용하면 됩니다.

- skill 폴더를 설치하거나 복사
- Codex가 `SKILL.md`를 읽게 함
- 그 다음 자연어로 요청

### Claude Code

이 저장소를 instruction source처럼 사용하면 됩니다.

실용적인 방법:

- skill 폴더를 로컬 작업 영역에 복사하거나
- Claude Code에게 이 저장소를 주고 `SKILL.md`를 따르라고 요청

그 다음 이렇게 사용하면 됩니다.

```text
movies, cafe 주제로 오픽 연습 문제 만들어줘.
```

### ChatGPT

ChatGPT는 보통 `SKILL.md`를 네이티브 skill 파일처럼 직접 읽지는 않습니다.

실용적인 방법:

- 이 저장소를 열고
- `SKILL.md`의 핵심 규칙을 복사해서
- custom instructions 또는 project instructions에 넣고
- 자연어로 대화

### Gemini

Gemini도 보통 raw skill 파일보다 복사한 지시문 방식이 더 잘 맞습니다.

실용적인 방법:

- 이 저장소를 참고 자료로 사용
- 핵심 규칙을 작업 지시문에 복사
- 자연어로 요청

## 파일 구성

- `SKILL.md`: 핵심 동작 규칙
- `agents/openai.yaml`: 메타데이터
- `README.md`: 영어 설명
- `README.ko.md`: 한국어 설명

## 참고

- **OPIc English only**
- 비공식 연습용 도구입니다
- 공식 라이브 시험 문제는 제공하지 않습니다

