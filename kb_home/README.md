---
id: kb-home
title: kb_home — github-prac 지식 베이스 진입점
type: map
status: stable
updated: 2026-08-18
---

# kb_home

이 저장소(`github-prac`)에 쌓인 분석 문서를 **사람과 LLM이 같은 경로로 찾아 들어올 수 있게** 정리한 위키입니다.

원문은 옮기지 않았습니다. 루트의 `포터/`, `가치사슬/`, `KSF/`, `시장규모/`, `페르소나/`, `CJM/`, `OS/`, `JTBD/` 폴더가 그대로 원본이고, kb_home은 그 위에 **색인·요약·규칙**을 얹는 층입니다. 원문을 고칠 때 kb_home을 고치지 않아도 링크는 깨지지 않지만, 판단이 바뀌면 여기 요약도 같이 손봐야 합니다.

## 어디서부터 읽는가

| 목적 | 들어갈 곳 |
|---|---|
| 이 저장소가 무슨 순서로 쌓였는지 보기 | [분석 사슬 지도](./01_maps/moc-analysis-chain.md) |
| 방법론만 골라 보기 | [방법론 지도](./01_maps/moc-frameworks.md) |
| 특정 시장·사례로 들어가기 | [사례 지도](./01_maps/moc-cases.md) |
| 아직 답이 없는 것 확인하기 | [열린 질문](./01_maps/moc-open-questions.md) |
| 용어 뜻 확인하기 | [용어집](./00_meta/glossary.md) |
| 새 문서 쓰기 | [템플릿](./06_templates/) · [작성 규칙](./00_meta/conventions.md) |

LLM으로 작업할 때의 읽기·쓰기 규칙은 [AGENTS.md](./AGENTS.md)에 따로 적어 뒀습니다.

## 폴더 구조

```
kb_home/
├── README.md              이 문서 — 위키 진입점
├── AGENTS.md              LLM 작업 규칙 (읽는 순서, 손대도 되는 범위)
├── 00_meta/               위키 자체의 규칙 — 작성 규칙·분류 체계·용어집·변경 기록
├── 01_maps/               MOC(Map of Content) — 주제별 관문, 여기서 원문으로 흩어짐
├── 02_concepts/           개념 하나당 파일 하나 (원자 노트)
├── 03_frameworks/         방법론 8종의 요약 카드 + 원문 링크
│   ├── porter-five-forces/    포터의 5가지 힘
│   ├── value-chain/           가치사슬
│   ├── ksf/                   핵심 성공 요인
│   ├── market-sizing/         TAM-SAM-SOM
│   ├── persona/               페르소나·스펙트럼
│   ├── cjm/                   고객 여정 지도
│   ├── opportunity-score/     기회점수 (AOS·DOS)
│   └── jtbd/                  Jobs To Be Done
├── 04_cases/              사례별 적용 — 시장 하나가 폴더 하나
│   └── sports-ott-accessibility/
│       ├── evidence/          인터뷰·수치 근거
│       └── decisions/         결정 기록 (무엇을 왜 그렇게 정했는지)
├── 05_sources/            출처 — raw/ 원본 파일, notes/ 인용 가능한 요약
├── 06_templates/          새 문서 스캐폴드
├── 07_prompts/            재사용 프롬프트·에이전트 지시문
├── 08_archive/            폐기·구버전 (지우지 않고 옮김)
└── assets/                이미지·다이어그램
```

## 왜 이렇게 나눴는가

방법론(`03_frameworks`)과 사례(`04_cases`)를 갈라 놓은 게 핵심입니다. 이 저장소의 문서는 대부분 "방법론 → 시장 두 곳 적용 → 비교" 꼴로 반복되는데, 둘을 한 폴더에 두면 프레임워크를 다시 쓰려는 사람과 특정 시장 결론만 확인하려는 사람이 같은 목록을 뒤져야 합니다.

출처(`05_sources`)를 따로 뺀 이유도 비슷합니다. 숫자가 어디서 왔는지는 분석 문서마다 반복해서 적기보다 한 곳에 모아 두고 가리키는 편이 검증하기 쉽습니다.
