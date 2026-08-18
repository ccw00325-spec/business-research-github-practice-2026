---
id: meta-conventions
title: 작성 규칙
type: meta
status: stable
updated: 2026-08-18
---

# 작성 규칙

## 파일명

- 소문자 영문 + 하이픈: `market-sizing.md`, `moc-analysis-chain.md`
- 원문 분석 문서는 기존 한글 파일명을 그대로 둡니다. 루트 폴더의 규칙(`KSF01-OTT.md`)과 kb_home의 규칙을 억지로 통일하지 않습니다
- 순번이 의미 있는 문서는 앞에 두 자리 숫자: `01-...`, `02-...`
- 폴더의 대표 문서는 `README.md`, 프레임워크 카드는 `index.md`

## 프론트매터

모든 문서 맨 위에 YAML 블록을 둡니다.

```yaml
---
id: 문서를 가리킬 짧은 키 (중복 금지)
title: 사람이 읽을 제목
type: concept | framework | case | source | map | meta | template | prompt | decision
status: draft | review | stable | archived
updated: YYYY-MM-DD
tags: [선택]
sources: [선택 — 05_sources/notes 의 id]
related: [선택 — 다른 문서의 id]
---
```

`updated`는 내용이 바뀔 때만 올립니다. 오탈자 수정으로는 올리지 않습니다.

## 링크

같은 저장소 안은 상대 경로로 걸고, 절대 경로(`C:\...`)는 쓰지 않습니다. 원문을 가리킬 때는 kb_home 기준으로 올라갑니다.

```markdown
[KSF 도출 방법론](../../KSF/KSF-도출-방법론.md)
```

## 상태 값

| status | 뜻 |
|---|---|
| `draft` | 초안. 다른 문서에서 결론으로 인용하면 안 됩니다 |
| `review` | 내용은 다 썼고 검토를 기다립니다 |
| `stable` | 인용해도 되는 상태 |
| `archived` | 밀려난 판단. `08_archive/`에 있습니다 |

## 한 문서 한 주제

개념 노트는 하나의 개념만 담습니다. 두 개념을 비교하고 싶으면 세 번째 문서를 만들고 양쪽을 링크합니다. 이 저장소의 `비교-*.md` 문서들이 이미 그 방식입니다.
