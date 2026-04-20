# OPIc Question Generator Skill

[Read this README in English](README.md)

> **OPIc English only**를 위한 비공식 연습용 skill

![OPIc Question Generator](assets/cover.png)

## 개요

이 skill은 **OPIc English** 연습을 위해 문제를 만들고, 사용자가 쓴 답변을 더 자연한 말하기 표현으로 고쳐주는 용도입니다.

할 수 있는 것:

- 오픽 스타일 연습 문제 생성
- 서베이 기반 문제 묶음 생성
- 롤플레이 및 후반 하드 팔로업 문제 생성
- 답변 교정
- 더 자연한 spoken expression 제안
- `IM / IH / AL` 스타일 예시 제공

하지 않는 것:

- 공식 라이브 시험 문제 제공
- 특정 유료 강의나 교재 원문 복제
- 공식 점수 보장

## 범위

이 skill이 다루는 범위:

- **OPIc English**

다루지 않는 범위:

- 다른 언어의 OPIc
- OPIc 연습을 벗어난 일반 영어 회화 전체

## 사용 방법

### AI 에이전트용

아래 요청이 들어오면 이 skill을 사용하는 것이 적절합니다.

- 오픽 모의고사 문제 생성
- 서베이 기반 연습 세트 생성
- 오픽 답변 교정
- 더 자연한 spoken rewrite
- IM / IH / AL 스타일 예시 생성

권장 흐름:

1. 사용자가 서베이 주제를 줬는지 확인
2. 난이도 밴드를 줬는지 확인
3. 원하는 출력 모드를 확인
4. 요청한 것만 생성

권장 출력 모드:

- questions only
- questions + types
- questions + MP
- questions + sample answers
- answer correction
- answer correction + natural rewrite
- answer correction + IM/IH/AL versions

### 사람 사용자를 위한 예시

자연어로 그냥 요청하면 됩니다.

예시:

```text
서베이 주제는 movies, youtube, cafe야.
3-4 난이도로 15문항 모의고사를 만들어줘.
한국어 설명도 같이 붙여줘.
```

```text
내 답변을 교정해주고 왜 어색한지 설명해줘.
더 자연한 버전도 같이 보여줘.
```

```text
내 답변을 IM, IH, AL 느낌으로 각각 바꿔줘.
```

## 입력 옵션

원하면 아래 옵션을 요청에 직접 넣을 수 있습니다.

- `survey_topics`
  예: `movies, youtube, cafe, technology`
- `difficulty_band`
  예: `1-2`, `3-4`, `5-6`
- `difficulty_detail`
  예: `3-3`, `4-4`, `5-5`, `6-6`
- `question_count`
  예: `1`, `3`, `15`
- `output_mode`
  예: `questions only`, `questions + MP`, `answer correction`
- `language`
  예: `Korean`, `English`, `mixed`
- `include_roleplay`
  예: `yes`, `no`
- `include_hard_followups`
  예: `yes`, `no`
- `answer_style`
  예: `corrected only`, `natural rewrite`, `IM/IH/AL`

## 난이도 구조

이 skill은 난이도를 두 단계로 다룹니다.

### 1. `difficulty_band`

문제 생성에 가장 크게 영향을 주는 설정입니다.

- `1-2`
  더 단순한 질문, 과거 경험 비중이 낮음
- `3-4`
  표준 콤보 구조 + 롤플레이 포함
- `5-6`
  더 어려운 후반 질문, 비교/문제 해결 비중 강화

### 2. `difficulty_detail`

세부 선호값입니다.

- `1-1`, `1-2`, `2-1`, `2-2`
- `3-3`, `3-4`, `4-3`, `4-4`
- `5-5`, `5-6`, `6-5`, `6-6`

이 값은 미세 조정용입니다.  
각 세부값을 완전히 별도의 엔진처럼 다루지는 않습니다.

## 주요 출력 형태

### 1. 문제 생성

- 단일 질문
- 3문항 콤보
- 15문항 모의고사
- 롤플레이 세트
- 하드 팔로업 세트

### 2. 답변 교정

- 문법과 표현 수정
- 원래 의미 유지
- 실제로 말하기 쉽게 정리

### 3. 자연한 말하기 표현

- 더 쉬운 표현 제안
- 더 자연한 오픽 스타일 표현 제안

### 4. 레벨 스타일 예시

원하면 아래 스타일로 보여줄 수 있습니다.

- `IM version`
- `IH version`
- `AL version`

이 예시는 연습용 스타일 참고이며, 공식 채점 보장은 아닙니다.

## 공개용 주의사항

- 이 skill은 **비공식 연습 도구**입니다.
- 공개된 OPIc 구조와 일반적으로 알려진 연습 패턴을 바탕으로 구성됩니다.
- 공식 라이브 문제를 복원한다고 주장하지 않습니다.
- 연습과 코칭 목적에 맞춰 사용해야 합니다.

## 저장소 구조

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

## 업로드 전 확인

GitHub 업로드 전에 아래를 확인하세요.

- 이미지 파일이 `assets/cover.png`에 있는지
- 프로젝트가 **OPIc English only**로 설명되어 있는지
- 특정 유료 자료 원문을 복사하지 않았는지
- 공식 라이브 문제라고 주장하지 않는지

