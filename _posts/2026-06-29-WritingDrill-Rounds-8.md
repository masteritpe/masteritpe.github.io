---
layout: post
title: "WritingDrill_Rounds_8"
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

### [빅데이터] KDD

**[정의]**

통계적 패턴이나 지식을 찾기 위해 체계적으로 정리한 방법론

**[핵심/키워드]**

&lt; 절차 &gt;
Selection(데이터 셋 선택)
Preprocessing(전처리)
Transformation(데이터 변환)
Data Mining(데이터 마이닝) 
Interpretation/Evaluation(평가)

### [통계] 정규분포 (Normal Distribution)

**[정의]**

분포 곡선이 평균값을 중앙으로 하여 
좌우 대칭으로 종 모양을 이루는 분포
(= 가우스분포)

**[핵심/키워드]**

- 특징 : 좌우대칭, 종모양(bell curve), 연속확률분포
- 함수 : PDF(확률밀도함수), CDF(누적분포함수)
- 정규분포는 최빈값 = 중앙값 = 평균(μ) 3개값이 모두 동일
- 기호 표현 : X ~ N(μ,σ²)
&lt;중심극한정리 &gt;
표본의 크기가 충분히 클 경우, 어떤 분포이든 표본평균의 분포는 정규분포에 근사

### [소공] 개인정보 보호 강화기술 (PET)

**[정의]**

개인정보를 수집·처리·분석·공유하는 과정에서 개인의 프라이버시를 보호하기 위한 기술의 집합

**[핵심/키워드]**

* 데이터 난독 처리도구
: 차분 프라이버시, 합성데이터 생성(SDG), 영지식증명
* 암호화된 개인정보 처리
: 동형 암호화(HE), 신원 기반 암호화(IBE), 안전한 다자연산(SMPC), 신뢰받는 실행환경
* 연합 및 분산 분석
: 연합 학습(FL), 분산 분석
* 데이터 책임도구
: 책임시스템, 개인정보 관리 시스템

### [빅데이터] CRISP-DM (Cross-Industry Standard Process for Data Mining)

**[정의]**

4개의 프로세스 모델을 적용하여 6단계로 데이터 마이닝을 분석할 수 있는 방법론

**[핵심/키워드]**

* 4개 프로세스 : 최상위, 일반화, 세분화, 프로세스
* 6단계 분석 방법론: 업무이해, 데이터이해, 데이터준비, 모델링, 평가, 배포
* 데이터마이닝 방법론
- KDD, CRISP-DM, SEMMA

### [통계] 베르누이 분포 (Bernoulli Distribution)

**[정의]**

결과가 참 또는 거짓, 두가지인 단일한 베르누이 시행의 결과를 
나타내는  이산 확률 분포

**[핵심/키워드]**

* 특징 : 단일 베르누이 시행, 이산확률분포, 
* 함수 : PMF(확률 질량 함수)
* 표기법 : X ~ B(1,p), 
기대값 E[X] = p, 분산 Var[X] = p(1-p)

### [소공] AOP (Aspect Oriented Programming)

**[정의]**

핵심 관심사(Core Concerns)에 대한 관점과 횡단 관심사(Cross-cutting Concerns)에 대한 관점들로 프로그램을 분해해 Weaving을 통해 프로그램을 구현하는 기법

**[핵심/키워드]**

* 관점 : core concern, cross-cutting concern
* 구성요소 : joint point, point cut, advice, aspect, weaving, target

### [빅데이터] 빅데이터 분석 방법론

**[정의]**

- 빅데이터 출현으로 인한 비정형데이터 활용을 위한 새로운 분석 방법론

**[핵심/키워드]**

* 기법/유형 
- 계층적 프로세스 모델(3계층, 5단계절차)

* 계층: 단테스 
- 단계(Phase), 테스크(Task), 스텝(Step)

* 절차: 기준분구평 
> 분석기획 
> 데이터준비 
> 데이터분석 
> 시스템 구현 
> 평가 및 전개

### [통계] 기하 분포 (Geometric Distribution)

**[정의]**

처음으로 성공이 일어날 때까지의 
베르누이 시행 횟수의 분포

**[핵심/키워드]**

* 특징 : 처음 성공까지 시행횟수, 이산확률분포
* 함수 : 확률질량함수
* 표기법 : X ~ Geo(p)
기대값 E[X] = 1/p, 분산 Var[X] = (1-p)/p2

### [소공] 인터프리트 언어(Interpreted Language)

**[정의]**

코드를 한 줄씩 해석(interpret) 하여 바로 실행하는 방식의 프로그래밍 언어.
사전 컴파일 변환없이, 실행 중에 인터프리터(Interpreter)가 코드를 읽고 해석하는 방식

**[핵심/키워드]**

* 특징
- 플랫폼 독립적
- 실시간 디버깅. 한줄씩 해석하며 즉시 실행

* 예시언어 
: Python, JavaScript, Ruby, PHP, Perl

### [빅데이터] 데이터 레이크 (Data Lake)

**[정의]**

대규모의 다양한 원시 데이터 세트를 기본 형식으로 저장하는 데이터 레파지토리

**[핵심/키워드]**

* 대규모 데이터, 다양한 형태, schema-on-read
* 절차 : 수집, 조직, 분석, 제공
* 계층 : raw, processed, curated

### [통계] 이항 분포 (Binomial Distribution)와 포아송 분포(Poisson Distribution)

**[정의]**

[이항분포]
성공률이 p인 베르누이 시행을 n번 시행했을 때의 확률분포

[포아송분포]
단위 시간 또는 공간 내 어떤 사건이 발생하는 횟수를 나타내는 이산확률분포

**[핵심/키워드]**

둘다 이산확률분포
* 이항분포 : 고정 시행 수 중 성공 개수. 베르누이 시행의 반복
* 포아송 분포 : 단위시간/공간 내 사건수, 이항분포의
극한형태, n→∞,p→0일 때 수렴

### [소공] REST (Representational State Transfer)

**[정의]**

웹의 기존 기술과 HTTP 프로토콜을 활용하여 분산 시스템을 설계하는 아키텍처 스타일

**[핵심/키워드]**

* 구성 : 리소스, 행동, 표현, 상태코드
 * 6원칙 : 클라이언트-서버, 무상태, 캐시, 일관된 인터페이스, 계층화된 시스템, 코드온디멘드

### [빅데이터] 데이터 메시 (Data Mesh)

**[정의]**

도메인 중심의 분산형 데이터 관리방식(탈중앙화)을 적용하는 데이터 아키텍처 패러다임

**[핵심/키워드]**

* 도메인 중심, 탈중앙화, 자율운영
 * 4원칙 : 도메인소유권, 데이터제품화, 셀프서비스, 연합형계산

### [통계] 불편추정량 (Unbiased Estimator)

**[정의]**

표본으로부터 구한 통계량의 기대치가 추정하려 하는 모수의 실제 값에 같거나 가까워지는 성질(불편성)

**[핵심/키워드]**

점추정의 4가지 성질 중 하나
(불편성, 충분성, 효율성, 유효성)
표본 기대값과 모수가 같으면, 편향은 0(제로)임

### [소공] SOA(Service Oriented Architecture)

**[정의]**

- 다양한 비즈니스 환경에서 이기종 통합 및 loosely coupled 하게 서비스 단위를 재사용, 재조립을 가능하게 하는 서비스 지향 아키텍처 

- 프로세스 중심, 플랫폼 독립적, loosely coupled

**[핵심/키워드]**

* 아키텍처 
Service Broker, Service Provider, Service Consumer 
* 기술요소 
XML, ESB, SOAP, WSDL, UDDI
* MSA 기본사상

### [빅데이터] 빅데이터 시각화(Visualization)

**[정의]**

데이터 시각화, 정보 시각화, 인포그래픽이 통
합된 영역으로 정보설계와 메시지 전달을 모
두 고려한 시각화

**[핵심/키워드]**

* 데이터시각화 + 정보시각화 + 인포그래픽
* 목적 : 정보전달 + 설득
* 유형(시각, 비교, 관계, 분포, 공간)
* 시각화 절차 : 정보 구조화→정보 시각화→정보 시각표현
* 시각화 도구 : Excel, CSV, JSON, D3, Crossfilter, Tangle, R, Gephi, Tableau, Infogram, Datawrapper
* 벤 프라이 시각화 방법론

### [통계] 점추정 (Point Estimation)

**[정의]**

모집단의 모수를 하나의 값으로 
추정하는 과정

**[핵심/키워드]**

하나의 값 => 모집단 추정 
추정량 4가지 준거(불편성, 충분성, 효율성, 유효성)
방식(베이지안, 적률법, 최대가능도)
MSE, RMSE, LSM, MLE, MME

### [소공] 4+1 Architectural View Model

**[정의]**

- 소프트웨어 아키텍처를 다양한 이해관계자 관점에서 설명하기 위해 Philippe Kruchten이 제안한 모델
- 고객(사용자) 요구사항을 중심으로 설계자, 시스템통합자, 개발자, 시스템엔지니어의 관점으로 소프트웨어 아키텍처를 구축하는 설계방법

**[핵심/키워드]**

* 특징 : 다양한 이해관계자 관점, 4가지 관점+1
* 5가지 뷰
논리 뷰(Logical) : 설계자 관점
구현 뷰(Implementation) : 개발자 관점
프로세스 뷰(Process) : 시스템 통합자 관점
배포 뷰(Deployment) : 시스템 엔지니어 관점
유스케이스 뷰(Use-Case) : 사용자 관점

### [빅데이터] 텍스트 마이닝 (Text Mining)

**[정의]**

비정형 텍스트 데이터에서 유용한 정보, 패턴, 지식을 자동으로 추출하고 발견하는 과정

**[핵심/키워드]**

* 기법 : 정보 추출, 문서분류(군집화), 문서요약, Concept Linkage, Question Answering, Topic Tracking
* 절차 : 데이터 수집/정제/반환 > 전처리 > 정보추출 > 클러스터링/범주화 > 요약/검색
* 전처리 : 토큰화, 불용어, 형태소, 어간/어미, 대소문자 통일
* 표현 : BoW, TF-IDF, Word Embedding, Word2Vec
* 마이닝 : 분류, 군집, 토픽모델링, 감성분석

### [통계] 구간추정 (Interval Estimation)

**[정의]**

일정 확신으로 모수가 포함될 구간을 
추정하는 것

**[핵심/키워드]**

신뢰구간, 신뢰수준,
작은 오차범위, 짧은 신뢰구간

### [소공] 요구공학 (Requirements Engineering)

**[정의]**

시스템의 개발, 변경의 목적(What)을 식별하기 위해 이해관계자들의 요구를 이해 및 조정하여 체계적으로 수집, 분석, 명세화, 검증하는 공정 또는 학문

**[핵심/키워드]**

* 특징 : 요구분석, 지속적 변경관리
* 원칙 : 명확성, 완전성, 검증가능성, 일관성, 수정용이성, 추적가능성, 이용성
* 개발 프레임워크 : 타당성, 추출(수집), 분석, 명세화, 검증
* 관리 프레임워크 : 협상, 기준선, 변경관리, 확인 검증
* 분류 : 기능 (기능, 자료, 인터페이스, 사용자), 비기능 (자원, 성능, 보안, 품질)
* 요구사항 명세서, 요구사항 추적표, CMMI v1 (RD, REQM), CMMI v2/3(RDM)

### [빅데이터] 소셜 네트워크 분석(SNA, 사회연결망 분석)

**[정의]**

- 수학의 그래프 이론을 바탕으로 소셜 네트워크 서비스에서 소셜 네트워크 연결 구조와 연결 강도를 분석하여 사용자의 명성 및 영향력을 측정하는 분석기법
- SNS데이터 활용해 사회연결망과 사회구조등을 사회과학적으로 분석하는 기법

**[핵심/키워드]**

- 구성요소 : 노드, 링크, 차수(밀도)
* 분석 주요속성
응집력(관계), 등가, 명성(하위), 범위, 중계(중심연결) 

* 분석 기법 
- 중심성 분석 : 연결중심성(Degree Centrality), 매개중심성
(Betweenness Centrality), 근접(인접) 중심성(Closeness Centrality), 고유벡터 중심성(Eigenvector Centrality) 
- 이웃 분석
- 응집도 분석
- 밀도 분석
- 친화도 분석

### [통계] 중심극한정리 (Central Limit Theorem)

**[정의]**

표본의 크기가 크면 표본평균의 확률분포는 정규 분포를 보인다는 정리

**[핵심/키워드]**

충분한 표본 크기 , 모집단 분포 무관
표본평균 분포 => 정규분포

### [소공] ATAM (Architecture Trade-off Analysis Method)

**[정의]**

다양한 품질속성(성능, 신뢰성, 보안 등)의 상충관계(Tradeoff)를 분석하여 아키텍처의 품질을 평가하는 기법

**[핵심/키워드]**

* 특징 : 품질속성과 상충관계
* 절차 : 소개, 조사분석, 테스트, 보고
* 상세절차 : 
- 소개: ATAM, Biz 동인, 아키텍처
- 조사 : 식별, 유틸리티트리, 접근법분석
- 테스트 : 우선순위, 분석반복
- 보고 : 결과발표

### [빅데이터] 오피니언 마이닝 (= 감성분석)

**[정의]**

- 다양한 온라인 뉴스와 소셜 미디어 코멘트, 사용자가 만든 콘텐츠에서 표현된 의견을 추출/분류/이해하고 자산화 하는 컴퓨팅 기술 

- 어떤 사안이나 인물, 이슈, 이벤트에 대한 사람들의 의견이나 평가, 태도, 감정 등을 분석 
- 인터넷에 산재한 게시물 및 댓글 등에서 소비자의 의견을 수집/분석해 제품이나 서비스 등에 대한 평한을 추출해 내는 마이닝 기법

**[핵심/키워드]**

* 수행단계 
1) 특징추출: 의미 있는 요소, 특징을 추출하는 단계 
2) 의견 분류: 어떤 의미로 사용되었는지 분석하고 분류하는 단계 
3) 요약 및 전달: 선호도가 밝혀진 오피니언 정도를 요약하고 사용자에게 전달

### [통계] t-검정 (t-test)(=Student's t-test)

**[정의]**

모집단의 분산 또는 표준편차를 
모르는 경우 모평균 검정을 위해 
사용되는 방법

**[핵심/키워드]**

가설검정, t-분포, t-value,
모집단 분산/표준편차 모름
적은 표본크기, 두 집단 평균차이
독립표본, 대응표본
student, welch, 양측검정, 단측검정

### [소공] DDD(Domain-Driven Development)

**[정의]**

- 해당 도메인과 일치하도록 소프트웨어를 모델링하는 데 중점을 둔 소프트웨어 설계 접근 방식
- 적절한 도메인 모델을 선택하고, 선택된 도메인 모델을 기반으로 분석, 설계, 구현에 걸친 SW 개발 전 과정을 주도하고 모델을 의사소통의 핵심수단으로 사용하기 위해 적용할 수 있는 기법과 패턴의 집합

**[핵심/키워드]**

* 구성요소 
Entity(객체)
Value(값)
Aggregate(집합체): 연관된 객체와 값의 묶음
Repository(저장소)
Service(서비스)

### [빅데이터] 연관규칙(Association Rule)

**[정의]**

특정사건들이 동시에 발생하는 빈도로 상호간의 연관성을 표현하는 규칙
(예: 장바구니 분석)

**[핵심/키워드]**

- 연관성 측정지표(지지도,신뢰도,향상도)
- 빈발 항목 집합(Frequent Item set)을 기반으로 연관규칙도출
- Apriori 연관규칙 탐색과정 : 결합(join)→가지치기(pruning)
*연관규칙 알고리즘
- 기본 연관분석 : 연관규칙, Apriori(선험적 알고리즘), FP-Growth(빈발패턴성장), Eclat(메모리 효율)
- 순차 패턴분석(연속규칙) : AprioriAll, GSP(Generailzed Sequential Pattern Mining), PrefixSpan

### [통계] 독립표본 t-검정 (Independent t-test)

**[정의]**

두 개의 독립적인 집단 간의 평균 차이를 검정하기 위한 통계적 방법

**[핵심/키워드]**

* 가정사항 : 독립성, 정규성, 등분산성
- 서로 다른 두 집단 간 t-검정
- 두 집단이 같은 모집단에서 나왔는지를 평균값을 기준으로 비교하는 가설검정 방법

### [소공] 소프트웨어 프로세스 (SP, Software Process) 인증

**[정의]**

SW 기업 및 개발 조직의 SW 프로세스 품질 역량 수준을 심사하여 등급을 부여하는 제도

**[핵심/키워드]**

* 근거 : SW 진흥법 제21조, 시행령 제18조부터 제22조, 시행규칙 제8조부터 제 11조
 * 기준 : 5개영역(프로젝트관리, 개발, 지원, 조직관리, 프로세스개선), 16개 항목
 * 등급 : 2등급, 3등급
 * 대상 : 사업종료 후 1년이내, SW 제품, 조직단위

### [빅데이터] 데이터라벨링

**[정의]**

- 원천 데이터를 AI가 효과적으로 학습할 수 있도록 사람이 먼저 라벨링을 통해 데이터 셋을 만들어 주는 과정

**[핵심/키워드]**

* 절차
원천데이터수집>데이터전처리>데이터저장>라벨링>
학습데이터 검토 및 업데이터>데이터 큐레이션 및 정제>모델적용>평가 및 모니터링

### [통계]  대응표본 t-검정 (Paired t-test)

**[정의]**

같은 집단에서 두 번 측정된 값(또는 짝지어진 두 집단)의 평균 차이를 비교하는 통계적 검정 방법

**[핵심/키워드]**

* 가정사항 : 정규성
* 하나의 모집단 내부 두 집단 간 t-검정

### [소공] 소프트웨어사업 영향평가

**[정의]**

공공기관이 SW 사업을 추진할 경우 민간시장에 미치는 영향을 사전에 분석해 결과를 과기정통부 장관에게 제출하게 하는 제도

**[핵심/키워드]**

* 근거 : SW진흥법 제43조, 시행령 제36조
 * 대상기관 : 공공, 연구, 공단, 지자체, 국가
 * 대상사업 : 장이 추진하는 SW사업
 * 제외 : 상용SW, 안보관련, 민간투자, 특정목적
 * 평가항목 : 민간 SW 유사성, 침해가능성, SW 사업 필요성, 공공성
 * 결과 : 침해가능없음, 최소화, 재검토
 * 평가시기 : 예산편성, 발주준비, 재평가
 * 평가유형 : 기관공동, 대국민서비스

### [빅데이터] 교차분석=카이제곱검정

**[정의]**

- 두 범주형 변수간의 연관관계를 볼때 교차표(분할표)를 작성하여 변수들간 관계를 분석하는 기법

**[핵심/키워드]**

1) 적합도 검정 - 변수 1 (불량원인-작업조)
2) 독립성 검정 - 변수 2 (작업조-기계호기 고장횟수)
3) 동질성 검정 - 변수 2 (성별-자동차선호도)

### [통계] z-검정 (z-test)

**[정의]**

모집단의 분산(또는 표준편차)이 알려져 있을 때, 표본 평균이 특정 값과 유의미하게 다른지를 검정하는 가설검정 방법

**[핵심/키워드]**

큰 표본크기, 정규분포, 
분산/표준편차 알고있음
Z = (X - μ)/σ

### [소공] 기능점수 (FP, FunctionPoint)

**[정의]**

사용자 관점에서의 사용자가 요구하고 사용자에게 인도되는 기능을 정량적으로 산정하는 소프트웨어 규모측정 방법

**[핵심/키워드]**

* 특징 : 사용자중심, 기능점수
* 표준 : ISO/IEC 14143
* 프로세스 : 측정유형, 범위 및 경계, 데이터기능, 트랜잭션기능, 미조정점수, 조정인자(보정계수), 조정 후 결정
* 측정항목 : 데이터기능, 트랜잭션기능, (+DET, RET, FTR(정규법))
* 유형 : 정규법, 간이법
* 데이터 기능 : ILF, EIF
* 트랜잭션 기능 : EI, EO, EQ

### [빅데이터] ANOVA/분산분석 (Analysis Of Variance)

**[정의]**

- 집단간 분산비교, 차이분석(평균)을 위한 통계 분석 기법 
- 독립집단 3개 이상
- 집단간의 평균이 서로 차이가 있는지 확인하기 위한 검정 방법

**[핵심/키워드]**

- 검정방법: F-test 
F통계량 = 집단간분산/집단내분산 
- F통계량이 1근처이면 집단간 차이없음, 1보다 크면 집단간 차이있음

### [통계] 오차의 등분산성(Homoscedasticity)

**[정의]**

- 회귀모델에서 오차의 분산이 일정하다는 가정
- 예측값에 관계없이 오차의 크기가 동일하게 분포되어 있어야 한다는 것

**[핵심/키워드]**

- 선형회귀 추정량의 효율성 보장
- 신뢰구간과 가설검정의 정확성 확보
- 예측의 일관된 정확도 유지

### [소공] CMMI 3.0 (Capability Maturity Model Integration 3.0)

**[정의]**

소프트웨어 개발 및 서비스 관리 등 다양한 산업에서 프로세스 성숙도를 평가하고 개선하기 위한 글로벌 표준모델

**[핵심/키워드]**

* 특징 : 프로세스 성숙도 평가
 * 도메인 : core, development, service, supplies, security, safety, people, data, virtual
 * 구성 : category area, capability area, practices

### [빅데이터] 불균형 데이터 처리

**[정의]**

- 특정 클래스의 데이터가 타 클래스의 데이터 수와 너무 차이가 날 때, 샘플링을 통해 이 비율을 맞추는 작업

**[핵심/키워드]**

* 불균형 데이터 처리 기법
1) 언더 샘플링/다운 샘플링
- 랜덤 언더 샘플링, Tomek link, CNN, OSS(Tomek link+CNN), ENN

2) 오버 샘플링/업 샘플링 
- 랜덤 오버 샘플링, SMOTE, Borderline SMOTE, ADASYN, Combine Sampling

### [통계] 다중공선성 (Multicollinearity)

**[정의]**

회귀분석에서 독립변수들 간에 
강한 상관관계가 나타나는 문제

**[핵심/키워드]**

ρ(Xi, Xj) ≈ ±1
확인(산포도, 상관계수, 허용/공차, 
분산팽창지수(VIF >=10))
해결(무시, 변수제외, 변수통합, 
FA, PCA, Ridge)

### [소공] FTA(Fault Tree Analysis)

**[정의]**

시스템 고장(Top Event)의 원인을 논리 회로 구조로 도식화하여 분석하는 연역적(Top-down) 위험 분석 기법

**[핵심/키워드]**

* 구성 :AND/OR 게이트, 기본사상, 사상(원), 연결기호
* 사건들 간의 논리적 관계를 AND/OR 게이트 등으로 표현하여 고장의 원인 조합을 도출

### [빅데이터] 데이터 비식별화

**[정의]**

개인정보에서 개인을 식별할 수 있는 정보를 삭제하거나, 다른 정보와 쉽게 결합하여도 특정 개인을 식별할 수 없도록 처리하는 기술

**[핵심/키워드]**

* 비식별화 적용 대상
- 식별자(주민번호,여권번호), 준식별자(개인/신체특성), 민감정보(종교,정치성향등) 

* 비식별화 조치 세부기술(가총삭범마)
- 가명처리: 휴리스틱 가명화, 암호화, 교환
- 총계처리: 총계처리, 부분총계, 라운딩, 재배열
- 삭제 : 식별자 삭제, 식별자 부분삭제, 레코드 삭제, 식별 요소 전부삭제
- 범주화 : 랜덤 라운딩, 범위 방법, 제어 라운딩
- 마스킹 : 임의 잡음 추가, 공백 및 대체

* 프라이버시 모델 - K익명성, L다형성, T근접성

### [통계] 상관관계 분석

**[정의]**

- 두 변수간의 선형관계(비례식성립)를 분석하는 기법

**[핵심/키워드]**

- 선형성 강도에 대한 통계적 분석

* 상관분석의 가정사항(조건) - 이정선
- 이변량: 비교 가능한 두개의 연속형 변수 존재 
- 정규분포: 두 변수 중 적어도 하나의 변수는 정규성 만족
- 선형성 검증: 연속형 두 변수간 선형적 관계 존재(산점도)

* 학습시간 - 성적의 관계, 키-몸무게
* 상관계수 종류 : 피스켄
1) 피어슨 상관계수(감마) 
- 적률 상관계수
- 등간/비율변수-등간/비율변수
2) 스피어만(로우)
- 순위 상관계수
- 서열변수-서열변수
3) 켄달(타우)
- 서열변수-서열변수

### [소공] 정보시스템 상주감리

**[정의]**

감리원이 사업 현장에 상주하거나 주기적으로 투입되어 위험요소 및 산출물 검토, 자문을 수행하는 감리

**[핵심/키워드]**

* 법적근거
- 전자정부법 제 57조
* 특징 : 현장상주, 제3자의 독립적 관점, 기술적 측면의 감사와 평가
* 추진배경 : 대기업 참여 하한금액 상향(20억→40억)
중소기업 경험 부족→3단계 감리만으로 불충분하여
상주감리 추가 허용
* 대상 :40억 이상 사업 중소기업이 수행, 위험도 난이도 높은 사업(발주자판단)
* 자격 : 수석감리원(20억이상 3회 이상, 3년 이상 PM/QA)

### [빅데이터] NoSQL

**[정의]**

- 데이터의 읽기보다 쓰기에 중점을 둔, 수평적 확장이 가능하며 다수 서버들에 데이터 복제 및 분산저장이 가능한 데이터베이스
- BASE
- 수평, 복제, 분산

**[핵심/키워드]**

* 종류
- Key/Value Store: Redis 
- Column Family: Hbase, Cassandra (내부 key sorting) 
- Document Store: MongoDB(BSON, Replication)
- Graph: Neo4j

* NoSQL 모델링 패턴
Denormalization(반정규화)
Aggregation(집계 기반 구조)
Application Side Join (클라이언트 측 조인)
Atomic Aggregation (원자성 집계)
Index Table(인덱스 테이블)
Composite Key Table(복합 키 테이블)

### [통계] 데이터레이크하우스

**[정의]**

- 데이터레이크의 유연성 및 확장성과 데이터웨어하우스의 데이터 구조 및 데이터 관리 기능을 결합한 새로운 개방형 데이터관리 아키텍처

**[핵심/키워드]**

- 하이브리드 데이터 관리 아키텍처
- 데이터레이크 + 데이터웨어하우스(일관성,ACID)

* 데이터레이크하우스 구성요소
1) 수집계층 
2) 스토리지레이어 
3) 메타데이터레이어 
4) API계층 
5) 소비층

### [소공] HAZOP

**[정의]**

공장 설비 프로세스에 존재하는 위험요소 및 운용상의 문제점을 찾아내는 정성적 분석기법

**[핵심/키워드]**

* 구성요소 : 가이드워드(Guideword), 변수(Parameter), 원인, 결과, 안전장치 
- 가이드워드 : 없음(No), 과다(More), 과소(Less), 부분적(Part of), 대등(As well as)
* 절차 : 분석범위 설정 > 팀구성 > 예비조사 > 토론 > 분석결과 기록
* 설계가 완료된 이후 수행 → 설계의 잠재적 결함이나 리스크 사전 도출
* “가이드워드”를 활용한 체계적인 질문을 통해 위험요소 탐색

### [빅데이터] 프라이버시 모델 - KLT

**[정의]**

* k-익명성
- 준식별자의 모든 가능한 조합에 해당하는 데이터의 갯수가 최소한 k개 이상이 되어야 한다는 조건을 구현한 기법 

* l-다양성 [두음:다동배]
- 특정인 추론이 안된다고 해도 민감한 정보의 다양성을 높여 추론 가능성을 낮추는 기법 
- 동질성 또는 배경지식 등에 의한 추론 방지

*t-근접성
: ℓ-다양성 뿐만 아니라, 민감한 정보의 분포를 낮추어 추론 가능성을 더욱 낮추는 기법

**[핵심/키워드]**

* k-익명성 
- 준식별자
- 연결 공격 방지

* l-다양성
- 동질성 또는 배경지식 등에 의한 추론 방지

*t-근접성
- 전체 데이터의 분포와 특정 정보의 분포차이를 t이하로 하여 추론 방지 
- 쏠림공격방어, 유사성공격방어

### [통계] 통계적가설검정

**[정의]**

모집단의 특성에 대한 가설을 설정한 뒤에 표본의 검정통계량을 이용하여 가설의 채택여부를 결정하는 통계적 분석방법

**[핵심/키워드]**

통계적 가설검정 절차
- 가설설정(귀무가설, 대립가설)
- 유의수준(α) 결정
- 검정통계량 선정 및 계산
- 가설검정(기각역)
:검정통계량이 기각역에 포함되면 → 귀무가설 기각
- 유의성검정(P-Value)
:P-value < α(유의수준)이면 → 귀무가설 기각
- 통계적 결론

### [소공] STAMP

**[정의]**

- SW 관계 중심 분석기법
- 사고의 원인을 특정 기능이나 컴포넌트의 결함이 아닌 전체 시스템의 구성 및 제어 문제로 접근하는 위험분석 모델

**[핵심/키워드]**

* 시스템을 제어 구조(Control Structure)로 보고, 사고를 제어 실패로 간주하여 분석하는 방법론
* 구성요소
제어 구조 (Control Structure), 제어 행위 (Control Actions)
피드백 (Feedback), 제어 실패 (Control Flaws), 시스템 제약조건 (Safety Constraints)
* 제어 구조 흐름 (Control Loop)
Controller → Actuator → Controlled Process → Sensor → Controller

### [빅데이터] 데이터 품질 인증제도(DQ인증)

**[정의]**

- 과학기술정보통신부가 지정한 데이터 품질 인증기관이 ①데이터 내용, ②데이터 관리체계를 진단하고 수준을 평가해 품질을 인증하는 제도
&lt;관련법령&gt;:「데이터 산업진흥 및 이용촉진에 관한 기본법」제20조

**[핵심/키워드]**

* 인증대상
 - 데이터 내용 : 정형, 비정형, 반정형, AI학습용
 - 데이터 관리체계 : 프로세스, 인력, 조직, 기술 등 관리체계의 성숙도 평가

* 심사항목
- 정형데이터 : 완전성, 유효성, 일관성, 정확성, 접근성, 유일성

- DQC인증은 2022년 폐지. 2023년 DQ인증제도로 공식 전환
- DQ인증은 '데이터 내용 + 관리체계' 품질 인증으로 확대 및 구체화

### [통계] 회귀분석

**[정의]**

독립변수와 종속변수 간 인과관계를 분석하기 위한 통계기법

**[핵심/키워드]**

회귀분석 절차
- 회귀계수 도출(최소 제곱법)
- 결정계수 도출
- 회귀식 유의성 검정(F검정)
- 독립변수 유의성 검정(T검정)
- 다중공선성 진단(VIF)

### [소공] 서버리스 컴퓨팅

**[정의]**

- 특정 이벤트의 반응하는 함수가 실행되는 FaaS와 BaaS 기반으로, 마치 물리적 서버가 없는 것처럼 동작하여 기존의 방식보다 연결 및 처리속도를 개선한 컴퓨팅 기술

**[핵심/키워드]**

Client (SPA: React, Vue 등)
    ↕️ API 호출
Serverless Backend (Lambda, API Gateway 등)

* 핵심기술 
- Client: SPA(Single Page Application), Web App 
- Front End: API G/W, Restful API
- Function Service: FaaS, Event Router
- Back End: BaaS, Container

### [빅데이터] 개인정보 처리 가이드라인

**[정의]**

- 개인정보 오/남용 방지 및 데이터 산업 활성화를 위해 안전한 가명정보 활용 방안을 안내하는 가이드라인
- 개인정보보호법 제28조의2에 근거
- 개인정보의 처리목적 범위 내에서 정보주체의 동의없이 가명정보를 처리하는 과정에서 발생할 수 있는 오/남용 방지

**[핵심/키워드]**

* 구성: 개인정보, 가명정보, 익명정보
* 대상: 통계작성,과학적연구,공익적기록보존)
- 가명정보: 특정 개인을 식별할 수 없도록 처리했지만, 추가정보와 결합하면 식별 가능한 정보
→ 통계, 연구, 공익적 목적 등을 위해 동의 없이 활용 가능
- 익명정보: 특정 개인을 식별할 수 없는 정보
→ 완전히 식별이 불가능하도록 처리되면 자유롭게 활용 가능
* 가명처리절차: 사위가적사
사전준비>위험도검토>가명처리>적정성검토>안전한 사후관리

### [통계] 모수통계, 비모수통계

**[정의]**

* 모수통계 
- 모집단의 분포를 가정하고 통계분석을 수행하는 방법
- Z-분포, T-분포, F-분포, 카이제곱 분포를 따른다고 가정 


* 비모수통계 
- 모집단의 분포를 가정하지 않고 통계분석을 수행하는 방법

**[핵심/키워드]**

&lt; 모수통계 &gt;
- 모집단의 정규분포 가정(주로 연속형변수) 
- 표본분산, 표본평균 등 모수 이용
- 예시 : Z검정, T검정, F검정, ANOVA, 피어슨 상관계수

&lt; 비모수통계 &gt; 
- 모집단의 정규분포 가정하지 않음(주로 범주형변수)
- 중앙값, 순위 등 비모수 이용
- 예시 : 콜모고로프-스미르노프, 카이제곱, 맨 휘트니 U test, 윌콕슨 부호 test, 스피어만 상관계수

### [소공] 형상관리 (Configuration Management)

**[정의]**

SW 생명주기상 무결성(Integrity)을 보장하기 위해 형상 항목을 식별, 통제, 감사 및 기록하는 생명주기 지원 및 보호 활동

**[핵심/키워드]**

* 대상 : 모든 산출물, 변경 관리 및 일관성
* 절차 : 식별, 통제, 감사, 기록
* 도구 : cvs, svn, git clearcase, perforce
* 기준선 : 기능, 분배, 설계, 시험, 제품, 운영
* 형상관리 통제 위원회(CCB)

### [빅데이터] 데이터 안심구역

**[정의]**

법적 기준(데이터산업법 등)에 따라 지정, 미개방 데이터 등 민감한 데이터를 안전하게 분석·활용할 수 있는 구역

**[핵심/키워드]**

* 목적
- 미개방 데이터(공공·민간 보유)의 
안전한 분석,활용

* 적용 데이터
- 미개방 데이터, 민감 데이터, 
공간정보 등 다양한 유형의 데이터

* 법적 근거
- 데이터 산업법 12조 

* 운영주체
- 데이터산업법 제11조, 과학기술정보통신부 등 
관계기관 지정

### [통계] 확률분포

**[정의]**

- 확률변수 x가 특정한 값을 가질 확률을 나타내는 분포 

- 이산형 확률변수=>이산형 확률분포=>확률질량함수(pmf) 
- 연속형 확률변수=>연속형 확률분포=>확률밀도함수(pdf)

**[핵심/키워드]**

이산확률분포
-이산균등 : x값 유한개(주사위1~6)
-초기하 : 불량품(10p 불량7일때 6p에 불량 5확률)
-베르누이 : 동전앞뒤, 주사위 6 나올 확률
-이항 : 독립 베르누이 n번 시행
-포아송 : 특정범위내 사건수
-기하 : 특정사건이 1번째 일어날 확률(야구에서 1번째 안타)
-음이항 : 특정사건이 n번째 일어날 확률(n번째 안타)

연속확률분포
-정규분포, 표준정규분포, 카이제곱분포 등

### [소공] 민간투자형 소프트웨어(SW) 사업 추진 가이드 2.0

**[정의]**

민간의 자본과 기술을 활용하여 시스템을 구축하고, 공공의 운영 노하우와 권한을 바탕으로 민간과 협력하여 사업을 추진하는 소프트웨어 기반 사업

* 법적근거
소프트웨어진흥법 제40조(민간투자형 소프트웨어사업)

**[핵심/키워드]**

* 사업유형
① 구매형: 민간이 이미 개발한 SW를 서비스 형태로 이용하는 사업
② 개발형: 민간이 민간자본을 선 투자하여 소프트웨어를 개발하는 사업

* 투자비 회수방식에 따른 사업유형
① 임대형(BTL, Build-Transfer-Lease) 방식
: 국가나 지자체가 지급하는 시스템(SW) 임대료 등 사용료로 투자비를 회수하는 방식
② 수익형(BTO, Build-Transfer-Operate) 방식
: 시스템(SW) 사용 요금 등 정보서비스 수익으로 투자비를 회수하는 방식

