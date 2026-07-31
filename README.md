# 📊 analytics-portfolio

> **비즈니스를 먼저 경험한 데이터 분석가의 포트폴리오 저장소**
> 이커머스 앱마켓에서 마케팅 운영을 하며 필요해서 시작한 분석이, 지금은 본업이 되었습니다.
>
> *I believe good analytics starts with understanding the business problem.*

---

## 👋 소개

비즈니스 문제를 데이터와 시스템으로 해결하는 15년 경력의 Business Analyst. 최근 10년간 MAU 1,000만 규모의 이커머스 앱마켓에서 마케팅 운영과 데이터 분석을 수행해 왔습니다.

**Core Strengths**

- **Experiment Design** — A/B 테스트 설계·검증 (인센티브 구조 실험으로 CAC 약 30% 절감)
- **Product & Marketing Analytics** — 세그멘테이션 · 코호트 · 리텐션 · 프로모션 ROI
- **Dashboard Development** — 셀프서브 Tableau BI 구축·운영
- **Data Governance** — 테이블 사전 · 표준 지표 쿼리 · SQL Dictionary
- **Workflow Automation** — 반복 산출물 생성 4시간 → 10분 (Python + AI)

📁 **선별 포트폴리오**: [tinyurl.com/kyungmin-ba](https://tinyurl.com/kyungmin-ba)
💼 **LinkedIn**: [linkedin.com/in/kkyungmin1](https://linkedin.com/in/kkyungmin1)

---

## 🖼 Featured Projects

실물 산출물을 가명 데이터로 재현한 샘플입니다. 각 README에 배경 → 설계 → 결과 서사가 정리되어 있습니다.

| 프로젝트 | 내용 |
|---|---|
| 🌐 [Partner Onboarding Knowledge Hub](onboarding_playbook/README.md) | 해외 파트너 Self-service Onboarding 시스템 — 35+ 페이지 Knowledge Hub + 34장 마케팅 플레이북, 1.5년 운영 |
| 📖 [SQL Dictionary](sql_dictionary/README.md) | "같은 지표, 다른 숫자" 문제를 해결한 쿼리 표준화 위키 — 기준정의·[CTE] 모듈·테이블/코드 사전·ERD |
| 📈 [Tableau Dashboards](dashboards/README.md) | GMV Breakdown(리워드별 분해 + 공헌이익 라인) · 주차별 게임 포지셔닝 · 이벤트 퍼널(발급→사용→거래→ROAS) |
| 🏆 [신작 랭킹 알고리즘](ranking_algorithm/README.md) | 2019년 설계한 시간감쇠 랭킹 — **현재까지 실서비스 운영 중** (실화면 포함) |

<p>
<a href="onboarding_playbook/README.md"><img src="onboarding_playbook/images/help_toc_sample.png" alt="Onboarding Knowledge Hub" width="33%"></a>
<a href="dashboards/README.md"><img src="dashboards/images/gmv_breakdown_sample.png" alt="GMV Breakdown Dashboard" width="49%"></a>
</p>

---

## 📋 Complete Project List — 30+ projects

6개 영역, 30건+ 분석·구축 이력입니다. 전체 목록은 [PROJECTS.md](PROJECTS.md)에 시기·수행 내용·핵심 기법과 함께 정리되어 있습니다 (⭐ 포트폴리오 수록 6건, 🖼 재현 샘플 링크 포함).

| 영역 | 대표 프로젝트 |
|---|---|
| 🧪 실험 설계 · A/B 테스트 | 결제수단 전환 A/B 테스트 1차(2×2 세그먼트 설계) → 후속 재설계로 **CAC 약 30% 절감** |
| 🎯 프로모션 · 이벤트 분석 | 프로모션 사후분석 정례화(순증 효과·체리피커 분리·ROI), 신규 게임 유입 마케팅 효과 분석(4개 타이틀 교차 검증) |
| 👥 세그멘테이션 · 코호트 | 크레딧 정책 변경 1년 코호트 추적, 결제액×등록여부 Tier 세그먼트, 신규/복귀/기존 유입 분해 |
| 🏆 랭킹 · 스코어링 · 분류체계 | 시간감쇠 신작 랭킹(프로덕션 운영 중), 2축 패싯 분류체계(1,200+ 상품 라벨링) |
| ⚙️ 파이프라인 · 자동화 | 프로모션 대상 선정 자동화, 업무 오케스트레이션(**4시간 → 10분**), BI 연동 정례 리포팅 |
| 📊 대시보드 · 거버넌스 · KM | GMV Breakdown 대시보드, SQL Dictionary(25개 테이블·562개 컬럼), 파트너 온보딩 Knowledge Hub |

➡️ [전체 목록 보기 → PROJECTS.md](PROJECTS.md)

---

## 🔁 일하는 방식

이 저장소의 프로젝트들은 하나의 사고방식에서 나왔습니다 — **반복을 발견하면 시스템으로 바꿉니다.**

- 반복 문의 → **Knowledge Hub** (파트너 온보딩)
- 반복 쿼리 → **SQL Dictionary** (지표 표준화)
- 반복 분석 → **Tableau 대시보드** (셀프서브 BI)
- 반복 업무 → **Python 자동화** (4시간 → 10분)

> *I don't just solve problems — I design systems that prevent the same problem from happening again.*

분석도 같은 순서입니다 — **질문을 먼저 쓰고, 데이터는 그다음.**

---

## 🔒 원칙

1. **모든 데이터는 합성·가명 데이터입니다.** 실제 회사 데이터·코드·내부 기준값은 일절 포함하지 않으며, 모든 케이스는 공개 가능한 형태로 재구현했습니다.
2. **레시피 형식**: `언제 쓰나 → 재료(데이터 형태) → 코드 → 주의할 점`. "언제 쓰나"는 전부 실무에서 직접 겪은 상황입니다.
3. **검증 규율**: 모든 노트북은 첫 셀에 "확인해야 할 질문"을 먼저 쓰고 시작하며, Sanity Check 셀을 상설로 둡니다.

---

## 📎 그 외

- 🎪 **[Conference Notes](conferences/README.md)** — 컨퍼런스 참관기 8건 (2024.07~2026.06)
- 🍳 실무 재구현 케이스 스터디와 분석 레시피 노트북은 별도 저장소(**analytics-cookbook**)로 준비 중

---

*이 저장소는 계속 업데이트됩니다. (Last updated: 2026.07)*
