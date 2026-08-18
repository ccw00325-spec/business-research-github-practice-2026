---
id: meta-taxonomy
title: 분류 체계
type: meta
status: stable
updated: 2026-08-18
---

# 분류 체계

## type

문서가 어떤 역할인지 하나만 고릅니다.

| type | 역할 | 사는 곳 |
|---|---|---|
| `map` | 관문. 다른 문서로 흩어 보냄 | `01_maps/`, 각 폴더 README |
| `concept` | 개념 하나 | `02_concepts/` |
| `framework` | 재사용 가능한 절차·판정 기준 | `03_frameworks/` |
| `case` | 특정 시장·제품에 적용한 결과 | `04_cases/` |
| `decision` | 무엇을 왜 그렇게 정했는지 | `04_cases/*/decisions/` |
| `source` | 출처 요약과 인용 가능한 수치 | `05_sources/notes/` |
| `template` | 새 문서 스캐폴드 | `06_templates/` |
| `prompt` | 재사용 프롬프트 | `07_prompts/` |
| `meta` | 위키 운영 규칙 | `00_meta/` |

## tag

주제 축입니다. 필요한 만큼 붙이되 새 값은 여기 먼저 등록합니다.

**분석 단계** — `industry-structure`, `value-chain`, `ksf`, `market-sizing`, `persona`, `journey`, `prioritization`, `interview`

**시장** — `ott`, `commerce`, `accessibility`, `sports`

**성질** — `methodology`, `application`, `comparison`, `raw-data`, `open-question`

## 쓰지 않는 것

- 태그로 상태를 표현하지 않습니다. 상태는 `status` 필드입니다
- 태그 계층(`market/ott`)을 만들지 않습니다. 평평하게 둡니다
