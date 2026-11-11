# 02. 조직

## 조직도

```
사장 겸 디렉터 (사용자) ─ 방향 제시 · 승인 1 · 승인 2
 └─ 비서실장 (메인 에이전트) ─ 배분 · 취합 · 충돌 조정 · 보고 · 학습 기록
     ├─ 트렌드 리서처 (사원)        01_research
     ├─ 제품 기획자 (대리)          02_concept
     ├─ 카피라이터 (대리)           03_copy
     ├─ SNS 콘텐츠 기획자 (사원)    04_sns
     ├─ 검수관 (과장 · 독립)        읽기 전용 · 최종 관문
     ├┄ 비주얼 디렉터 (대리)        05_visual       합류 예정
     └┄ 성과 분석가 (사원)          06_performance  합류 예정
```

검수관을 팀 밖에 독립으로 둔 이유: 같은 팀 안에서 검토하면 자기 작업을 자기가 채점하는 구조가 된다. 식품은 "저당", "제로", 건강 효능 표현 하나로 문제가 될 수 있어 별도 관문이 필요하다.

## 직급 = 권한

| 직급 | 할 수 있는 것 | 할 수 없는 것 |
|---|---|---|
| 사장 | 방향 제시 · 콘셉트 선택 · 최종 승인 | — |
| 비서실장 | 직원 호출 · 취합 · 충돌 조정 · 기록 | 직접 실무 · 콘셉트·결과 확정 |
| 과장 | 대외 결과물 재작업 판정 (최대 2회) | 파일 쓰기 · 내용 직접 수정 |
| 대리 | 완성본 작성 · 동료 결과물 검토 | 다른 직원에게 지시 · 확정 |
| 사원 | 조사 · 초안 · 동료 결과물 검토 | 판단이 필요한 결정 (질문으로 올림) |

## 직원별 상세

| 직원 | 담당 | 도구 | 산출물 | 이 직원의 결과를 검토 | 이 직원이 검토 |
|---|---|---|---|---|---|
| trend-researcher | 시장·경쟁 제품·트렌드·리뷰 조사, 근거 대장(E) | Read, Glob, Grep, WebSearch, WebFetch, Write | research_report, competitor_table, voice_of_customer, evidence, sources | product-planner | 콘셉트 (근거 일치) |
| product-planner | 인사이트·메시지, 콘셉트 2~3안 | Read, Glob, Grep, Write | insights, concepts, concept_<안> | trend-researcher + quality-reviewer | 리서치, 카피 (콘셉트 일치) |
| copywriter | 제품명·패키지·상세페이지 카피 | Read, Glob, Grep, Write | product_names, package_copy, detail_page_copy | product-planner + quality-reviewer | SNS (제품명·톤) |
| sns-content-planner | 릴스·쇼츠 구성, 게시물 캘린더 | Read, Glob, Grep, WebSearch, Write | reels_structure, reels_plan, content_calendar | copywriter + quality-reviewer | — |
| quality-reviewer | 표시·광고 표현, 근거 연결, 톤, 비방 | Read, Glob, Grep, WebSearch | 판정 텍스트 (비서실장이 저장) | — (최종 관문) | 대외 결과물 전부 |

## 직원 지침 위치
- 공통 층: `/CLAUDE.md` — 회사, 브랜드, 조직, 승인 규칙, 공통 규칙
- 개인 층: `/.claude/agents/<직원>.md` — 직급, 담당, 쓰기 폴더, 도구, 할 수 없는 일, 완료 기준

브랜드 메시지가 바뀌면 공통 층 한 곳만 고친다.
