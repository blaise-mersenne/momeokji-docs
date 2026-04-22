# 00. 뭐먹지 문서 마스터 인덱스 (Master Index)

> **마지막 업데이트:** 2026-04-21
> **문서 상태:** 초안 (Draft) - 지속 업데이트 예정

---

## 서비스 한 줄 정의

개인의 식성, 과거 식사 데이터, 현재 상황(위치/식재료)을 종합 분석하여 최적의 메뉴와 획득 방법(외식/직접 요리)을 제안하는 **초개인화 푸드 큐레이션 플랫폼.**

---

## 문서 구조 및 참조 가이드

| 문서 | 내용 | 주요 참조 대상 |
|---|---|---|
| **00_MASTER.md** | 전체 문서 지도 (현재 문서) | 전체 팀 |
| **01_PRODUCT.md** | PRD + BM + Core User Flow | 전체 팀, 신규 합류자 |
| **02_USER_EXPERIENCE.md** | 홈UX + 온보딩 + 페르소나/엣지케이스 | 프론트엔드, 디자이너 |
| **03_RECOMMENDATION.md** | 추천엔진 + 입맛평가 + 동적정렬 | 백엔드, ML |
| **04_DATA_PIPELINE.md** | 메뉴DB구축 + UGC태그추출 + 데이터플라이휠 | 백엔드, 데이터 |
| **05_B2B_CONSOLE.md** | 파트너콘솔 + 그룹추천 BM연계 | B2B 개발, 영업 |

---

## Epic → 문서 매핑

| Epic | 기능명 | 위치 |
|---|---|---|
| Epic 1 | 듀얼 추천 엔진 (사먹기 vs 해먹기) | 03_RECOMMENDATION.md |
| Epic 2 | 다차원 입맛 평가 시스템 | 03_RECOMMENDATION.md |
| Epic 3 | B2B 파트너 콘솔 | 05_B2B_CONSOLE.md |
| Epic 4 | 프리미엄 그룹 추천 | 05_B2B_CONSOLE.md |
| Epic 5 | 메인 홈 및 내비게이션 UX | 02_USER_EXPERIENCE.md |
| Epic 6 | 회원가입 및 온보딩/프로파일링 | 02_USER_EXPERIENCE.md |
| Epic 7 | 서비스 페르소나 및 예외 상황 방어 UX | 02_USER_EXPERIENCE.md |
| Epic 8 | 초개인화 동적 정렬 및 마이크로 태그 | 03_RECOMMENDATION.md |
| Epic 9 | 하이브리드 메뉴 데이터 구축 및 태그 추출 | 04_DATA_PIPELINE.md |

---

## 미확정 항목 전체 목록

개발 착수 전 반드시 확정이 필요한 항목들입니다. 확정 시 각 문서의 해당 항목을 업데이트하고 아래 목록에서 제거해 주세요.

### BM/정책 관련
| ID | 내용 | 위치 |
|---|---|---|
| P-1 | 프리미엄 그룹 추천 월 구독 가격 | 01_PRODUCT.md |
| P-2 | B2B 사먹기 광고 CPC/CPM 단가 | 01_PRODUCT.md |
| P-3 | 해먹기 수수료(CPS) 수취 수수료율 | 01_PRODUCT.md |
| P-4 | 소형 마트 솔루션 이용료 수치 | 01_PRODUCT.md |
| P-5 | 무료 → 프리미엄 플랜 전환 시점 및 기준 | 01_PRODUCT.md, 05_B2B_CONSOLE.md |

### UX 관련
| ID | 내용 | 위치 |
|---|---|---|
| U-1 | 해먹기 Dimmed 처리 기준 수치 (현재 "50% 초과") | 02_USER_EXPERIENCE.md |
| U-2 | 비회원 Soft Gating 발동 횟수 기준 (현재 "1회") | 02_USER_EXPERIENCE.md |
| U-3 | 2D 캐릭터(동료 아바타) 디자인 및 리소스 확보 여부 | 02_USER_EXPERIENCE.md |
| U-4 | FAB 버튼 최종 디자인 형태 | 02_USER_EXPERIENCE.md |

### 추천 알고리즘 관련
| ID | 내용 | 위치 |
|---|---|---|
| R-1 | 완벽 매칭 예외 규칙 발동 수치 (현재 "매칭률 95%") | 03_RECOMMENDATION.md |
| R-2 | 거리 필터 예외 시 허용 초과 범위 | 03_RECOMMENDATION.md |
| R-3 | 혈당 스파이크 방지 가중치 구현 방식 및 데이터 소스 | 03_RECOMMENDATION.md |
| R-4 | 직전/이후 식사 연계 필터링 구현 방식 | 03_RECOMMENDATION.md |
| R-5 | 가구 형태 자동 추정 알고리즘 기준 | 03_RECOMMENDATION.md |
| R-6 | 입맛 유사도 협업 필터링 구현 방식 | 03_RECOMMENDATION.md |

### 데이터 파이프라인 관련
| ID | 내용 | 위치 |
|---|---|---|
| D-1 | 포털 지도 API 크롤링/연동 가능 범위 (약관 검토) | 04_DATA_PIPELINE.md |
| D-2 | UGC 자연어 태그 마이닝 AI 모델 및 구현 방식 | 04_DATA_PIPELINE.md |
| D-3 | 태그 신뢰도 점수 집계 기준 수치 | 04_DATA_PIPELINE.md |
| D-4 | 게이지 애니메이션 보상 UI 구현 방식 | 04_DATA_PIPELINE.md |

### B2B 콘솔 관련
| ID | 내용 | 위치 |
|---|---|---|
| B-1 | POS 시스템 및 프린터 연동 개발 여부 (Tech Spike) | 05_B2B_CONSOLE.md |
| B-2 | 그룹 추천 무료 사용 횟수 제한 수치 | 05_B2B_CONSOLE.md |
| B-3 | 그룹 추천 최대 초대 가능 인원 수치 | 05_B2B_CONSOLE.md |
| B-4 | 그룹 중복 방지 기준 시간 (현재 "24시간") | 05_B2B_CONSOLE.md |
| B-5 | 오디언스 취향 인사이트 익명화 처리 방식 | 05_B2B_CONSOLE.md |
| B-6 | 스페이스 입장 코드 자릿수 (현재 "4~6자리") | 05_B2B_CONSOLE.md |

---

## 외부 참조 링크

| 항목 | 링크 |
|---|---|
| Figma 프로토타입 (v1.0) | https://www.figma.com/proto/ihpTXWZsn4X9k7UXX74N2E |

---

## 📝 변경 이력 (CHANGELOG)

| 날짜 | 내용 | 작성자 |
|---|---|---|
| 2026-04-21 | 최초 문서 구조 수립 및 전체 PDF → Markdown 변환 완료 | Claude |
