---
layout: post
title: "WritingDrill_Rounds_12"
date: 2026-06-29
categories: Drill
tags: [Drill]
---


<script>
    window.MathJax = {
        tex: {
            inlineMath: [['$', '$'], ['\\(', '\\)']],
            displayMath: [['$$', '$$'], ['\\[', '\\]']],
            processEscapes: true
        }
    };
</script>
<script defer src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>


<style>
.easy-box { background: linear-gradient(135deg, #fff8e1 0%, #fef5e7 100%); border-left: 4px solid #d68910; border-radius: 8px; padding: 16px 20px; margin-bottom: 28px; }
.easy-box .easy-title { font-size: 16px; font-weight: 700; color: #b9770e; margin-bottom: 10px; letter-spacing: 0.5px; }
.easy-box p { font-size: 15px; line-height: 1.7; color: #3a3a3a; word-break: keep-all; margin: 0; }

.visual-container { background: #fff; padding: 24px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.05); border: 1px solid #e2e8f0; margin-bottom: 32px; }
.visual-header { display: flex; align-items: center; gap: 8px; font-size: 18px; font-weight: 800; color: #1a3a6c; margin-bottom: 20px; padding-bottom: 14px; border-bottom: 2px solid #e8edf5; }

.table-presentation { width: 100%; border-radius: 8px; overflow: hidden; border: 1px solid #1a3a6c; }
.tp-header { display: flex; background: #1a3a6c; color: white; font-weight: 700; text-align: center; font-size: 15px; }
.tp-header-col { flex: 1; padding: 14px 10px; border-right: 1px solid rgba(255,255,255,0.2); word-break: keep-all; display: flex; align-items: center; justify-content: center; }
.tp-header-col:last-child { border-right: none; }
.tp-row { display: flex; border-bottom: 1px solid #e2e8f0; background: white; }
.tp-row:last-child { border-bottom: none; }
.tp-row:nth-child(even) { background: #f8fafc; }
.tp-col { flex: 1; padding: 14px 10px; font-size: 14.5px; text-align: center; border-right: 1px solid #e2e8f0; word-break: keep-all; color: #2d3748; display: flex; align-items: center; justify-content: center; }
.tp-col:last-child { border-right: none; }

.quote-card { background: linear-gradient(135deg, #f7f4ec 0%, #faf8f1 100%); border-radius: 12px; padding: 26px 28px; border-left: 5px solid #c0392b; box-shadow: 0 4px 12px rgba(0,0,0,0.06); margin-bottom: 32px; }
.quote-card .quote-header { font-size: 14px; font-weight: 700; color: #c0392b; letter-spacing: 2px; margin-bottom: 14px; }
.quote-card .quote-ko { font-size: 18px; line-height: 1.6; color: #1a1a1a; font-weight: 600; word-break: keep-all; margin: 0; }

.split-2 { display: flex; align-items: stretch; gap: 12px; margin-bottom: 20px; }
.split-2-card { flex: 1; padding: 24px 20px; border-radius: 12px; background: #f8fafc; border: 1px solid #e2e8f0; text-align: center; font-size: 15px; font-weight: 700; color: #2d3748; line-height: 1.7; word-break: keep-all; }
.split-2-connector { font-size: 28px; font-weight: 900; color: #4a5568; display: flex; align-items: center; justify-content: center; }

.split-3 { display: flex; gap: 10px; margin-bottom: 20px;}
.split-3-item { flex: 1; padding: 16px 10px; border-radius: 12px; text-align: center; background: #f8fafc; border: 1px solid #e2e8f0; }
.split-3-item.c1 { background: #fff5f5; border-top: 4px solid #fc8181; }
.split-3-item.c2 { background: #fffaf0; border-top: 4px solid #fbd38d; }
.split-3-item.c3 { background: #f0fff4; border-top: 4px solid #9ae6b4; }
.split-label { font-size: 12px; color: #718096; margin-bottom: 6px; font-weight: 700; }
.split-val { font-size: 15px; font-weight: 800; color: #2d3748; line-height: 1.4; }

.dueum-box { background-color: #1a3a6c; color: #ffffff; border-radius: 8px; padding: 16px 20px; margin-top: 8px; margin-bottom: 24px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); }
#previewText .dueum-box p, .dueum-box p { font-size: 16.5px !important; line-height: 1.7 !important; color: #ffffff !important; word-break: keep-all !important; margin: 0 !important; font-weight: 700 !important; }
</style>

### [소프트웨어공학] 리만(Lehman)의 SW변화의 원리

**[정의]**

- SW에 대해 추가, 수정 개발이 이루어지게 되는데 그 과정에서 해당 SW는 어떤 일정한 패턴을 보이며 변화하고 진화하다는 논리

**[핵심/키워드]**

* E-Type 변화원리
* 8대원리 
- 지속적인 변화, 증가하는 복잡성, 자기 조정, 조직적 안전성, 친화적 유지, 지속적인 성장, 점진적 쇠퇴, 피드백 시스템

### [소프트웨어공학] SW 기술부채

**[정의]**

소프트웨어 설계·개발·테스트·배포 전 과정에서 장기적 관점의 솔루션 대신 짧은 기간 내 임시방편의 해법을 선택해 차후 발생가능한 추가적 위험비용

**[핵심/키워드]**

&lt; 발생원인 &gt;
- 최적화되지 않은 코드, 문서화 부족, 테스트 미비
&lt; 유형 &gt;
- 의도적, 비의도적, 아키텍처적, 코드기반, 테스트 부족, 문서화 부족, 의존성
&lt; 해결방안 &gt;
* 기술적 해결 : 코드 리팩토링, 자동화 테스트, 의존성 관리, 아키텍처 개선
* 프로세스 개선 해결 : 프로세스, 리뷰 강화, Agile, Devops
* 조직 및 문화 해결 : 인식 개선, 혁신 투자, KPI 도입
* 전략적 해결 : 로드맵, 점진적 개선, 외부 컨설팅
&lt; AI 기술부채 &gt;
- AI 측면 기술부채

### [소프트웨어공학] 프로토타입 (Prototype) 모델

**[정의]**

최종 제품을 개발하기 전에 시제품(Prototype)을 먼저 제작하여 사용자 피드백을 반영하는 SDLC 모델

**[핵심/키워드]**

&lt; 특징 &gt;
- 사용자 중심, 피드백 제공
&lt; 절차 &gt;
- 요구분석 > 포로토타입 개발 > 프로토타입 검토 > 상세 개발 > 설치
&lt; 유형 &gt;
* 개발목적 : 탐색적, 진화적, 실험적, Rapid
* 개발방식 : 스레드, 수직, 수평
*  SDLC 활용 : 나선형, 반복형

### [소프트웨어공학] 오버로딩 (Overloading)

**[정의]**

동일한 이름의 함수로 정의 하되 인자의 값을 형태나 개수를 다르게 하는 다형성 기법

**[핵심/키워드]**

* 객체지향 다형성 특징, 동적 메소드 실행
* 함수 /메소드 이름 동일, 매개변수 타입, 개수 다름, 함수 반환 타입 무관, static 메소드 가능
* 유형 (함수 오버로딩, 메소드 오버로딩, 생성자 오버로딩)
* 오버라이딩

### [소프트웨어공학] 오버라이딩 (Overridng)

**[정의]**

부모 클래스의 함수를 자식 클래스에서 재정의하여 사용하는 다형성 기법

**[핵심/키워드]**

* 객체지향 다형성 특징, 상속, 동적 메소드 실행
* 함수 / 메소드 이름 동일, 매개변수 타입, 순서, 개수 동일, 리턴 타입 동일, static 메소드 불가
* 오버로딩

### [소프트웨어공학] 인수테스트 주도 개발 (Acceptance Test Driven Development, ATDD)

**[정의]**

테스트로부터 시작해서 구현을 마무리 짓는 TDD의 범위를 소스코드 수준에서 인수 테스트 수준까지 확장하여 고품질의 SW를 생산하는 개발방법

**[핵심/키워드]**

&lt; 특징 &gt;
- 인수 테스트, 협업강조, 자동화, BDD 연계
&lt; 단계 &gt;
- Discuss, Distill, Develop, Demo, TDD Cycle (Red, Green, Clean)

* TDD, BDD, 인수테스트

### [소프트웨어공학] 애자일 추정 (Agile Estimation)

**[정의]**

애자일 프로젝트에서 프로젝트, 릴리즈 또는 스프린트의 규모를 산정하기 위해 Product Backlog의 Story Point를 기반으로 노력을 추정하는 절차/기법

**[핵심/키워드]**

&lt; 특징 &gt;
- 상대적 크기, 협업, 불확실성
&lt; 단계 &gt;
- 항목 수집 > 팀 논의 및 비교 > 추정기법 적용 > 합의 도출 > 결과 반영 및 조정
&lt; 기법 &gt;
 (1) 스토리 포인트 (Stroy point) : 사용자 스토리 복잡도, 노력, 불확실성 상대적 평가
 (2) 플래닝 포커 (Planning Poker) : 팀원이 각자 제시, 합의 도출
 (3) 티셔츠 사이즈 (T-Shirt Sizing) : S, M, L, XL 등 크기로 직관적 측정
 (4) 퍼펙트 신뢰도 측정 (Confidence Interval Estimation) : 예상 범위 3~5점 추정
 (5) 유사 조건 (Affinity Estimation) : 유사 작업 그룹화 크기 비교
 (6) 일정기반 (Bucket System) : 미리 정의된 범주 작업
 (7) 시간기반 (Time based Estimation) : 실제 소요 시간 
 (8) 점 투표 (Dot Voting) : 직접 항목에 점 부여, 우선순위 및 상대적 크기 결정

### [소프트웨어공학] 린 (Lean) 개발방법론

**[정의]**

낭비(불필요한 작업)를 최소화하고 효율성을 극대화하는 방식으로, Toyota 생산시스템에서 시작된 LEAN 제조 원칙을 소프트웨어 개발에 적용한 방법론

**[핵심/키워드]**

&lt; 특징 &gt;
- 낭비 최소화, 지속적 개선, 고객 가치 중심
&lt; 7대 낭비 요소 &gt;
- 재작업, 재학습, 가외작업, 작업 전환, 결함 및 품질 문제, 지연 및 대기시간, 이관 및 커뮤니케이션 손실
&lt; 7개 가치 &gt;
- 낭비제거, 배움증폭, 늦은 결정, 팀에 권한 위임, 빠른 납품, 통합성 구축, 전체 최적화

### [소프트웨어공학] SRE (Site Reliability Engineering)

**[정의]**

대규모 서비스나 인프라의 신뢰성, 안정성을 달성하기 위해 고도의 SW기술을 적용하여 운영관리하는 공학기법

**[핵심/키워드]**

&lt; 목표 &gt;
- 서비스 안전성 (Reliability), 확장성 (Scalability), 운영 효율성 (Efficiency) 극대화
&lt; 핵심요소 &gt;
- 측정 및 모니터링, 용량 계획, 변경 관리, 긴급 대응, 문화 및 조직 정착
&lt; 측정 지표 &gt;
- SLI (Service Level Indicator), SLO (Service Level Objective), SLA (Service Level Agreement)
&lt; 적용원칙 &gt;
- 운영 자동화, 모니터링 및 로깅, 에러 버짓 (Error Budget), 확장 가능한 탄력적 인프라, 블레임리스 포스트모템, 카오스 엔지니어링

* Devops 구현 핵심역할

### [소프트웨어공학] Spring Cloud

**[정의]**

마이크로 서비스 아키텍처(MSA) 환경에서 서비스간 통신, 구성관리, 부하분산, 장애복구 등을 쉽게 구현할 수 있도록 지원하는 Spring기반 프레임워크

**[핵심/키워드]**

&lt; 특징 &gt;
- MSA 지원, 중앙설정관리, 장애복구
&lt; 기능 &gt;
- 서비스 등록 및 디스커버리, API Gateway, 구성 관리, 로드 밸런싱, 회로 차단, 분산 트랜잭션 및 모니터링, 서비스 배포 및 컨테이너 오케스트레이션, 모니터링 및 운영관리

### [소프트웨어공학] 속성기반 설계 (Attribute Driven Design, ADD)

**[정의]**

만족 돼야할 품질 속성을 바탕으로 분할 과정을 진행해 나가면서 SW 아키텍처를 만드는 방법

**[핵심/키워드]**

&lt; 특징 &gt;
- 품질속성 중심, 반복 설계
&lt; 절차 &gt;
1\. 시스템 분할 > 2. 선택된 모듈 정제 (아키텍처 드라이브 선택) > 3. 재귀 및 통합

### [소프트웨어공학] 아키텍처 문서화 (Architecture Documentation)

**[정의]**

SW 아키텍처의 구조, 구성요소, 상호작용, 품질속성을 문서화하여 체계적으로 정리하는 과정

**[핵심/키워드]**

* 핵심설계 결정사항 설명, 서로 다른 관심사 중심 접근 고려
&lt; 절차 &gt;
1\. 뷰집합 확보 > 2. 뷰 문서화 > 3. 뷰 통합 > 4. 뷰 표현
&lt; 문서화 방법 &gt;
(1) Perry and Wolf's Model : 요소, 표현법, 근거
(2) Shaw and Garlan's Model : 컴포넌트, 커넥터, 패턴
(3) 4+1 View : 논리, 구현, 프로세스, 배포, 유스케이스
(5) Siemens Four View Model : 개념, 모듈, 실행, 코드, H/W 아키텍처
(6) ISO/IEC 42010 : 이해관계자, 관점, 모델, 설계결정

### [소프트웨어공학] ATAM (Architecture Tradeoff Analysis Method)

**[정의]**

다양한 품질속성 (성능, 신뢰성, 보안 등)의 상충관계(Trade off)를 분석하여 아키텍처의 품질을 평가하는 기법

**[핵심/키워드]**

* 품질속성, Trade off, 공통성과 가변성 평가 
&lt; 특징 &gt;
- SAAM 발전, Trade off, 이해관계자 참여 필수
&lt; 단계 &gt;
1\. 구축 및 프로젝트 준비 &gt; 2. 소개 및 조사와 분석 &gt; 3. 평가 진행 &gt; 4. 후속 조치 및 보고서 작성
&lt; 평가단계 &gt; 소조테보
2\. 소개 (1 소개, 2 비즈니스 동인, 3 아키텍처 소개)
3\. 조사 및 분석 (4. 접근법 식별, 5. 품질속성 유틸리티 트리, 5. 접근법 분석)
4\. 테스트 (7. 브레인스토밍과 시나리오 우선순위 결정, 8. 분석 반복)
5\. 보고 (9. 결과발표)
&lt; 한계 / 개선 &gt;
* 한계 : 시간 소요, 주관적, 초기 적용 어려움, 경제성 결여
* 개선 : 자동화도구, 정량적 평가, Mini-ATAM, CBAM

### [소프트웨어공학] 람다 아키텍처 (Lambda Architecture)

**[정의]**

실시간 데이터 처리와 배치 데이터 처리를 결합하여 대용량 데이터 (Big Data)를 효율적으로 처리하는 아키텍처

**[핵심/키워드]**

&lt; 특징 &gt;
- 실시간 + 배치, 확장성, 고가용성, 내결함성
&lt; Layer &gt;
1\. 배치 레이어 (Batch Layer) : 주기적 처리, Hadoop, Spark, Flink
2\. 스피드 레이어 (Speed Layer) : 실시간 처리, Storm, Kafka
3\. 서빙 레이어 (Serving Layer) : 빠르게 조회, Cassandra, HBase

* Kappa Architecture

### [소프트웨어공학] 서버리스 아키텍처 (Serverless Architecture)

**[정의]**

서버단에서 로직이나 상태를 관리하지 않고 실행에 필요한 하드웨어 자원의 배분 및 할당을 클라우드에서 동적으로(dynamically) 관리해주는 클라우드 컴퓨팅의 실행 모델

**[핵심/키워드]**

* 클라우드 인프라 활용, 동적 관리, stateless, Function as a service
&lt; 구성요소 &gt;
* FaaS : 독립적 함수 실행
* API Gateway : 클라이언트 요청 처리, 함수 호출 라우팅
* 스토리지 서비스 : 데이터 저장
* 데이터베이스 : 데이터 저장 및 관리
* 이벤트 트리거 : 이벤트 발생 시 함수 실행
* 보안 및 인증 : 인증 및 권한 관리

### [소프트웨어공학] 헥사고날 아키텍처 (Hexagonal Architecture)

**[정의]**

응용 프로그램의 핵심 비즈니스 로직 (Core Logic)과 외부 인터페이스를 명확하게 분리하는 설계방식

**[핵심/키워드]**

* 포트, 어댑터, 클린 아키텍처의 일반화
&lt; 특징 &gt;
- 외부 분리, 테스트 용이, 도메인 중심 설계 (DDD), MSA
&lt; 레이어 &gt;
- Application Core : 비즈니스 로직, Usecase, Entity
- Ports : 인터페이스 역할, Input, Output
- Adapter : 구현 및 외부 연결, Driving, Driven
- External System : 상호작용 외부 시스템, DB, API, UI

### [소프트웨어공학] RFP (Request For Proposal)

**[정의]**

발주자가 정보 시스템에 대한 요구사항을 구체적으로 정리하여 공급업체에 참여를 공식적으로 제안하는 문서

**[핵심/키워드]**

&lt; 특징 &gt;
- 공식적 입찰 문서, 구체적 요구사항, 경쟁 입찰 가능, 최적의 공급업체 선정
&lt; 주요 항목 &gt;
1\. 사업의 개요 (배경, 내용, 범위, 기대효과)
2\. 프로젝트 일정 (제출 마감일, 발표일정, 선정 발표일, 개략적 추진 일정)
3\. 정보 요구내역 (서비스 제공자, 조직 및 인력, 추진내역, 보유기술)
4\. 기술적 환경 (현재 기술 현황, 시스템 아키텍처)
5\. 관련 요구사항 (제안 목차, 핵심인력 및 참고자료, 형식 및 제출부수, 제출장소, 질의문의처)
&lt; 작성원칙 &gt;
- 명확한 요구사항, 공정한 평가기준, 일관된 양식, 사업 범위 및 책임 명확화

### [소프트웨어공학] AI 개발 생명주기 (AI Development Life Cycle, AI DLC)

**[정의]**

데이터의 수집과 처리, 학습의 결과물로서 AI 모델, 그리고 AI 모델을 기반으로 다양한 지능적 기능을 수행하는 AI 시스템을 구현하는 일련의 과정

**[핵심/키워드]**

&lt; AI 개발 생애주기 단계 &gt; - OECD 정의 기반
* 개발 계획 및 설계 → 데이터 수집 및 처리 → 모델 구축 및 조정 → 테스트, 평가, 검증 → 배포 및 제공 → 운영 및 모니터링 → 폐기 및 해체
&lt; AI 개발 생애 주기별 SW역할 &gt;
1\. 데이터 수집 : 원천 데이터 추출, 대용량 저장 (Hadoop)
2\. 데이터 전처리 : 데이터 정제, 형식변환 (Apache Airflow)
3\. 모델 개발,학습 : AI 모델 구현 및 훈련 (TensorFlow, PyTorch)
4\. 모델 최적화 : 모델 경량화, 호환성 확보 (ONNX, TF-Lite)
5\. 모델 추론 : API 서빙, 모델 호스팅 (ONNX Runtime, TensorFlow)
6\. 배포 및 운영 : 버전,성능관리, 모델드리프트 감지 (Docker, Kubernetes)
7\. 애플리케이션 개발 : App통합, 프론트엔드-백엔드 연계

### [소프트웨어공학] 상주감리

**[정의]**

현장에 상주하거나 주기적으로 투입되는 상주감리원이 사업관리 지원, 자문 등을 수행하는 감리

**[핵심/키워드]**

* 현장 상주, 주기적 투입
* 3단계 감리 시 요구사항 감리 생략 가능 → 상주감리원이 요구사항 점검
* 대상 : 대기업 참여 제한, 높은 위험 난이도 사업, 40억 미만
* 상주감리원 자격 : 20억 이상 감리 참여 3회이상, PM이나 QA 3년 이상

* PMO

### [소프트웨어공학] ISO/IEC 25019 : 2023

**[정의]**

기존 ISO/IEC 25010 품질모델을 보완하고, 정보시스템 및 IT서비스의 사용중 품질을 평가하기 위한 기준을 강화한 표준

**[핵심/키워드]**

* 품질-사용 모델, 사용자 맥락 중심, 이해관계자 중심, 비기능적 품질 강화
&lt; 핵심특성 &gt;
* 효용성, 위험감소, 수용가능성
&lt; 특성 &gt;
* 효용성 (사용성, 접근성, 적합섷)
* 위험감소 (경제적 위험감소, 환경 및 사회적 위험감소, 간강 위험감소, 생명 안전보장)
* 수용가능성 (사용자 경험, 신뢰성, 규정준수)

* ISO/IEC 25010

### [소프트웨어공학] CMMI3.0 (Capability Maturity Model Integration 3.0)

**[정의]**

조직의 프로세스 성숙도를 평가하고 성과를 개선하기 위한 최신 프레임워크로, 보안(Security), 안전(Safety), 데이터(Data), 가상(Virtual )환경 등 새로운 도메인을 추가하여 확장된  CMMI 모델

**[핵심/키워드]**

* CMMI 2.0 + 새로운 도메인 추가
&lt; 도메인 &gt;
* 기존 (Core, DEV, SVC, SPM)
* 신규 (SEC, SAF, PPL, DAT, VRT)
&lt; 구성요소 &gt;
* Category Area : 2.0 동일, Doing, Managing, Enabling, Improving
* Capability Area : 12개 하위 Practics 그룹
* Practices (31개) : Core (17개), 도메인별 특정 (14개)
* Domain (8개)

### [소프트웨어공학] 코드스멜 (Code Smell)

**[정의]**

유지보수성이 낮거나 개선이 필요한 비효율적인 코드 패턴

**[핵심/키워드]**

* 비효율적, 개선 필요
&lt; 주요 유형 &gt;
* 중복된 코드, 긴메소드, 큰클래스, 너무 많은 인수, 두 가지 이상의 이유로 수정되는 클래스, 다른 클래스를 지나치게 사용, 그룹 중복, 기본 데이터 타입 선호
&lt; 해결 &gt;
* 리팩토링

### [소프트웨어공학] 리팩토링 (Refactoring)

**[정의]**

코드의 기능은 유지하면서 구조를 개선하는 작업

**[핵심/키워드]**

* 기능 유지, 구조 개선, 코드 스멜, 기술부채 등 해결
&lt; 주요 유형 &gt;
* 결합도 측면 : Move Method, Move Field, Extract Class
* 응집도 측면 : Pull Up Method, Pull Up Field, Push down Method, Push down Field, Inline Class
* 가독성 측면 : Rename
&lt; 활용 및 효과 &gt;
* TDD, 유지보수 향상

### [소프트웨어공학] ITIL v4.0의 서비스 가치 시스템 (Service Value System, SVS)

**[정의]**

다양한 조직 요소와 활동을 통합 및 조정하고 강력하고 통일되며 가치에 집중하는 방향성을 조직에 제시하여 가치를 지속적으로 창출하는 시스템

**[핵심/키워드]**

* 지속적 가치 창출, ITIL
&lt; 구성 &gt;
* 기회 / 수요, 서비스 가치사슬, 가이드 원칙, 거버넌스, 관리 실행, 지속적 개선, 가치
&lt; 서비스 가치 사슬 &gt;
* 계획, 참여, 설계 및 전환, 획득 및 구축, 운영, 개선
&lt; 가이드 원칙 &gt;
* 가치 중심, 현재 상태 시작, 반복적 피드백, 협업 및 투명성, 전체론적 사고, 단순 및 실용적, 자동화 활용
&lt; 프랙티스 &gt;
* 일반관리 실행 (14개), 서비스 관리 실행 (17개), 기술관리 실행 (3개)

### [소프트웨어공학] 인공지능(AI) 서비스 도입 사업 대가산정 (2025년 8월 개정 기준)

**[정의]**

인공지능(AI) 서비스 도입 시 서비스 가격표 또는 견적서에 제시된 이용료(구독료)와 투입공수방식의 전문작업비에 따라 대가를 산정하는 방식

**[핵심/키워드]**

&lt; 도입 사업비 &gt;
* 서비스 총이용료 + 커스터마이징 작업비용 + 구축개발비용
&lt; 절차 &gt;
1\. 사전준비 &gt; 2. 이용료 계산 &gt; 3. 커스터마이징 작업비용 &gt; 4. 서비스 도입 산정비 선정
&lt; 사업유형 &gt;
* 단순 AI 서비스 제공사업
* 커스터 마이징 기반 사업 (기본 커스터마이징, AI 데이터 구축 커스터마이징, AI 모델 커스터마이징)
* 시스템 통합 기반 사업
&lt; 비용구성 &gt;
* 서비스 이용료
* 커스터 마이징 작업 비용 (요구사항 분석 및 설계, 데이터 구축, 모델 구현 및 학습, 서비스 검증 및 안정화)
* 시스템 통합 및 기능 개발비 (FP)

* FP 방식 (정량) + SNAP (정성)

### [소프트웨어공학] FMEA (Failure mode effective analysis)

**[정의]**

제품 및 프로세스의 가능한 문제점, 원인을 사전에 예측/위험도 평가하여 사전 예방이 가능하도록한 기법

**[핵심/키워드]**

* 고장원인 개입 에방, 영향 분석, 위험도 평가 (RPN), HW 중심, 귀납적 (Bottom Up)
&lt; 절차 &gt;
1\. 분석 대상 정의 > 2. 기능 식별 및 고장모드 > 3. 고장 영향 > 4. 고장원인 > 5. 위험 우선순위 평가 > 6. 개선조치 수립 및 실행 > 7. 개선 효과 검토 및 지속적 업데이트
&lt; 분류 &gt;
* System FMEA, Design FMEA, Product FMEA
< RPN, 위험우선순위 >
* 심각도 x 발생도 x 검출도

* FTA, HAZOP, ETA

### [소프트웨어공학] HAZOP (HAZard OPerability)

**[정의]**

시스템, 공정, 또는 제품에서 잠재적인 위험(Hazard)과 운전문제(OperabilityIssues)를 사전에 분석하는 기법

**[핵심/키워드]**

* 위험과 운전문제, 가이드 워드, 귀납적 (Bottom Up), HW 중심, 팀기반 평가
&lt; 가이드 워드 &gt;
* 다른 상황 예측, 예상 못한 위험 발견
* 예시 (More, Less, No, None, Reverse, As well as, Other than)
&lt; 단계 &gt;
1\. 시스템 정의 및 범위 설정 > 2. 노드 설정 > 3. 가이드 워드 적용 > 4. 이상상황 분석 및 영향 평가 > 5. 원인 분석 및 개선 조치 > 6. 문서화 및 지속적 개선
&lt; 결과 도출방식 &gt;
* 편차, 이탈, 원인, 결과, 보호조치, 개선조치

* FTA, FMEA, ETA

### [소프트웨어공학] STPA (System-Theoretic Process Analysis)

**[정의]**

STAMP를 기반으로 하는 위험분석기법, 시스템 생명 주기 전 과정에 걸쳐 존재하는 잠재적 위험과 발생원인을 시스템의 상위수준에서 분석하는 기법

**[핵심/키워드]**

* STAMP, 시스템 기반, 사전 예방
&lt; 절차 &gt;
1\. 사고 및 위험 정의 > 2. Control Structure 도출 > 3. UCA 도출 > 4. 원인 시나리오 도출
&lt; UCA &gt;
* 부재, 부적절, 제공시간 및 순서, 지속시간
&lt; 활용 &gt;
* ISO 26262, FDA 의료 디바이스, 국민 생명과 안전 영향 SW

* CAST

### [소프트웨어공학] SNAP (Software Non-functional Assessment Process)

**[정의]**

기능 중심의 FP(Function Point) 방식이 측정하지 못하는 비기능적 요구사항(성능, 보안, 데이터베이스 등)의 크기를 정량적으로 측정하는 기법

**[핵심/키워드]**

* AI 규모 산정 시 FP 단점 보완, 정성적, ISO/IEC/IEEE 32430: 2025, 비기능 중심
&lt; 카테고리 &gt;
* Data Operation, Interface Design, Technical Environment, Architecture
&lt; 측정절차 &gt;
* 기술 요구사항과 서브 카테고리 매핑 > 서브 카테고리 측정 규칙 적용 > 기술규모 합산

### [소프트웨어공학] CAST (Causal Analysis based on System Theory)

**[정의]**

STAMP 이론 기반으로 시스템 전체 관점에서 사고 발생 이후 근본 원인을 분석하여 재발 방지를 도모하는 사고 원인 분석 기법

**[핵심/키워드]**

* STAMP, 근본원인 조치 (사후 최소화), 전조징후(Precursor) 및 기여요인(Contributing factor)
&lt;절차&gt; 
* 기본정보 수집 > 안전 컨트롤 스트럭처 모델링 > 손실에 대한 각 컴포넌트 분석 > 컨트롤 스트럭처 결함 식별 > 개선 프로그램 생성수립

* STPA

### [테스트] 테스트 완료 조건 (Test Completion Criteria)

**[정의]**

Test를 종료할 시점을 결정하기 위해 기준이 되는 조건을 설정하는 작업

**[핵심/키워드]**

* 종료시점, 목표 달성, 테스트 계획서 명시
&lt; 완료조건 &gt;
* 완전성, 목적, 테스트 기준, 테스트 커버리지, 테스트 리스크, 테스트 스케줄

### [테스트] 테스트 오라클 (Test Oracle)

**[정의]**

테스트를 수행한 결과가 참인지 거짓인지를 판단하기 위해서 미리 정의된 참 값을 대입하여 비교하는 기법 및 활동

**[핵심/키워드]**

* 미리 정의된 참 값 대입
&lt; 구성요소 &gt;
* 입력값, 예상결과, 실제결과, 비교 매커니즘
&lt; 유형 &gt;
* 참 오라클, 완전 오라클, 샘플링 오라클, 휴리스틱 오라클, 일관성 검사 오라클, 자동 생성 오라클
&lt; 한계 &gt;
* 완전 오라클 구현 불가능, 비기능 요구사항 검증 어려움, 비결정적 결과 적용 어려움
&lt; 개선 &gt;
* 휴리스틱 및 머신러닝 기반, 샘플링 오라클, 일관성 검사 오라클, 자동화 연계, 이중화 검증 시스템

### [테스트] Record and Replay

**[정의]**

사용자의 행동 (입력 이벤트)을 기록(Record)하고 동일한 동작을 자동으로 반복 실행(Replay)하는 테스트 자동화 기법

**[핵심/키워드]**

* 입력이벤트 기반, Record, Replay, 임베디드 테스팅
&lt; Record &gt;
1\. 캡쳐 시작 > 2. 이벤트 후킹 > 3. 이벤트 송신 > 4. 이벤트 저장
&lt; Replay &gt;
2\. 재수행 시작 > 6. 이벤트 검색/변환 > 7. 이벤트 전송 > 8. 이벤트 전달 . 9. 결과 전달

### [테스트] 리뷰(Review)

**[정의]**

소프트웨어 실행 없이 코드, 문서, 설계 등을 검토하여 오류를 찾고 개선하는 프로세스

**[핵심/키워드]**

* 정적 테스트, ISO 20246, 공식/비공식
&lt; 특징 &gt;
- 실행없음, 조기 오류 발견, 문서화 가능
&lt; 유형 &gt;
* 비공식 리뷰, 워크스루, 기술리뷰, 인스펙션, 감사
&lt; 적용기법 &gt;
* Ad-hoc (비구조적, 독립수행, 비공식, 코드리뷰)
* 체크리스트 (체크리스트기반, 인스펙션, 기술리뷰)
* 시나리오 (구조적 지침, 특정결함 식별, 워크스루)
* 관점기반 (이해관계자 관점, 동일 결함 감소, 기술리뷰)
* 역할기반 (역할관점, 특정 역할가능, 인스펙션, 감사)

### [테스트] 인스펙션 (Inspection)

**[정의]**

프로그램을 실제로 실행해보지 않고 소프트웨어 개발단계에서 산출되는 결과물을 동료가 결함발견을 목적으로 검토하는 방법

**[핵심/키워드]**

&lt; 특징 &gt;
* 공식적, 사전준비 필수, 결함문서화, 역할기반
&lt; 유형 &gt;
* 시스템 설계, 상세설계, 코드 인스펙션, 테스트 인스펙션, 프로세스 인스펙션
&lt; 참가자 &gt;
* 주재자, 개발자, 제출자, 기록자, 검토자
&lt; 절차 &gt;
1\. 계획 > 2. 사전 교육 > 3. 준비 > 4. 인스펙션 회의 > 5. 수정 > 6. 후속조치
&lt; 원칙 &gt;
* 체크리스트 사전 작성, 5명 이내, 2시간 이내, 산출물만 비판, 오류해결 시도 금지, 반드시 기록 남기고 후속 조치 수행

### [테스트] 회귀테스트 (Regression)

**[정의]**

프로그램에 수정이나 확장이 가해진 후 변경 부분 뿐만 아니라 기존 기능도 같이 테스트를 수행하여 오류사항들을 검출해내는 테스트 기법

**[핵심/키워드]**

* 변경부분 + 기존기능 테스트, 테스트 자동화, 다양한 테스트 레벨, Ripple Effect, Side Effect
&lt; 단계 &gt;
1\. 변경사항 분석 > 2. 테스트케이스 선택 > 3. 회귀테스트 수행 > 4. 테스트 결과 검토 > 5. 결함 수정 및 재테스트
&lt; 유형 &gt;
* Retest All, Selective, Priority

### [테스트] 분류트리 (Classification Tree) 테스트

**[정의]**

테스트대상 시스템의 입력조건을 분류하고, 이를 트리구조로 표현하여 테스트케이스를 생성하는 테스트 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 시각적 표현, 트리 (Tree) 구조, 체계적 테스트 설계, 테스트케이스 최적화, 명세기반 / 경험기반
&lt; 단계 &gt;
1\. 파라미터 결정 > 세부 트리 구성 > 3. ID 부여 > 4. 테스트케이스 작성 > 5. 유효/비유효 분기점 설정 > 6. 테스트 수행 및 결과 분석

### [테스트] 탐색적 테스트 (ExploratoryTest)

**[정의]**

테스트 설계, 테스트 수행, 테스트 계획, 테스트 기록 및 학습을 동시에 진행하는 휴리스틱(Heuristic) 테스팅 접근법

**[핵심/키워드]**

&lt; 특징 &gt;
* 차터 기반, 사전 테스트케이스 없음, 계획과 수행이 동시 진행, 경험과 직관
&lt; 테스트 구성&gt;
* Test Charter (목표와 범위설정), Time Boxing (한정된 시간), Test Note (결함기록), Debriefing (결과분석, 공유)
&lt; 단계 &gt;
1\. 테스트 준비단계 (테스트 리더) > 2. 테스트 진행 (세션단위 실행) > 3. 테스트 기록 및 공유 > 4. 다음 세션 여부 판단

### [테스트] E2E 테스트 (End to End Test)

**[정의]**

전체 시스템이 요구사항에 맞게 동작하는지 애플리케이션의 모든 구성요소를 처음부터 끝까지 테스트하는 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 실제 사용자 관점, 전체 시스템, 시나리오 기반, 자동화
&lt; 장점 &gt;
* 시스템 전체 문제 발견 가능, 실제 사용자 경험 보장
&lt; 단점 &gt;
* 느린 속도와 많은 리소스, 테스트케이스 복잡, 관리 어려움

### [테스트] 몽키 테스트 Monkey Test)

**[정의]**

무작위 입력(Random Input)을 사용하여 시스템의 예기치 않은 오류를 발견하는 테스트 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 무작위, 즉흥적, 비정형 (Adhoc) 테스트, 자동화, 안정성 테스트, 시스템 테스트, 비기능 테스트
&lt; 유형 &gt;
* Dumb Monkey, Smart Monkey, Brilliant Monkey

### [테스트] 사용성 테스트 (Usability Test)

**[정의]**

사용자가 제품 (웹사이트, 애플리케이션 등)을 쉽게 이해하고 효율적으로 사용할 수 있는지 평가하는 테스트 기법

**[핵심/키워드]**

&lt; 방법론 &gt;
* 정성적, 정량적 탐색적
&lt; 정성적 &gt;
* 직접관찰, 인터뷰, 생각하는 소리기법, 페이퍼목업, 컨텍스트기반 테스트
&lt; 정량적 &gt;
* A/B 테스트, 아이 트래킹, 클릭분석, 스크린 목업, 탭 테스팅
&lt; 탐색적 &gt;
* 카드소팅, 프로토타입 테스트
&lt; 절차 &gt;
* 목표 설정 > 사용자 선정 > 시나리오 작성 > 환경 구축 >  실행 > 결과분석 > 개선적용 > 최종 보고
&lt; 진행인원 &gt;
* 평가 진행자, 기록담당, 녹화담당, 관찰자

### [테스트] 리스크기반 테스트 (Risk based Test)

**[정의]**

비즈니스, 기술 상의 위험을 정량적으로 측정하여 우선순위가 높은 부분에 주어진 테스팅 자원을 집중, 전체적인 영향을 줄이기 위한 테스트 전략

**[핵심/키워드]**

&lt; 특징 &gt;
* 효과성, 효율성 극대화, 우선순위, 자원 최적화
&lt; 절차 &gt;
1\. 테스트 진행 계획 > 2. 리스크 식별 > 3. 정성 분석 > 4. 정량 분석 > 5. 대응 계획 > 6. 리스크 추적
&lt; 활용 &gt;
* ISO/IEC TS 42119-2

### [테스트] 글로벌화 테스트 (Globalization Test)

**[정의]**

제품의 고유기능 및 성능, 컨텐츠 외에 다양한 언어/문화권 사용자에게 서비스할 수 있도록 현지화한 소프트웨어에 대한 테스트

**[핵심/키워드]**

* 다양한 언어/문화권 사용자 서비스, 현지화, 국제화
&lt; 단계 &gt;
1\. 요구사항 분석 > 2. 국제화된 제품 설계 > 3. 국제화된 제품구현 > 4. 국제화된 제품 테스트 > 5. 제품 현지화 > 6. 현지화된 제품 테스트 > 7. 제품 출시
&lt; 유형 &gt;
* 글로벌화 검증 테스트 (GVT), 기능 테스트 (FVT), 번역검증 테스트 (TVT)
&lt; 용어 &gt;
* 국제화 (I18n), 현지화 (L10n), 글로벌화 (G13n)

### [테스트] 모델기반 테스트

**[정의]**

요구사항을 바탕으로 테스트 모델 구축 (UML상태 다이어그램)하고 적절한 테스트 전략을 적용함으로써 테스트케이스를 자동 생성하는 기법

**[핵심/키워드]**

&lt; 장점 &gt;
* 유연성, 재사용성, 추적성
&lt; 절차 &gt;
1\. 모델 설계 > 2. 모델 변환 > 3. 테스트 케이스 생성 > 4. 테스트 실행 > 5. 결과 분석 및 수정
&lt; 활용 &gt;
* ISO/IEC 26262

### [테스트] 시프트 레프트 테스팅 (Shit Left Testing)

**[정의]**

개발 초기부터 테스트를 수행하여 초기에 결함을 발견하고 수정하는 기법

**[핵심/키워드]**

&lt; 필요성 &gt; 
* 초기부터 버그 발견, 개발 속도 증가, 품질 향상, 비용절감, 애자일 및 CI/CD 연계
&lt; 테스트 환경 &gt;
* 개발 및 스테이징 환경
&lt; 사례 &gt;
* TDD, CI/CD

### [테스트] 시프트 라이트 테스팅 (Shift Right Testing)

**[정의]**

실 사용자 환경을 고려하여 개발 후반인 운영 단계에서의 테스트를 수행하는 기법

**[핵심/키워드]**

&lt; 필요성 &gt;
* 실제 환경 테스팅, 장애 대응력 점검, 운영환경
&lt; 사례 &gt;
* A/B 테스트, Blue-Green, Chaos Engineering, Canary 테스트

### [테스트] DevTestOps

**[정의]**

Dev(개발)+Test(테스트)+Ops(운영)의 통합 프로세스로, 소프트웨어 품질을 지속적으로 보장하는 접근방식

**[핵심/키워드]**

&lt; 단계 &gt;
전략 및 계획 수립 > 정적 테스트 (Shift Left) > 빌드 및 동적 테스트 (CI 연계) > 운영 환경 테스트 및 모니터링 (Shift Right) > 피드백 및 최적화
&lt; 특징 &gt;
* Shift Left와 Shift Right 적용, CI/CD 연계 테스트 자동화, 테스트 피드백 루프 최적화, 실제 운영 환경 기반 테스트 수행

### [테스트] 크라우드소싱 테스트 (Crowdsourcing Test)

**[정의]**

크라우드 소싱의 개념을 활용해 원격으로 수행하는 SW테스팅

**[핵심/키워드]**

* 군중 테스트
&lt; Pay per Bug 모델 &gt; 
* 발견된 버그에 대해서만 비용 지불
&lt; 효과 &gt; 
* 비용절감, 테스트 커버리지 확대, 전문성(집단지성)
&lt; 단계 &gt;
1\. 의뢰 > 2. 매니징 (Crowd) > 3. 테스팅 > 4. 결과 보고

### [테스트] TDMS (Test Data Management System)

**[정의]**

테스트 케이스에 맞는 다양한 데이터를 가지고 테스트를 할수 있도록 테스트 데이터를 제공하는 시스템

**[핵심/키워드]**

&lt; 단계 &gt;
* 1. (기간시스템, DW, 정보시스템) → 2. 복호화 → 3. 데이터 변환 서버 → 4. 암호화(민감정보) → 5. 적재
&lt; 주요기능 &gt;
* 테스트수행측면 : 테스트데이터확보, 테스트데이터제공, 테스트케이스관리, 테스트결과검증
* 보안측면 : 테스트데이터 Scrambling

### [테스트] MiL (Model-in-the-Loop) 시뮬레이션

**[정의]**

제어 알고리즘이나 시스템 모델을 물리적인 하드웨어나 실제 코드 없이 시뮬레이션 환경에서 검증하는 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 하드웨어 없음, 수학적 모델 시뮬레이션, 개발초기, 시스템 동작 검증, 이론 검증, 알고리즘의 논리적 오류
&lt; 다른 시뮬레이션 관계 &gt;
* MIL > SIL > HIL

### [보안] 분산 서비스 공격 (Distributed Denial of Service, DDoS)

**[정의]**

다수의 공격자(좀비 PC, 봇넷 등)를 이용해 동시에 특정 서버나 네트워크에 과도한 트래픽을 발생시켜 정상적인 서비스를 방해하는 공격

**[핵심/키워드]**

&lt; 특징 &gt;
* 분산된 공격원(좀비/에이전트 등 여러 시스템 활용), 대규모 트래픽
&lt; 절차 &gt;
* 악성코드 은닉 -&gt; 악성코드 감염 -&gt; 감염사실 은폐 및 명령대기 -&gt; DDoS 공격수행
&lt; 대응 &gt;
- PPS 증가 : 비정상 IP에 대한 ACL 적용, 공격 IP차단, SYN Proxy 사용, 보안 패치 및 장비 교체 
- 웹서비스 지연 : 서버 설정 변경, 웹 서버 증설, 공격 IP 차단 
- 대용량 트래픽 전송: 불필요한 서비스 차단, 공격자 IP 차단, DNS 서버 다중화, DNS 전용회선 준비
- 봇넷 유입 차단: IP 필터링, 지리적 차단, 의심 트래픽 필터링
- 행위기반탐지: 트래픽 이상 감지, AI기반 분석 도입
- Blackhole/Sinkhole 라우팅
&lt; 진화공격 &gt;
- DRDoS, Ransom DDoS(RDoS)
- Application Layer DDoS
- Multi-Vector DDoS
- IoT DDoS (Botnet 기반)
- Encrypted DDoS
- PDoS (Permanent DoS)
- Slowloris Attack(Slowly DDos), Carpet Bombing DDoS

### [보안] 세션 하이재킹 (Session Hijacking)

**[정의]**

사용자의 세션 식별 정보(Session ID 등)를 탈취하여 공격자가 정상 사용자로 위장해 인증 없이 서비스에 접근하는 공격

**[핵심/키워드]**

&lt; 특징 &gt;
* 스니핑/XSS 연계(타 기법과 조합)
&lt; 절차 &gt;
* 세션 수집 → 세션 재사용 → 정보 접근 및 조작 → 로그인 없이 서비스 이용
&lt; 대응방안 &gt;
*  HTTPS 적용(세션ID 암호화), 세션 타임아웃 설정(비활성 시 자동 만료), 세션 고정 방지(로그인 시 세션 ID 재발급), 2차 인증(MFA 적용)

### [보안] ARP 스푸핑 (ARP Spoofing)

**[정의]**

공격자가 위조된 ARP 메시지를 전송해 네트워크 내 장비들의 ARP 캐시를 변조, 자신의 MAC 주소를 다른 장비의 IP에 대응시키는 공격

**[핵심/키워드]**

&lt; 특징 &gt;
* 신뢰 기반 악용(ARP는 검증 없음), 간단한 수행(로컬에서 가능), MITM 가능(중간자 위치)
&lt; 절차 &gt;
* ARP Reply 위조 전송 → ARP 테이블 변조 → 트래픽 유도 및 가로채기
&lt; 대응방안 &gt;
* 정적 ARP 설정(고정 맵핑), 암호화 사용(HTTPS, SSH, VPN 등)

### [보안] Blind SQL Injection

**[정의]**

오류 메시지가 출력되지 않는 환경에서, 무작위로 문자를 삽입하여, 나오는 참,거짓에 따라 DB정보를 취득하는 공격 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 조건이 참일 경우와 거짓일 경우 응답 차이를 분석(Brute-force 방식)
&lt; 절차 &gt; 
* 조건문 포함 SQL 삽입 → 참/거짓 응답 차이 분석 > 한 글자씩 민감정보 추출 
&lt; 대응방안 &gt;
* Prepared Statement / Parameterized Query 사용, 입력값 검증, 최소 권한 원칙 적용, DB 오류 메시지 숨김

### [보안] SAST (Static Application Security Test)

**[정의]**

소스코드를 실행하지 않고 정적으로 분석하여 SQL Injection, 취약한 API 등 잠재적 보안 취약점을 사전에 탐지하는 보안 테스트 방식

**[핵심/키워드]**

&lt; 대상 &gt;
* 어플리케이션의 소스 코드, 바이트코드, 바이너리 등
&lt; 기법 &gt;
* 코드 내의 취약점 패턴 탐지, 규칙 기반 분석
&lt; 특징 &gt;
* 코드 실행 없이 분석
&lt; 도구 &gt;
* Snyk, SonarQube 등
&lt; 장단점 &gt;
* 장점 : 조기취약점 발견, 높은 ROI, 자동화 가능
* 단점 : 호출확인 제한, False Negative, 제한적 커버리지

### [보안] DAST (Dynamic Application Security Test)

**[정의]**

애플리케이션을 실제 실행한 후, 외부 공격 시뮬레이션을 통해 런타임 기반 취약점을 탐지하는 블랙박스 테스트 기법

**[핵심/키워드]**

&lt; 기법 &gt;
* HTTP 요청/응답을 기반으로 SQL Injection, XSS, 인증 우회 등 동적 취약점 탐지
&lt; 특징 &gt; 
* 블랙박스, 동적 테스트
&lt; 도구 &gt;
* 국내(Sparrow DAST), 해외(OWASP ZAP, Burp Suite 등)
&lt; 장단점 &gt;
* 장점 : 개발언어에 독립적, 전체 시스템 평가, 실제 상황 모사
* 단점 : 내부 문제 탐지 한계, 낮은 ROI, 확장성 제약

### [보안] 스피어 피싱 (Spear Phishing)

**[정의]**

특정대상(회사, 인물 등)을 겨냥한 맞춤형 피싱공격

**[핵심/키워드]**

&lt; 특징 &gt;
* 맞춤형, 지속공격, 능동적 피싱, 지능형
&lt; 절차 &gt;
* 목표 설정 및 정보 수집 → 신뢰관계 형성 및 공격설계 → 공격실행 → 권한 탈취 및 데이터 유출
&lt; 대응 &gt;
* 출처 확인, MFA, 백신 패치, 신고, 보안 솔루션

### [보안] 스미싱 (Smishing)

**[정의]**

문자메시지와 피싱의 합성어로 악성 앱 주소가 포함된 휴대폰 문자를 대량 전송 후 이용자가 악성 앱을 설치하도록 유도하여 금융정보 등을 탈취하는 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 문자메시지 활용, 피싱
&lt; 절차 &gt;
* 악성 앱 제작 / 업로드 → 스미싱 발송 → URL 클릭 → 악성앱 유포 → 악성 앱 설치 → 개인정보 / 금융정보 유출 → 정보 전송
&lt; 대응 &gt;
* 관리적 (권한 임의변경 금지, 결제 확인 및 취소)
* 기술적 (악성 애플리케이션 삭제, 공동 인증서 폐기 및 재발급)

### [보안] 토르네트워크 (Tor Network)

**[정의]**

사용자의 인터넷 트래픽을 여러 중계 노드를 거쳐 암호화 경로로 우회시켜 익명성 보장을 위해 설계된 다단계 경유 네트워크

**[핵심/키워드]**

&lt; 특징 &gt;
* 익명성, 다단계 암호화, .onion 도메인, 범죄악용, 다크웹 연계
&lt; 구성요소 &gt;
* Cell, Circuit, OP(Onion Proxy), Directory 서버, OR (Onion Router), Exit Node

### [보안] 다중 벡터 공격 (Multi-Vector Attack)

**[정의]**

사이버 범죄자가 피싱, 악성코드, DDoS 등 다양한 공격 수단을 동시에 또는 연계하여 사용함으로써 조직 보안시스
템 침투 성공률을 높이는 공격 방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 다양한 공격경로, 탐지회피, 복잡한 대응, 공격자 (효율증가), 방어자 (부담 증가)
&lt; 절차 &gt;
* 탐색 → 공격실행 → 은밀한 접근 → 권한유지 → 목표수행
&lt; 대응방안 &gt;
* 지능형 위협 차단 (ATP), 예방 중심 보안, 중앙 집중식 가시성 및 관리, 자동화된 인시던트 대응

### [보안] LOTL (Living off the Land) 공격

**[정의]**

공격자가 외부 악성코드 없이, 운영체제(OS)나 시스템에 기본적으로 존재하는 정식 도구(예: PowerShell,
WMI, certutil 등)를 이용해 공격을 수행하는 방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 탐지 회피(정상 도구 사용, 자급 자족 공격), 무기화(PowerShell등 악용), 정상행위 위장, fileless 공격
&lt; 절차 &gt;
* 초기 접근 → 도구악용 → 내부확산 → 은밀한 활동 → 흔적제거
&lt; 대응방안 &gt;
* 권한 최소화, 사용도구 통제, 행위기반 탐지, 로그 정밀 분석, EDR/XDR 활용, SBOM·정책 적용, 사용자 보안교육

### [보안] RSA(Rivest, Sharmir, Adleman) 알고리즘

**[정의]**

큰 소수 두 개의 곱에 대한 인수분해의 어려움을 기반으로 설계된 비대칭키 암호화 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 비대칭 구조(공개/개인키), 수학 기반 안정성(소인수분해 문제), 암호화/서명 인증 가능, 키 분배 용이, 속도 느림
&lt; 구성요소 &gt;
* p, q (소수), n (모듈러스), 오일러함수, e (공개지수), d (개인지수), 공개키 (e, n), 개인키 (d, n)
&lt; 키생성과정 &gt;
1) 두 개의 서로 다른 소수를 선택(p, q)
2) n 계산 (모듈러스) n = p × q
3) 오일러 함수 φ(n) = (p - 1)(q - 1)
4) 암호화 지수 e 선택 
5) 복호화 지수 d 계산

### [보안] 전자서명 (Electronic Signature)

**[정의]**

서명자의 신원을 확인하고, 전자문서의 위변조 여부를 검증하기 위해 전자적 방식(공개키 암호 기반)으로 생성된 데이터

**[핵심/키워드]**

&lt; 특징 &gt;
* 위조불가, 서명자 인증, 부인방지, 변경 불가, 재사용 불가, 분쟁해결 가능
&lt; 생성절차 &gt;
* 원문 작성 → 해시함수 적용 → 해시값 암호화 → 원문 + 서명 전송
* 문서, 해시함수, 개인키, 서명 알고리즘, 전자서명, 디지털 인증서
&lt; 서명검증 &gt;
* 원문 해시값 계산 → 서명 복호화 → 해시값 비교 → 확인 결과 판단
* 공개키, 전달된 문서의 해시값, 복호화된 해시값, 비교단계
&lt; 보안 및 부가요소 &gt;
* 타임스탬프, 키관리시스템, 보안 프로토콜, 생체인식 기술
&lt; 적용알고리즘 &gt;
* RSA, ECDSA, KCDSA, Dilithium, SPHINCS+

### [보안] IPSec (Internet Protocol Security)

**[정의]**

네트워크 계층(3계층)에서 IP 패킷을 암호화하고 인증하여 안전한 네트워크 통신을 보장하는 프로토콜 집합

**[핵심/키워드]**

* 구성요소
- 인증구성: SH, AH(인증, 무결성), ESP(인증, 무결성,기밀성), IKE
- 정책구성: SAD, SPD
* 운영모드
- 전송모드: Host-to-Host (종단 간) 
- 터널모드: Gateway-to-Gateway / Host-to-Gateway 통신
* 정책
- SP: 보안정책 
- SPD: 보안정책 DB 
- SA: 보안연관 파라미터 정의 
- SAD: 보안연관 DB 
* 키관리
- IKE: 키 교환 관련 SA 생성 
- ISAKMP: 키 교환/인증 프로토콜

### [보안] 탬퍼 프루핑 (Tamper Proofing)

**[정의]**

부정 조작을 검출하는 시스템을 통해 소프트웨어에 적용된 위·변조를 감지하여, 이상감지시 프로그램을 오작동하도록 만드는 기술

**[핵심/키워드]**

&lt; 특징 &gt;
* 디지털 컨텐츠 보호, 치환 암호 소프트웨어 위변조 판별
&lt; 생성기술 &gt;
* 해시함수, 핑거프린트, 워터마크
&lt; 방어기술 &gt;
* 원본비교, 프로그램 checking, 실행코드 난독화

### [보안] OAuth 2.0

**[정의]**

사용자가 서비스 제공자에게 로그인 정보(비밀번호 등)를 제공하지 않고, 제3자 애플리케이션이 사용자의 자원 접근을 위임받을 수 있게 해주는 인가(Authorization) 프로토콜

**[핵심/키워드]**

&lt; 특징 &gt;
* 비밀번호 미노출, 액세스 토큰 기반, 역할 분리
&lt; 구성요소 &gt;
* Resource Owner, Client(클라이언트), 권한서버, 자원서버, 액세스 토큰, 리프레시 토큰
&lt; 인가 절차 &gt;
1) 서비스 접근 요청 → 2) 인가 요청 → 3) 로그인 페이지 표시 → 4) 로그인 및 권한 승인 → 5) Authorization Code 전달 → 6) 토큰 요청 → 7) Access Token 발급 →  8) 리소스 요청 → 9) 리소스 응답 → 10) 사용자에게 서비스 제공

### [보안] 패스키 (Passkey)

**[정의]**

공개키 기반을 활용하여 비밀번호 없이 사용자 인증을 수행하는 인증 방식

**[핵심/키워드]**

&lt; 보안방식 &gt;
* 공개키-비공개키 기반 인증
&lt; 사용방식 &gt;
* 디바이스에 저장된 키 자동 사용
&lt; 표준문서 &gt;
* FIDO2 (WebAuthn, CTAP)
&lt; 사례 &gt;
* Apple/Google Passkey

### [보안] 웹 방화벽 (Web Application Firewall, WAF)

**[정의]**

웹 애플리케이션을 대상으로 하는 공격(예: SQL Injection, XSS 등)을 탐지하고 차단하는 HTTP/HTTPS 기반 전용 방화벽 시스템

**[핵심/키워드]**

* WAF는 웹 요청 내용(URI, 파라미터, 쿠키 등)을 검사, OSI 7 Layer
&lt; 주요기능 &gt;
* 웹 공격 탐지 및 차단, HTTP/HTTPS 트래픽 분석, 정책 기반 필터링, 세션 쿠키 보호, SSL 복호화 처리(SSL Offloading)
* 실시간 경보 및 차단, 로깅 및 감사 기능, OWASP Top 10 대응, API 보호 기능, 우회 공격 대응

### [보안] IPS (Intrusion Prevention System)

**[정의]**

침입 시도나 이상 행위를 실시간으로 탐지하고, 탐지 즉시 자동으로 차단하는 능동형 보안 시스템

**[핵심/키워드]**

* IDS의 탐지 기능 + 차단 기능
&lt; 구성 &gt;
* 패킷 캡처 엔진, 탐지 분석 엔진, 정책 제어 모듈, 로깅 및 경보 모듈, 관리자 인터페이스
&lt; 유형 &gt;
* 호스트기반(HIPS), 네트워크기반(NIPS) 
&lt; 탐지방식 &gt;
* 시그니처 기반 IDS, 행위기반 IDS

### [보안] NAC (Network Access Control)

**[정의]**

네트워크에 접속하려는 사용자나 단말(End point)의 보안 상태를 검사하고, 정책에 따라 접근을 허용·차단·격리하는 네트워크 접근 제어 시스템

**[핵심/키워드]**

&lt; 특징 &gt;
* 보안 상태 기반 제어(단말 상태 평가), 접속 전후 제어(Pre/Post 통제),
* 유연한 정책 설정(조건 기반 제어), 인증 연동(AD·LDAP 등 연계 : ID 기반 접근 제어)
&lt; 구성 &gt;
* 인증서버, 정책 서버, NAC 에이전트 / 센서, 네트워크 장비, 검역망, 관리 콘솔

### [보안] DLP (Data Loss Prevention)

**[정의]**

중요 데이터(기밀 정보, 개인정보 등)의 유출을 방지하고, 조직 내에서 데이터의 흐름을 감시·통제하는 정보 보안 기술 또는 시스템

**[핵심/키워드]**

&lt; 기능 &gt;
* 정보 유출 차단(실시간 유출 방지), 콘텐츠 분석(내용 기반 식별), 경로 차단(USB, 이메일, 프린터 등)
&lt; 구성요소 &gt;
* DLP 정책 서버, 에이전트, 콘텐츠 분석엔진, 유출경로 제어 모듈, 로깅 및 감사모듈, 관리자 콘솔
&lt; 유형 &gt;
* Network DLP, Endpoint DLP, Storage DLP, Cloud DLP

### [보안] SIEM (Security Information & Event Management)

**[정의]**

보안 정보 및 이벤트 관리로, 조직의 IT 인프라 전반에서 발생하는 로그와 이벤트를 실시간 수집/분석, 보안 위협 탐지/대응 통합 보안 솔루션

**[핵심/키워드]**

&lt; 특징 &gt;
* 로그 통합 수집(이기종 장비 연결), 실시간 상관 분석(다중 이벤트 연계), 탐지 정밀도 향상(고도화 기법), 모니터링 체계(대시보드/경고)
&lt; 구성요소 &gt;
* 로그 수집기, 로그 저장소, 상관분석 엔진, 경고 및 알림 모듈, 관제콘솔
&lt; 솔루션 명 &gt;
* Splunk Enterprise Security, Azure Sentinel

* ESM

### [보안] UEBA (User and Entity Behavior Analytics)

**[정의]**

사용자 및 엔터티(시스템, 장치 등)의 행위 패턴을 분석해 이상행위를 탐지하는 보안 분석 기술

**[핵심/키워드]**

&lt; 특징 &gt;
* 비정상 행위 탐지(룰 기반 아님), 머신러닝 분석(패턴 학습)
&lt; 기능 &gt;
* 행위 프로파일링, 이상행위 탐지, 위협점수화, 사고조사지원,정책없는탐지
&lt; 기술요소 &gt;
* 머신러닝(ML), 시간 기반 통계 모델링, 이상치 탐지 알고리즘 (Anomaly Detection)
* 행동기반 비교 분석, 리스크 스코어링 엔진, 정책 기반 가중치 모델

### [보안] 공격표면 관리 (Attack Surface Management, ASM)

**[정의]**

인터넷 등 외부에서 수집 가능한 모든 디지털 정보(자산, 서비스, 취약점 등)를 분류·분석·우선순위 지정하여 지속적으로 모니터링하고 위험을 사전에 식별·차단하는 보안 프로세스

**[핵심/키워드]**

&lt; 목표 &gt;
* 알려지지 않은 IT 자산 및 위협을 식별하고, Zero Trust 환경에서 위험 경고(Alarm) 체계
&lt; 공격 표면 관리 유형 &gt;
* 사이버 자산 공격표면 관리(CAASM)
* 외부 공격 표면 관리(EASM)
* 디지털 위험 보호 서비스(DRPS)
&lt; 관리방법 &gt;
* 식별 -&gt; 관리 자동화 -&gt; 최소화
&lt; 관리방안 &gt;
* 디지털 발자국 -&gt; 자산 재고 및 분류 -&gt;  지속적 모니터링 -&gt; 사고 모니터링 -&gt; 위험 감지 및 식별

* 측면이동

### [보안] SASE (Secure Access Service Edge)

**[정의]**

네트워크와 보안 기능을 클라우드에서 통합 제공하는 아키텍처 모델

**[핵심/키워드]**

&lt; 특징 &gt;
* 클라우드 통합(네트워크+보안), 위치 무관 보호, 엣지 적용, 제로 트러스트 기반, 멀티환경 유연성
&lt; 구성요소 &gt;
* 네트워크 보안 : CASB, SWG, FWaaS, ZTNA, VPN
* 네트워크 : SD-WAN, CDN, Carrier, Bandwidth Aggregation, Networking Vendors

* SSE + N/W

### [보안] 디스크 이미징 (Disk Imaging)

**[정의]**

하드디스크나 저장장치의 전체 내용을 바이트 단위로 복사해 동일한 이미지 파일을 만드는 작업

**[핵심/키워드]**

&lt; 특징 &gt;
* 포렌식 분석, 백업 및 복구, 악성코드 분석
&lt; 방식 유형 &gt;
* Disk to Disk : 원본디스크를 그대로 복제(하드카피)
* Disk to File: 이미지 파일로 저장
* File to File: 논리적 파일단위 선택 복사
&lt; 증거수집 절차 &gt;
* 사전 준비 → 원본보호 → 디스크 이미징 수행 → FTK Imager, dd, EnCase 등 사용, 비트단위 전체 이미지 작성 → 무결성 검증 → 백업 및 보관 → 분석 및 보고서 작성

### [보안] ISO/IEC 27001 : 2022

**[정의]**

정보보호 관리체계(ISMS)의 구축, 구현, 유지 및 지속적인 개선을 위한 요구사항을 규정한 국제 표준 2022 버전

**[핵심/키워드]**

&lt; 테마그룹 &gt;
*  조직적, 사람, 물리적, 기술적
&lt; 신규추가 &gt;
* 조직적(37개): 위협 인텔리전스, 정보 삭제, 정보 마스킹, 데이터 누출 방지, 클라우드 서비스 이용 보안 
* 사람(8개): 물리적 보안 모니터링
* 물리적(14개)
* 기술적(34개): 구성관리, 정보삭제, 데이터마스킹, 데이터 누출방지, 모니터링 활용, 웹필터링, 보안코딩

### [보안] ISMS-P (Information Security Management System –Privacy)

**[정의]**

조직의 정보자산 보호뿐 아니라 개인정보의 수집·이용·보관·파기 등 흐름 전반에 대한 보호체계를 포함한 통합인증 제도

**[핵심/키워드]**

&lt; 법적근거 &gt;
* 정보통신망법 제47조(정보보호 관리체계의 인증), 개인정보보호법 제32조의2(개인정보 보호 인증)
&lt; 인증유형 &gt;
* ISMS (정보보호 관리체계 인증 제도), ISMS-P (정보자산 보호 + 개인정보 흐름 전체 포한 통합)
&lt; 심사종류 &gt;
* 최초심사, 사후심사, 갱신심사
&lt; 인증절차 &gt;
1) 준비 및 신청단계 → 2) 심사단계 → 3) 인증
&lt; 인증대상 &gt;
* 의무 (ISP, IDC, 매출 1,500억 이상 상급병원, 1만명 이상 대학, 매출 100억이상 서비스, 일일평균 100만명), 자율
&lt; 인증기준 &gt;
* 관리체계 수립 및 운영(16),  보호대책 요구사항(64), 개인정보 처리단계별 요구사항(22)
&lt; 간편인증 &gt;
* 소기업 등 간편 인증
&lt; 동향 &gt;
* 의무 확대, 실효성 중심 사후관리

### [보안] 악성코드(Malware,멀웨어) 유형

**[정의]**

사용자의 동의 없이 시스템에 침투하여 정보를 탈취하거나 시스템을 파괴, 또는 권한을 탈취해 악의적 행위를 수행하는 프로그램

**[핵심/키워드]**

* 악의적 행위 프로그램, Crimeware
&lt; 특징 &gt;
* 은밀성, 다양한 전파 경로, 복합적 기능, 변종 쉬움
&lt; 유형 &gt;
* Trojan Horse, Virus, Worm, Spyware, Malicious Bot, Rootkit, Backdoor, keylogger, Adware, Ransomware, Downloader, Dropper, Cryptojacking
&lt; 대응 &gt;
* 관리적 (정책 및 기준, 최신 동향, 보고 체계, 정기적 교육, 공급망 보안)
* 물리적 (출입통제 강화, 인증강화, 저장매체 제어, 백업장치 보호)
* 기술적 (최신 백신, 자동감시, 이메일 검증, 정기적 백업, 정품 SW, 취약점 점검, 보안 솔루션, FW, EDR, XDR, SIEM, APT 관제)

### [보안] 사이버 복원력 (Cyber Resilience)

**[정의]**

사이버 공간에서 발생하는 예측 가능한 공격, 알려지지 않았거나 예측 불가능한 위협에 대해 조직의 목표를 달
성하는 능력을 유지하고, 부정적 영향에도 불구하고 회복하는 역량(Ability)

**[핵심/키워드]**

&lt; 구성요소 &gt;
* 비즈니스 영향 분석, 보안정책통제, 종합적 테스트 정책, 매니지드 보안 도구 설치, 사이버 복구 계획
&lt; 확보단계 &gt;
* 위협 평가 역량 확보 → 사이버 보안 방법 도입 → 위협 기반 계획 → 외부 위협으로부터 보호 → 내부 위협 최소화
&lt; 고려사항 &gt;
* 참조 프레임워크 모델: 선형·사이클링 모델, 성숙도 모델
* 조직의 임무와 구성: 임무 구성 파악, CMMI, CERT-RMM 기반 Process Area, CISA CRR 도메인
* 성숙도 수준: 성숙도 분야, 성숙도 수준

### [보안] 신뢰실행환경 (Trusted Execution Environment, TEE)

**[정의]**

메인 프로세서 내에서 일반 OS와 분리된 하드웨어 기반의 안전한 보안 영역

**[핵심/키워드]**

* 안전한 보안 영역, Secure Boot, 구조적 분리 (일반영역, 보안영역)
&lt; 주요 구현방식 &gt;
* Trust zone (ARM), SGX (Intel), SEV (AMD)
&lt; 핵심기술 &gt;
* 하드웨어 격리 (Bus 보안비트, 보안 메모리 영역)
* 안전한 스위칭 (SMC (Monitor Call), 모드 (Monitor Mode))
* 신뢰체인 (Secure Boot, Remote Attentation 디지털 서명)
&lt; 활용 &gt;
* 모바일 지문인식, DRM, SE와 융합 활용

### [보안] 공급망의 사이버 보안 위험관리 (Cybersecurity Supply Chain Risk Management, C-SCRM

**[정의]**

공급망 전체에서 사이버보안 위험에 대한 노출을 관리하고 적절하게 대응하기 위한 전략, 정책 및 절차 등의 관리체계

**[핵심/키워드]**

&lt; 레벨별 관리 &gt;
* 레벨 1: 전사 (이해관계자) → C-SCRM 전략·정책 수립 및 거버넌스
* 레벨 2: 프로세스 (비즈니스관리자) → 전략 기반의 세부 정책·절차 수립 및 각 비즈니스 영역 반영
* 레벨 3: 운영 (시스템 관리자) → 실제 시스템에 정책 적용 및 운영·보고
&lt; 단계 &gt;
* 개요 → 통합 필요성 → 체계 모델 (3단계) → 레벨별 관리 → 레벨별 이해관계자 → 활도 예시

### [보안] 개인정보 보호중심 설계 (Privacy by Design, PbD)

**[정의]**

정보시스템이나 서비스 개발의 기획·설계단계부터 개인정보보호를 고려하여, 사후대응이 아니라 선제적으로 보호조치를 설계하는 접근방식

**[핵심/키워드]**

* 사전 예방, 선제적 보호조치
&lt; 법적 근거 &gt;
* 개인정보보호법 제3조제2항
&lt; 7대원칙 &gt;
* 사전예방, 초기부터 보호조치, 보호 내재한 설계, 보호화 사업기능, 전 생애주기 보호, 가시성과 투명성, 프라이버시 존중
&lt; 8대전략 &gt;
* 최소화, 숨기기, 분리, 총계화, 정보제공, 통제, 집행, 입증
&lt; 인증제 &gt;
* 처리 적법성 평가제도, 인증대상 (IP 카메라, CCTV, 지문 도어락, 스마트가전, 구동 App, 연계 서비스)
* 절차 (계획 (준비) → 인증 (신청 → 시험 → 인증서), 관리 (사후관리))

### [보안] Purdue 모델

**[정의]**

ISA-99에서 제정한 PERA 기반, IDMZ를 사용한 IT와 OT의 이중분리 구조의 보안 참조모델

**[핵심/키워드]**

* ISA, PERA기반, IDMZ, 이중 분리 (IT, OT)
&lt; 계층 &gt;
* Level 0 (프로세스 장비, 네트워크 격리, 안전한 공급망)
* Level 1 (기본제어, 제조, 데이터 보호, 인적보안)
* Level 2 (현장제어, SCADA, HMI 모니터링, 안전 최우선, 인적보안)
* Level 3 (상시 운영 및 제어, 최적화, 비즈니스 이해, 안전한 공급망)
* IDMZ (네트워크 분리, 보안 연계, F/W, IPS, 네트워크 격리, 안전한 공급망)
* Level 4 (지점간 네트워크, DB, SCM, 비즈니스 이해, 안전한 공급망)
* Level 5 (비즈니스 애플리케이션, OLAP, AI, Bigdata, 비즈니스 이해, 네트워크 격리)
< 한계 / 개선 >
* 한계 (에어갭, 인증 취약점 발생) → 개선 (제로트러스트, MFA)

### [보안] 부채널 공격 (Side Channel Attack)

**[정의]**

실제 구현 과정에서 발생하는 물리적 정보(시간, 전력, 소리, 전자파 등)를 분석하여 비밀 정보를 추출하는 공격 방식

**[핵심/키워드]**

* 물리적 정보 분석
&lt; 분류 &gt;
* 제어 (Passive, Active), 모듈 접근 (침입, 준침입), 분석 (Simple SCA, Differential SCA)
&lt; 주요유형 &gt;
* 시차공격, 오류공격, 오류 메시지 공격, 전력 분석 공격, 전자파 분석, Tempest 공격, Cold Boot 공격, 멜트다운, 스펙터, 돌핀 어택)
&lt; 대응방안 &gt;
* Fixed Time, 무작위 지연, 전력 균등화, 차폐, 메모리 암호화, 오류 감지 회로 내장, 무의미한 메시지 출력, 커널 메모리 격리, 분기 예측 차단

### [보안] Model DoS

**[정의]**

AI의 추론(Inference) 과정에서 발생하는 방대한 연산 자원(GPU, CPU)을 고갈시키는 공격

**[핵심/키워드]**

* 연산자원 고갈, OWASP Top 10 for LLM
&lt; 유형 &gt;
* Sponge Examples (연산량 고갈), Recursive Input Attack (재귀호출), Output Overflow (토큰 폭주)
&lt; 절차 &gt;
* 대상 선정 → 공격 페이로드 / 악성 프롬프트 → 공격 도구 및 스크립트 → 공격 수행 / 자원 고갈 → 결과 및 반복
&lt; 대응 &gt;
* 입출력 제한 (Input Context Limit, Output Token Limit, Time out)
* 인프라 보안 (Rate Limit, Resource Quota)
* 탐지 / 필터링 (필터링, WAF)
* 관리 (비용 모니터링, 자동 차단)

### [보안] LLM 탈옥 (Jailbreaking)

**[정의]**

대규모 언어 모델에 설정된 보안 정책, 윤리적 가이드라인 및 필터링 시스템을 우회하여 모델이 원래 거부하도록 설계된 답변을 생성하게 만드는 공격 기법

**[핵심/키워드]**

* Prompt Injection
&lt; 절차 &gt;
* 대상 선정 → 공격 프롬프트 설계 → 탈옥 실행 → 탈옥 성공 및 반복
&lt; 주요 공격 기법 &gt;
* 페르소나 / Role Playing (DAN (Do Anything Now), 가상시나리오, 특정 상황이나 캐릭터 → 안전 가드레일 무력화)
* 인코딩 (Base64 Split, Payload Split, Bypass Attack, 데이터 형식 변조 → 의미 파악 어려움)
* 프롬프트 주입 (Few-shot, 심리적 압박, 잘못된 학습 → 규칙 위반 답변 유도 )
* 자동화 (GCG, PAPE, Data Poisoning, 출력 강제 조정 → 자동 공격)
&lt; 대응 &gt;
* 입력 필터링 (PPL 검사, 시맨틱 분석)
* 프롬프트 강화 (핵심 원칙 우선 명시, 수정 불가)
* 출력 모니터링 (내용 유해성 자동 검사, RLHF)
* 인프라 강화 (TEE,  거버넌스, Red Teaming)

### [보안] Agent Goal Hijack

**[정의]**

AI 에이전트가 수행해야 할 원래의 작업 목표를 해커가 프롬프트 인젝션, 기만적인 도구 출력, 또는 오염된 외부 컨텍스트를 사용하여 자신의 의도대로 변경하는 공격 기법

**[핵심/키워드]**

* OWASP Top 10 for Agentic Application, Zero-Click 공격, 구조적 취약점, 간접 프롬프트 인젝션
&lt; 절차 &gt;
* 대상 탐색 및 정찰 → 공격 벡터 및 명령어 준비 → 공격 전달 → 하이재킹 수행 → 공격 행위 수행
&lt; 공격사례 &gt;
* 데이터 유출, 권한 상승, 파괴적 행위, 지속성 공격
&lt; 대응 &gt;
* Human in the Loop, 권한 최소화, 이중 모델 검증, 입력 검증, 프롬프트 엔지니어링

### [보안] 측면 이동 (Lateral Movement)

**[정의]**

공격자가 초기 침투 후, 네트워크 내부에서 목표 시스템 (데이터, 중요 서버)을 찾아 옆으로 이동하며 권한을 확장하고 전파하는 핵심적인 공격 기법

**[핵심/키워드]**

* 초기 침투 → 확장, 원격 서비스, 합법적 도구 (WMI, Powershell) 악용, LOTL
&lt; 절차 &gt;
* 정찰 및 탐색 → 자격증명 탈취 → 권한 상승 → 확산 및 점유
&lt; 대응 &gt;
* 네트워크 세분화, 최소권한, MFA, 실시간 모니터링, IPS, IDS

### [보안] 다중 갈취(Multi Extortion) 랜섬웨어

**[정의]**

단순히 데이터를 암호화하여 복구 비용을 요구하던 기존 방식에서 벗어나, 여러 단계의 추가 협박을 통해 피해자가 돈을 지불할 수밖에 없게 만드는 진화된 공격 기법

**[핵심/키워드]**

* 여러 단계 추가 협박 랜섬웨어
* 기본 갈취 (데이터 암호화) → 이중 갈취 (데이터 유출) → 삼중 갈취 (DoS 공격) → 사중갈취 (이해관계자 직접 연락)
* RaaS 활용, 표적 공격 가능
&lt; 대응 &gt;
* MFA, 백업, 백신, 최신 패치

