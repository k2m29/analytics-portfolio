# ❄️ Snowflake World Tour Seoul 2026

`#AIReadyData` `#시맨틱뷰` `#지표표준화` `#행동예측` `#DataCleanRoom`

> 📅 **2026.08.27** · 🏢 **Snowflake** · 📍 코엑스 컨퍼런스센터

## 🔑 Key Findings

> **행사 전체를 관통하는 메시지는 "모델보다 데이터"** — LLM이 상향 평준화된 지금 Agentic AI의 성패는 AI Ready Data(품질·메타데이터·거버넌스)가 좌우한다는 것으로, 키노트·KB·다이닝브랜즈·IGAWorks 전 세션에서 공통으로 강조됨
>
> - **Snowflake의 한국 시장 투자 본격화**
>   - 2026년 3월 서울 오피스 개소 등 FY27 한국 우선순위를 발표함 (AI/Cortex 확산, 파트너 에코시스템, 무료 교육 프로그램)
> - **시맨틱 뷰(Semantic View)가 가장 인상적이었음**
>   - '매출' 같은 지표 정의를 dbt 모델 코드 한 곳에서 확정해 AI와 사람이 같은 기준으로 쓰게 하는 계층
>   - 우리 회사에서 SQL Dictionary로 지표 표준을 관리하는 것과 같은 문제의식이며, **지표 표준화가 AI 활용의 전제 조건**이 된다는 방향성을 확인함
> - **마케팅 관점에서는 IGAWorks의 LBM(행동 예측 모델) 기반 타깃팅이 볼만했음**
>   - LLM이 다음 단어를 예측하듯 유저의 '다음 행동 확률'을 예측해 오디언스를 추출함
>   - Snowflake Data Clean Room으로 자사 데이터와 외부 행동 데이터를 비식별 결합하는 구조 — CRM 타깃팅 확장 시 참고할 만함
> - **AX 도입 시 성과 관리 프레임 (KB·다이닝브랜즈 사례)**
>   - 반복 인시 절감 / 비용 / 매출 / 리스크 / 데이터 자산화 5개 영역으로 KPI·목표치·ROI를 산정하는 방식을 참고할 수 있음

## 💡 Lessons Learned

- **지표 표준화가 AI 활용의 전제 조건이라는 것을 외부에서 확인함.** 시맨틱 뷰는 '매출'의 정의를 코드 한 곳에 못박아 AI와 사람이 같은 기준을 쓰게 하는 계층인데, 우리가 SQL Dictionary로 하고 있는 일과 문제의식이 동일하다. 지표 사전을 AI가 참조하는 형태로 발전시킬 여지가 있음.
- **CRM 타깃팅을 '행동 확률' 기준으로 확장할 여지.** 세그먼트를 규칙(과거 행동)으로 자르는 대신 '다음 행동 확률'로 뽑는 접근 — 우리 이탈 예측 모델을 타깃 추출까지 밀어붙이면 같은 구조가 된다.
- **Data Clean Room은 자사 데이터의 한계를 보완하는 현실적 수단.** 자사 데이터로는 유저의 외부 행동을 알 수 없는데, 원본 반출 없이 비식별 결합으로 보완하는 구조. 제휴 데이터 활용을 검토할 때 참고.
- **AX 성과 관리 프레임이 실용적이었음.** 5개 성과 영역별로 산식(예: 인시 절감 = 업무 건수 × 기준 소요시간 × AI 절감률)을 먼저 정의하고, 외부 벤치마크는 목표 설정 참고값으로만 쓰되 자사 준비도에 맞춰 보수 조정 — **수치보다 과제별 산정 기준을 확보하는 것이 핵심**이라는 원칙이 인상적.

---

## 📝 세션 노트

> 원문 전체 기록입니다. 세션별로 펼쳐서 읽어보세요. 각 세션은 요약 → `---` → 상세 순서입니다.

<details>

<summary>SESSION 1: Keynote — Making AI Real for Business (10:00~11:30)</summary>

- 키노트의 중심 개념은 '에이전틱 엔터프라이즈(Agentic Enterprise)' — AI 모델 선택, 엔터프라이즈 데이터·컨텍스트, 소프트웨어·앱을 중앙의 '에이전틱 제어 영역'이 연결하는 구조를 제시함
- 고객의 선택권과 제어권을 강조함 — 데이터는 항상 고객 소유, 고객 데이터를 자사 모델 학습에 사용하지 않음, 특정 모델·벤더 종속 없음
- FY27 한국 우선순위 발표: 2026년 3월 서울 오피스 개소, AI·Cortex 확산(PoC→운영 전환 가속), 파트너 에코시스템, AI 데이터 입문 무료 교육(2일 코스, 하반기 시행)
- 가상 스포츠 리그(SnowLeague) 라이브 데모 — Streamlit 대시보드로 도시별 수익·마진을 실시간 분석하며 '일회성 성과를 수익성 있는 확장 계획으로 전환'하는 과정을 시연함

---

- **FY27 한국 비즈니스 주요 우선순위**
  - 2026년 3월 서울 오피스 개소(FY27 Q1), 장기 투자로 고객 과제 해결 가속화를 선언함
  - AI·Cortex 확산: 기업 내 데이터 위에서 AI 구축, PoC에서 운영 전환 가속
  - Partner Ecosystem: 구축·이관 가속화, 공동 고객 성과 확대
  - Global Revenue Enablement: AI 데이터 입문 무료 교육(2일 코스)을 하반기부터 본격 시행

- **에이전틱 엔터프라이즈 — 성공적인 성과를 위한 핵심 요소**
  - 중앙의 '에이전틱 제어 영역'을 축으로 AI 모델 선택 / 엔터프라이즈 데이터 및 컨텍스트 / 소프트웨어 및 앱 3개 요소가 연결되는 구조를 제시함
  - 기업이 AI 변화 속도를 따라가면서도 특정 벤더에 종속되지 않아야 하고, ERP 등 기존 시스템 자산과 에이전트가 원활하게 연동되어야 한다는 취지임

- **SnowLeague 라이브 데모**
  - 페르소나: 리그 영업 부문 VP. CEO는 매출 목표 상향, CFO는 수익성 확보를 요구하는 상황에서 마진율을 유지하며 지난 경기의 매출 효과를 다른 도시에서 재현하는 과제임
  - Streamlit Apps로 구축한 'SnowLeague Fan Command Center' 시연 — 비즈니스&참여 지표 / 경기장 영상 분석 / 실시간 팬 활동 피드 탭 구성
  - 총 수익 $40.3M, 순이익률 5.6%, VIP 업그레이드 8,370건, 최고 마진 도시 부산(+27%) 등 도시 필터로 도시별 수익 vs 인건비·마진을 비교 분석함

- **고객의 선택권과 제어권 (데이터·AI 비용 전반의 거버넌스)**
  - 고객의 거버넌스: 데이터는 고객이 지정한 위치에 그대로 유지, 고객이 승인한 방식으로만 액세스
  - 고객의 모델 선택권: 모든 주요 모델을 종속성 없이 지원, 고객 요구에 맞게 최적화
  - 고객이 정한 비용 규칙: 프런티어 모델부터 오픈소스 모델까지 전체 스펙트럼을 제공해 비용을 적정 수준으로 조정
  - 데이터는 고객의 독점적 자산이자 경쟁 우위이며, Snowflake는 고객 데이터를 자사 모델 학습에 사용하거나 학습용으로 제공하지 않는다고 명시함

- **거버넌스 기반 AI 실행 — 전체 앱 에코시스템 지원**
  - 제로 카피 통합: SaaS 데이터 실시간 쿼리, ETL/데이터 이동 불필요
  - 고객맞춤형 앱: CoCo를 통한 빌드, 설계 단계부터 거버넌스 적용
  - 마켓플레이스 앱: 데이터가 있는 곳에서 앱 실행, 데이터 이동 없음

</details>

<details>

<summary>SESSION 2: Keynote 고객 사례 — AI Ready Data가 여는 KB Agentic AI 미래 (KB국민은행)</summary>

- '검색·답변하는 AI'를 넘어 '스스로 판단하고 행동하는 AI(Agentic AI)'로의 전환 비전을 제시함 — 업무 결과를 단말기에 직접 입력, 운영 업무 자동 처리, 멀티스텝 오케스트레이션
- 행동하는 AI의 3대 요건: 강력한 LLM 모델 + 풍부한 Tool(MCP 기반) + AI Ready Data. 모델이 상향 평준화된 지금은 데이터 경쟁력이 성패를 좌우한다고 강조함
- 에이전트 적용 범위를 프런트오피스(PB·RM, 금융상담 — 사용 정착)에서 미들·백오피스(리스크·여신심사·법률지원 — 개발 중), AI Dev 센터(발족)까지 전방위 확장 중임
- 데이터 분석 에이전트 KB DAVIS: 자연어 질문을 SQL로 변환하고 인사이트 보고서를 자동 완성함

---

- **금융권 AI의 5대 데이터 도전 과제**
  - 단절된 데이터 사일로 / 정형·비정형 데이터의 혼재 / 메타데이터 부재 / 데이터 품질·신뢰성 불균일 / 거버넌스·컴플라이언스 부족 — 이를 해결해야 '행동하는 AI'가 가능하다고 진단함

- **KB국민은행 에이전트 현황**
  - 프런트오피스(사용 정착): PB·RM 에이전트(고객 포트폴리오 분석·시장 인사이트), 금융상담 에이전트(상품 추천·상담 스크립트)
  - 미들&백오피스(개발 중): 리스크 관리 에이전트(시장·신용·운영 리스크 실시간 모니터링, 이상 징후 자동 감지), 여신심사 에이전트(심사 프로세스 자동화), 법률지원 에이전트(계약서 검토·규제 변경 모니터링·컴플라이언스 체크)
  - AI Dev 센터(발족): IT개발 전 과정 자동화(기획→요건정의→개발→테스트→반입), AI Native 개발 프로세스 정착, 대직원→대고객 AX 확장
  - KB DAVIS(데이터 분석 에이전트): 자연어 질문→SQL 변환, 종합 데이터 분석 및 인사이트 보고서 자동 완성

- **행동하는 AI로의 전환 (Next Vision)**
  - 현재 단계(답변하는 AI): 질문 분석 → 답변 제공 → 보고서 작성
  - 목표 단계(행동하는 AI): 업무 결과를 단말기에 직접 입력(사람 개입 없이 시스템 반영), 운영 업무 자동 처리, 멀티스텝 Orchestration — AX 생산성의 Quantum Jump 실현

- **행동하는 AI를 위한 3대 요건**
  - 강력한 LLM 모델: 추론+플래닝+툴 콜링이 조화롭게 작동하는 기반 지성
  - 풍부한 Tool: MSA 기반 시스템과 MCP(Model Context Protocol)로 연결한 행동 수단
  - AI Ready Data: AI가 즉시 이해·활용할 수 있는 구조로 준비된 데이터 — 행동의 근거가 되는 가장 핵심적인 경쟁력

- **결론: From Data to Agent**
  - 모델이 상향 평준화된 지금 성패는 각 기업이 보유한 데이터의 품질과 활용도가 결정함. AI Ready Data 체계는 단기 프로젝트가 아니라 경쟁자가 쉽게 복제할 수 없는 장기 전략 자산임

</details>

<details>

<summary>SESSION 3: Track 4 — Iceberg 레이크하우스를 Zero-Ops로 굴리는 법 (13:00~13:30)</summary>

- Snowflake의 Iceberg 레이크하우스 전략은 Connect → Enhance → Zero-Ops 3단계 여정으로 설계됨. 세 방식 모두 Apache Iceberg 기반이라 완전 개방형·이동 가능·벤더 종속 없음
- Zero-Ops(Snowflake 관리형)는 Snowflake가 모든 유지관리를 대신해 오버헤드·TCO를 최소화하고, 네이티브 테이블 수준의 간편함과 IRC(Iceberg REST Catalog)를 통한 개방형 상호운용성을 제공함
- Snowflake 관리형 Iceberg 테이블에는 Data/Metadata Compaction, Automatic Clustering, Snapshot Expiry, Search Optimization 5종 최적화가 네이티브 테이블과 동일하게 자동 수행됨
- Connect(카탈로그 페더레이션): AWS Glue, OneLake, Unity, Google Lakehouse, Apache Polaris 등 외부 카탈로그의 Iceberg 테이블을 데이터 이동 없이 읽기·쓰기 가능. Connect→Enhance 마이그레이션은 명령 한 줄로 수행함

---

- **지능형 테이블 최적화 (자동 유지 관리 5종)**
  - Data Compaction: 작은 Parquet 파일을 최적 크기로 병합, delete-file 누적 제거, I/O 감소로 스캔 속도 향상
  - Metadata Compaction: 대량 DML 후 매니페스트 파일 재구성, 쿼리 계획의 메타데이터 오버헤드 감소
  - Automatic Clustering: 고카디널리티 컬럼 기준 클러스터링으로 파티션 프루닝 성능 향상
  - Snapshot Expiry: 일정에 따라 오래된 스냅샷 만료, 스토리지 회수하면서 Time Travel은 유지
  - Search Optimization: 고선택도 포인트 룩업 지원, 보조 인덱스 자동 생성

- **Connect: 모든 Iceberg 카탈로그와 페더레이션**
  - 카탈로그 연결 데이터베이스(CLD)로 거의 모든 위치의 데이터를 거버넌스 기반으로 통합 관리·활용함
  - 모든 Iceberg 테이블에 읽기·쓰기 지원, 스토리지 변경 사항 자동 감지·업데이트, Auto Discovery로 외부 Iceberg 테이블 자동 인식, 원격 IRC 연결
  - 연결 대상: AWS Glue, Microsoft OneLake, Unity, Google Lakehouse, Apache Polaris + 원격 카탈로그(Iceberg REST API). 데이터 레이크의 데이터를 Horizon Catalog로 보호함

- **레이크하우스 아키텍처 여정 설계 (3가지 배포 옵션)**
  - Connect(직접·외부 관리형): 외부 카탈로그나 원시 Parquet/Delta 파일에 기존 데이터가 있는 경우의 시작점. 데이터 이동 없이 즉시 분석 시작
  - Enhance(고객 스토리지 + Snowflake 관리형): Horizon Catalog로 고객 스토리지 버킷에서 Snowflake의 엔지니어링 기능 대부분 활용
  - Zero-Ops(Snowflake Storage + Snowflake 관리형): 오버헤드·TCO 최소화, 새 워크로드 추가에 적합. 네이티브 테이블과 동일한 간편함 + 완전한 개방형 상호운용성
  - 마이그레이션: Connect→Enhance는 명령 한 줄, Enhance→Zero-Ops도 곧 지원 예정임

</details>

<details>

<summary>SESSION 4: Track 4 고객 사례 — 다이닝브랜즈의 클라우드 데이터 현대화 여정 (13:40~14:10)</summary>

- 다이닝브랜즈그룹(외식업)이 Snowflake 기반 클라우드 데이터 현대화 + AX를 추진한 사례. 성능 테스트에서 Snowflake 파이프라인(EC2–Airflow, 2단계)이 기존 3단계 방식 대비 약 15% 우수(15분 26초 vs 18분 06초, 2,100만 건/2.3GB 기준)함
- AX는 2트랙 병행: Track A는 Snowflake 기반 데이터 플랫폼(DW·마트·셀프 대시보드, AI Ready Data), Track B는 AWS Bedrock 기반 Gen AI 플랫폼(Vector DB·RAG) — 2단계에서 '데이터 플랫폼 x Gen AI 인터페이스'로 확장함
- 성과 관리 프레임이 실용적이었음 — 반복 인시 절감(20~30%), 구매/재고/물류 비용(2~5%), 매출(1~3%), 리스크 비용(5~15%), 데이터 자산화 5개 영역으로 KPI·산식·외부 벤치마크를 정의하고 투자 타당성 검토 후 구축, 구축 후 지속적 ROI 실적관리를 강조함

---

- **Why Snowflake? 성능 테스트**
  - 테스트 조건: 원천 21,356,019건, 약 2.3GB
  - 기존 경로(3단계): S3–Glue ETL → 스테이징 저장 → DW 반영 = 18분 06초
  - Snowflake 경로(2단계): EC2–Airflow ETL → 스테이징→DW 원스탑 반영 = 15분 26초 (약 15% 우수)
  - 구성요소: EC2 + Airflow → S3 → Snowpipe → Staging Table → Stream/Task → Target Table → Dynamic Table. 일괄 로드·증분 적재 등 전사 확장 요건 충족

- **우리의 AX는 다르다 (2트랙 병행)**
  - 배경: 시스템별 개별 데이터 운영, 분석 환경 미구축 + AI 기술 발전 + 즉각적 가치 창출 필요
  - [1단계] Track A(데이터 플랫폼): Snowflake 기반 DW 구축 → 데이터 통합 → 마트/셀프 대시보드 → AI 활용 가능한 정형데이터 기반(AI Ready Data)
  - [1단계] Track B(AI 플랫폼): AWS Bedrock 기반 Gen AI 플랫폼(보안/권한/가드레일) → Vector DB·RAG 기반 업무지식 활용 → 현업 활용 확대·고도화
  - [2단계] AX 확장: '데이터 플랫폼 x Gen AI 인터페이스' — 비전문가의 고객 데이터 AI분석, AI 기반 메뉴 개발·상품믹스, 수요 예측·발주·재고, 매장 운영·손익/KPI 최적화

- **AX에서 가장 중요하게 보는 것 (Lessons Learned)**
  - 성과 영역 5개: 반복 인시 절감(목표 20~30%), 구매/재고/물류 비용 절감(2~5%), 매출 증대·방어(1~3%), 리스크 비용 절감(5~15%), 데이터 자산화(통합 데이터셋·재활용 지표·활용 부서 수)
  - 성과 산정 방식 예시: 인시 절감=업무 건수×기준 소요시간×AI 절감률, 비용 절감=대상 비용×개선률, 매출 효과=증분 매출+손실 방어 매출, 리스크 절감=리스크 관련 비용×감소율
  - 벤치마크 활용 원칙: 외부 사례 수치는 목표 설정 참고값, 자사 데이터 준비도·업무량·적용 범위에 따라 보수 조정, 수치보다 과제별 산정 기준 확보가 핵심
  - AX Master Plan 검증 항목: 기준 데이터 확보 여부, KPI 산식·현행값 정의, 투자비·운영비 대비 ROI 산정, 우선 추진 과제·목표값 확정

</details>

<details>

<summary>SESSION 5: 마케팅 빌리지 — AI와 DATA로 무장한 탑티어 기업들 (14:00~14:20)</summary>

- 회사–상호작용 계층(채널)–고객 사이에 에이전트가 개입하는 '새로운 세계의 마케팅' 구조 변화를 제시함
- 마케팅 AI 에이전트의 발전 단계를 L1(인사이트)~L5(실행)의 5단계로 정의 — 단순 답변에서 캠페인 시작·CRM 업데이트 같은 승인된 작업 '실행'까지 진화함
- SCI 고객 태그 체계: 총 14,162개 태그(Fact 11,326 + Segment 2,476 + Prediction 360)로 고객의 과거–현재–미래 행동을 이해·예측, 11개 도메인 일 20억 건 이벤트를 매일 학습·업데이트함
- 실환경 A/B 검증 성과: KB증권 CVR 1.5배 상승·CPC 44.2% 절감, 쿠팡 CTR 2.8배 상승·CPC 58% 절감

---

- **AI 에이전트 발전 5단계**
  - L1 인사이트 어시스턴트: 프롬프트 기반 답변·인사이트 생성 (예: 캠페인 성과 요약)
  - L2 컨텍스트 어시스턴트: 워크플로우 전반에서 대화·파일·데이터·지식 활용 (예: 세그먼트·이전 캠페인 결과 분석)
  - L3 계획 수립 에이전트: 마케팅 목표를 단계로 세분화하고 계획 조정 (예: 통합 캠페인 계획 수립)
  - L4 의사 결정 에이전트: 규칙·임계값에 따라 최적의 다음 조치 추천·선택 (예: 오디언스·오퍼·채널·예산 배분 우선순위)
  - L5 실행 에이전트: 승인된 작업 실행 (예: 캠페인 시작, CRM 업데이트, 영업팀 알림)

- **SCI 태그 체계 — 고객의 과거·현재·미래**
  - Fact Tag 11,326개: 앱 사용 일수, 체류 시간, 광고 클릭 이력, 매장 방문 횟수, 카테고리 구매 등 (과거)
  - Segment Tag 2,476개: 편의점 이탈 징후, 가격 민감 성향, 여행 관심 고관여, 프리미엄 소비 성향 등 (현재)
  - Prediction Tag 360개: 간편식 구매 확률, 마트 이탈 확률, 여행 예약 확률, 카테고리 첫구매 확률 등 (미래)
  - 예측 생성 예시: D-14 경쟁 편의점 앱 사용 증가 → D-7 체류 시간 증가 → D-3 관련 광고 클릭(Fact) → 비교 구매 성향·이탈 징후(Segment) → 7일 내 재방문 확률·30일 내 이탈 확률(Prediction)

- **SCI SUID 파이프라인**
  - 11개 도메인(커머스, 포스트백, 앱 사용성, 위치, 유저 프로필, DSP, SSP, CDP, 리워드, TV, 리퀘스트)의 일 20억 건 이벤트를 F.Raw로 정제, 단계별 특화 딥러닝으로 F-Tag → S-Tag → P-Tag 산출
  - F-Raw(무슨 일이 일어났는지) → F-Tag(행동 단위×시간 축×변화율의 구조화된 사실) → S-Tag(현재 상태) → P-Tag(12개 업종 7일 내 행동 확률 예측, 예: 7일 내 뷰티 구매 확률 73%)

- **실환경 A/B 검증 사례**
  - KB증권(2026.06.25~07.02): 동일 캠페인·소재·매체에서 SCI 타깃 vs 일반 DSP — CVR 23.04% vs 14.98%(1.5배), CPC 14.74원 vs 26.39원(44.2% 절감)
  - 쿠팡(2026.06.25~07.09): CTR 7.46% vs 2.64%(2.8배), CPC 5.90원 vs 14.14원(58% 절감)

</details>

<details>

<summary>SESSION 6: 마케팅 빌리지 고객 사례 — [IGAWorks] 차세대 SCI AI 기술을 활용한 고객 세그먼트 분석과 행동 예측 (14:50~15:20)</summary>

- "LLM은 답을 만들고, LBM은 다음 행동을 예측합니다" — LLM이 다음 단어를 예측하듯 LBM(Large Behavior Model)은 고객의 '다음 행동 확률'을 예측하는 모델임
- IGAWorks의 LBM인 WorksFM(국내 유일)은 3,400만 사용자·일 20억 건 행동 데이터를 학습, "7월에 일본 여행 갈 사람 5만 명 찾아줘" 같은 자연어 질의로 예측 기반 타깃 오디언스를 추출함
- CDP/CRM/DSP/GA4/APP/POS 등에 흩어진 접점 데이터를 Identity–Behavior–Prediction의 하나의 행동 타임라인으로 재구성하는 것이 LBM의 역할 — Bloomberg/Amazon/Meta/TikTok과 동일한 '시퀀스→임베딩→벡터 검색→의사결정→실행' 구조임
- SCI Data Alliance: Snowflake Data Clean Room에서 파트너 내부 데이터와 SCI 외부 행동 데이터를 비식별 ID 매칭으로 결합(원본 반출 없음) — 이탈 방지·잠재 고객 발굴·신규 사업으로 확장함

---

- **LLM vs LBM 비교**
  - LLM: 입력=텍스트, 학습 데이터=인터넷 텍스트, 예측 목표=Next Token, 출력=논리적으로 그럴듯한 응답
  - LBM: 입력=행동 데이터(14,162개 행동 태그), 학습 데이터=IGAWorks 행동 데이터, 예측 목표=Next Behavior, 대표 모델=WorksFM, 출력=행동할 확률(%), Self-Labeling으로 주 122억 건 학습 데이터 자동 생성
  - 출력 예시: LLM은 "오늘→날씨는→맑고…", LBM은 "앱 실행→상품 조회→장바구니→구매" 시퀀스

- **고객 여정 = 연결된 행동 시퀀스**
  - 여정 단계: Search(관심 표출)→Click(탐색)→View(상품 이해)→Cart(구매 의도)→Buy(전환)→Repeat(관계)
  - 문제: CDP·CRM·DSP·GA4·APP·POS·Survey 등 서로 다른 ID·테이블에 데이터가 분절됨 — 흩어진 행동을 하나의 타임라인으로 이어야 다음 행동이 보임

- **글로벌 동향 비교 (Global Synthesis)**
  - Bloomberg(금융 코퍼스→Terminal AI 의사결정), Amazon(쇼핑+광고→ROAS 최적화), Meta(Andromeda retrieval→Advantage+), TikTok(관심 그래프→Feed+Ads+Shop) — 영역은 달라도 Data→Identity→Embedding→Vector Search→Decision→Activation 구조는 동일함
  - IGAWorks: 11개 도메인 행동 / SCI+WorksFM / Vector Search / 예측 기반 오디언스

- **WorksFM 아키텍처 (행동에서 예측까지 하나의 엔진)**
  - 예시 질의 "7월에 일본 여행 갈 사람 5만 명 찾아줘"의 4단계 처리: 질문 의도 분해(관심사·지역·시기·인원) → F-Tag(실제 행동)/S-Tag(현재 관심·상태)/P-Tag(다음 행동 확률)로 사람 이해 → 3,400만 사용자 중 유사 고객 탐색 → 다음 행동 확률·유사도·관심 상승세 기준 상위 5만 명 선별

- **SCI Data Alliance (Snowflake Data Clean Room)**
  - 파트너 내부 데이터(구매 내역·멤버십·방문 빈도·프로모션 반응)는 유저의 외부 행동을 알 수 없다는 한계 — SCI 외부 데이터(3,400만 명의 11개 도메인 크로스 행동+예측)와 결합해 보완함
  - 안전한 연결·비식별 ID 매칭·원본 데이터 반출 없음. 이탈 방지 → 잠재 고객 발굴 → 신규 사업으로 확장

</details>

<details>

<summary>SESSION 7: Track 3 — AI 데이터 엔지니어링의 핵심: dbt 프로젝트와 시맨틱 뷰, Snowflake CoCo (16:30~17:00)</summary>

- Snowflake 데이터 엔지니어링 전체 스택을 Connect(수집) → Transform(변환) → Semantic Layer → Serve(서빙) 구조로 제시하고, AI 코딩 에이전트 Cortex Code(CoCo)가 전 과정을 지원함
- CoCo에는 데이터 엔지니어링용 내장 스킬 8종이 있음(dbt Projects, Dynamic Tables, Openflow, Snowpark, DCM, Verify, Lineage, Data Quality) — 파이프라인 배포·검증·계보·품질까지 에이전트가 자동화함
- 시맨틱 뷰는 dbt 프로젝트 안에서 `materialized='semantic_view'`로 정의하는 모델 — 업스트림 dbt 모델을 `ref()`로 참조하고, '매출' 같은 지표의 정의(예: 확정 주문만 집계)를 코드 한 곳에서 확정하는 계층임

---

- **Data Engineering in Snowflake (아키텍처 전체도)**
  - 최상단 거버넌스: Horizon Catalog — 메타데이터 관리, RBAC, 테이블/행/열 접근 제어, Discovery
  - Connect(수집): Openflow, Snowpipe & COPY, Snowpipe Streaming, Datastream + Zero-Copy Integration, Marketplace
  - Transform(변환): 선언형(SQL — dbt Projects, Dynamic Tables) + 프로그래밍형(Python/Spark — Snowpark, Snowpark Connect)
  - Semantic Layer: Semantic View, OSI(Open Semantic Interchange), OpenLineage
  - Serve(서빙): Agents(Snowflake CoCo), Analytics Tool, Applications
  - 하단 Interoperable Storage: Snowflake Tables, Apache Iceberg, Delta Tables × AWS/Azure/GCP
  - CoCo의 특징: Snowflake를 이해함, 컨텍스트 인지, 파이프라인 작업 자동화, 안전하고 거버넌스된 개발

- **데이터 엔지니어링을 위한 CoCo 내장 스킬 8종**
  - dbt Projects: 네이티브 dbt 프로젝트 배포 / Dynamic Tables: 파이프라인 생성·최적화·모니터링 / Openflow: 커넥터 배포·구성·진단 / Snowpark: UDF·저장 프로시저 배포
  - DCM Projects: 매니페스트 기반 선언적 인프라 관리 / Verify: dbt show/test로 변경 안전 검증 / Lineage: 계보·의존성 분석 / Data Quality: DMF 기반 스키마 수준 품질 모니터링

- **시맨틱 뷰 정의 예시 (dbt 프로젝트 내)**
  - `models/semantic/sv_sales.sql`에 `config(materialized='semantic_view')`로 선언, TABLES는 `ref('orders_enriched')` 등 업스트림 dbt 모델 참조 + PRIMARY KEY 지정
  - RELATIONSHIPS로 테이블 간 조인 관계 선언, DIMENSIONS와 METRICS(예: `total_revenue = SUM(CASE WHEN STATUS='F' THEN ORDER_AMOUNT END)`)를 정의
  - **"'매출'의 의미는 바로 여기서 정해집니다"** — 확정 주문(STATUS=F)만 매출로 집계한다는 비즈니스 규칙을 코드·주석으로 명시, 지표 정의를 시맨틱 뷰 한 곳에서 확정함

</details>
