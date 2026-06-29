---
layout: post
title: "WritingDrill_Rounds_1"
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

### [인공지능] 범용 인공지능(Artificial General Intelligence, AGI)

**[정의]**

기계가 자신의 지능을 이해하고, 학습하고, 적용하여 인간 지능과 구별할 수 없는 방식으로 문제를 해결할 수 있는 수준의 인공지능

**[핵심/키워드]**

- 레벨0 : AI 미진입
- 레벨1 : 신진(챗GPT) 
- 레벨2 : 유능함(30%) 
- 레벨3 : 전문가(10%) 
- 레벨4 : 거장(1%) 
- 레벨5 : 슈퍼휴먼 
- 딥러닝 &amp; 머신러닝, 자연어 처리, 컴퓨터 비전, 로보틱스, 추론과 결정, 심리 인식 &amp; 사회적 지능&lt;/agi&gt;&lt;/agi의&gt;

### [법제도] 민간투자형 소프트웨어 사업

**[정의]**

민간의 자본과 기술을 활용하여 시스템을 구축하고, 공공의 운영 노하우와 권한을 바탕으로 민간과 협력하여 사업을 추진하는 소프트웨어 기반 사업

**[핵심/키워드]**

&lt;법적근거&gt; 소프트웨어진흥법 제40조(민간투자형 소프트웨어사업) 

&lt;사업유형&gt;
① 구매형: 민간이 이미 개발한 SW를 서비스 형태로 이용하는 사업
② 개발형: 민간이 민간자본을 선 투자하여 소프트웨어를 개발하는 사업

### [소프트웨어공학] SW 공학(SW Engineering)

**[정의]**

질 좋은 SW를 경제적으로 생산하기 위해 공학, 과학 및 수학적 원리와 방법을 적용하는 것

**[핵심/키워드]**

&lt;구성요소&gt; 원기언도산 
- 원리, 기법, 언어, 도구, 산출물  
&lt;원리&gt; 정관모추변일점
- 정형성과 엄격, 관심사의 분리, 모듈화, 추상화, 변화예측, 일반화, 점진화

### [인공지능] 협업 필터링(Collaborative Filtering)

**[정의]**

대규모의 기존 사용자 행동 정보를 분석하여 해당 사용자와 비슷한 성향의 사용자들이 기존에 좋아했던 항목을 추천하는 알고리즘
- 유사도 기반

**[핵심/키워드]**

&lt;유형&gt;
- Memory Based
  ㄴ User Based: 비슷한 사용자 구매 상품 추천
  ㄴ Item Based: 구매 아이템 연관 상품 추천 
- Model Based
  ㄴ 기계학습: 딥러닝, 행렬분해, 특이값 분해

### [법제도] 개인정보영향평가(Privacy Impact Assessment, PIA)

**[정의]**

개인정보를 활용하는 새로운 정보시스템 도입 및 기존 시스템의 중요한 변경 시, 시스템의 구축·운영이 기업의 고객은 물론 국민 프라이버시에 미칠 영향에 대하여 미리 조사·분석·평가하는 체계적인 절차

**[핵심/키워드]**

&lt;법적근거&gt; 「개인정보 보호법」 제33조(개인정보 영향평가)

&lt;대상기관&gt; 
- 개인정보파일을 구축․운영하거나 기존 시스템을 변경 또는 연계하려는 공공기관

&lt;의무대상&gt;
- 100만 명 이상의 개인정보파일 
- 내·외부 시스템과 연계 결과, 50만 명 이상 
- 의료정보 등 민감정보 또는 주민등록번호 등 고유식별정보를 포함하여 5만 명 이상 
- 개인정보 검색체계 등 개인정보파일의 운영체계를 변경

&lt;수행단계&gt;
- 개인정보 흐름분석 
- 개인정보 침해요인 분석 
- 영향 평가서 작성

### [소프트웨어공학] 나선형(Spiral)모델

**[정의]**

시스템을 개발하면서 생기는 위험을 최소화하기 위해 나선을 돌면서 점진적으로 완벽한 시스템으로 개발하는 모델  
- 폭포수 모델 + 프로토타입 장점 수용

**[핵심/키워드]**

&lt;절차&gt; 계위개고 
- 계획, 위험분석(프로토타입), 개발/검증, 고객피드백

### [인공지능] 다중 에이전트 시스템(Multi-Agent System, MAS)

**[정의]**

여러 개의 자율적(Autonomous) 에이전트(Agent) 가 상호 협력·경쟁·조정을 통해 공동의 목표를 달성하거나 복잡한 문제를 해결하는 시스템

**[핵심/키워드]**

&lt;구성 요소&gt;
- Agent: 자율적으로 동작하는 개체 (소프트웨어, 로봇, 프로세스 등)
- Environment: 에이전트가 인식·작용하는 외부 환경
- Communication: 메시지 기반 상호작용 프로토콜
- Coordinator/Manager: 협업 조정 및 목표 분배 담당 (필요 시) 

&lt;기술요소&gt; 
- 통신·협력: FIPA ACL, KQML(에이전트 간 메시지 교환과 지식 공유를 표준화)
- 의사결정·추론: MARL, 지식기반 추론, LLM(다중 에이전트의 학습·논리적 판단·계획 수행 지원)
- 환경·시뮬레이션: NetLogo, Mesa, GAMA, JADE, SPADE(복잡한 모델링과 분산 시뮬레이션 구현)
- 플랫폼·프레임워크: CrewAI, AutoGen, LangGraph, Swarm(에이전트 협업·워크플로우 자동화·집단지능 구현)

### [법제도] 개인정보의 안전성 확보 조치 기준

**[정의]**

개인정보가 분실, 도난, 유출, 위조, 변조 또는 훼손되지 아니하도록 안전성 확보에 필요한 기술적, 관리적 및 물리적 안전조치 수립 기준

**[핵심/키워드]**

&lt;법적근거&gt; 개인정보 보호법 제29조(안전조치의무) 
&lt;주요개정내용&gt; 
- 제6조 접근통제(외부접속 인증) 
- 제6조 인터넷망 차단 
- 제6조의2 인터넷망 차단(신설) 
    ㄴ일평균 이용자 100만명 이상 시
       ① 접근 권한 설정 가능자
       ② 개인정보 다운로드·파기 가능자 PC인터넷망 차단
     ㄴ 위험 분석 결과에 따라 예외 허용
     ㄴ 단,민감정보 등은 예외 불가
- 제8조 접속기록 보관 대상
- 제8조 접속기록 점검 방식

### [소프트웨어공학] 클린룸(Clean Room) 모델

**[정의]**

공식명세(FormalSpecification)와 수학적 기법을 활용하여 오류를 최소화하고 고품질 소프트웨어를 개발하는 SDLC 모델

**[핵심/키워드]**

&lt;절차&gt;
- 요구사항 수집 및 분석 → 박스 구조 명세 → 정형 설계 →
정확성 검증 → 코드 생성 → 코드 검증 → 통계적 사용 테스트 → 인증

&lt;상세화 검증방법&gt; 블상클 
- 블랙박스: 입력부터 출력까지의 데이터 흐름 확인 
- 상태박스: 블랙박스를 내부 기능 표현 
- 클리어박스: 상태박스에 제어 흐름 추가

### [인공지능] 적대적 공격(Adversarial Attack)

**[정의]**

딥러닝의 심층신경망을 이용한 모델에 적대적 교란을 적용하여 오분류를 유발하고 신뢰도 감소를 야기하는 머신러닝 공격기법

**[핵심/키워드]**

&lt;공격유형&gt; 포모도회
- 포이즈닝 공격: 잘못된 학습데이터 주입
- 모델 추출 공격: 반복적인 질의에 의한 답으로 인공지능의 동작을 모사
- 도치 공격: 반복적 질의로 학습에 사용된 데이터 추출
- 회피 공격: 분류 데이터 변조하여 오인식 유도 

&lt;대응방안&gt; 예탐차은 
- 사용자 인증(행위, 생체신호 기반, 환경 기반)
- CAPTCHA, DefenseGan
- 이상 거래 탐지 
- 신용 예측(오버샘플링, 기존 데이터 합성)

### [법제도] 정보보호 공시 제도

**[정의]**

이용자의 안전한 인터넷 이용 및 정보보호 투자 활성화를 위하여 정보보호 투자/인력/인증/활동 등 기업의 정보보호 현황을 일반에 공개하는 자율·의무공시제도

**[핵심/키워드]**

&lt;법적근거&gt;
- 「정보보호산업의 진흥에 관한 법률」제13조(정보보호 공시), 동법 시행령 제8조(정보보호 공시)

&lt;공시항목&gt; 투인평활
1) 정보보호투자액
2) 정보보호인력
3) 정보보호인증/평가
4) 정보보호활동

&lt;의무대상&gt;
- IDC, ISP, CSP, 상급종합병원

&lt;예외대상&gt; 소금공전
- 소기업, 금융회사, 공공기관, 전자금융업자

### [소프트웨어공학] 정보공학 방법론 (InformationEngineeringMethodology)

**[정의]**

기업 전체 또는 기업의 주요부분을 계획, 분석, 설계 및 구축에 정형화된 기법들을 상호 연관성 있게 통합, 적용하는 데이터 중심 방법론

**[핵심/키워드]**

&lt;단계&gt;
정보전락계획(ISP) → 업무영역분석(BAA) → 업무시스템설계(BSD) → 시스템구축(BSC)

### [인공지능] 강화학습(Reinforcement Learning, RL)

**[정의]**

데이터의 상태를 인식하고 이에 반응한 행위에 대하여 환경으로부터 받는 포상을 학습하여 행위에 대한 포상을 최적화하는 정책을 찾는 기계학습

**[핵심/키워드]**

&lt;유형&gt; 
1) Model Free
- 정책 기반 방법(Policy-based): 직접 정책을 최적화하여 최적의 행동을 학습
- 가치 기반 방법(Value-based): Q-러닝(Q-Learning)처럼 가치 함수를 학습하여 최적 행동 선택 
2) Mode Based
- 모델 기반 방법 (Model-based)- 환경의 동적 모델을 학습하여 최적의 행동 결정 
3) Model-Free + Model-Based (혼합형)

<데이터를 학습하는 방식에 따른 분류 ‘On-Policy vs Off-Policy’>
- Model-Free RL(모델 없이 학습)에 적용 
- On-Policy : 현재 실행 중인 정책(Policy)을 사용하여 학습
- Off-Policy : 과거 경험 데이터를  재사용하여 학습 (Replay Buffer 사용)

### [법제도] 데이터 안심 구역

**[정의]**

법적 기준(데이터산업법 등)에 따라 지정, 미개방 데이터 등 민감한 데이터를 안전하게 분석·활용할 수 있는 구역

**[핵심/키워드]**

&lt;법적근거&gt; 데이터산업법 제11조,시행령 제12·13조 

&lt;제공서비스&gt; 
- 다양한 유용한 분석 데이터 
- 안전하고 수준 높은 분석 환경 
- 누구나 활용 가능한 분석 서비스 
- 이해하기 쉬운 분석 사례

### [소프트웨어공학] 객체지향 설계 5대 원칙(SOLID원칙)

**[정의]**

객체지향방법론이 지향하는 재사용과 유지보수 극대화를 달성하기 위한 클래스 단위에서의 설계 원칙

**[핵심/키워드]**

&lt;응집도 증가&gt; SI
- 단일 책임 원칙(SRP)
- 인터페이스 분리 원칙(ISP)

&lt;결합도 감소&gt; OLD
- 개방-폐쇄 원칙(OCP)
- 리스코프 치환 원칙(LSP)
- 의존 역전 원칙(DIP)

### [인공지능] 민코프스키 거리(Minkowski Distance)

**[정의]**

맨하탄거리와 유클리드 거리를 한번에 표현한 거리 척도

### [법제도] EU_디지털 서비스법 (DSA)

**[정의]**

온라인 플랫폼과 디지털 서비스 제공자의 책임성과 투명성을 대폭 강화하는  유럽연합(EU)의 혁신적 규제 법안

**[핵심/키워드]**

&lt;특별 규제 대상&gt; 
- 월간 활성 이용자 4,500만 명 이상 또는 EU 전체 인구의 10% 이상을 보유한 '초대형 온라인 플랫폼(VLOPs)' 및 '초대형 온라인 검색엔진(VLOSEs)'은 가장 엄격한 규제를 적용

&lt;VLOP 주요 의무 사항&gt;
- 시스템 리스크 평가 및 관리
- 외부 감사 
- 투명성 강화

### [소프트웨어공학] CBD(Component-BasedDevelopment,컴포넌트 기반 개발)

**[정의]**

기 개발된 SW 컴포넌트를 조립, 시스템을 개발하여 객체지향의 단점인 SW 재사용성을 극대화한 개발방법론

**[핵심/키워드]**

&lt;컴포넌트 개발단계&gt; 
- 분설추설구: 도메인 분석→도메인 설계→컴포넌트 추출→ 컴포넌트 구현
- 검형인: 검색←형상관리←컴포넌트 인증
- 응조기분정: 응용시스템←컴포넌트 조립←컴포넌트 기반설계←영역분석←요구사항 정의)

&lt;사례&gt;
- 마르미3: 국내환경 적합하게 개발 
- 마르미4(EMMA): 임베디드 시스템 개발 목적

### [인공지능] K-평균 군집(K-Means Clustering)

**[정의]**

데이터의 유사성을 기반으로 최적의 중심점을 찾아 K개의 그룹으로 분류하는 방법

**[핵심/키워드]**

&lt;절차&gt;
1) 군집 수 K를 정의하여 임의 위치 지정(initial Centroids)
2) 모든 데이터들의 거리 계산 후 가장 가까운 중심점 기준으로 군집화 
3) 각 군집마다 계산하여 새로운 중심 계산 
4) step 2~3을 반복, 클러스터가 변경되지 않으면 학습 완료

### [법제도] 지식재산 기본법

**[정의]**

지식재산의 창출ㆍ보호 및 활용을 촉진하고 그 기반을 조성하기 위한 정부의 기본 정책과  추진 체계를 마련하여 우리 사회에서 지식재산의 가치가 최대한 발휘될 수 있도록 하는  법률(2011.7.20. 최초 시행)

**[핵심/키워드]**

&lt;지식재산권 유형&gt; 
- 산업재산권: 특허권, 실용신안권, 디자인권, 상표권
- 저작권: 협의의 저작권, 저작 인접권
- 신지식 재산권: 첨단 산업 재산권, 산업 저작권, 정보재산권, 기타

### [소프트웨어공학] 프로덕트 라인 (Product Line, SPL)

**[정의]**

제품/서비스 군별로 SW핵심자산을 개발하고 이를 관리/조직적인 재사용을 통해 경제적인 SW제품을 생산하여 SW재사용성과 생산성을 극대화 하기 위한 개발방법론 

- 제품들에 사용되는 모든 S/W산출물을 재사용

**[핵심/키워드]**

&lt;구성요소&gt; 
- Domain 공학(CoreAssetDevelopment) 
- Application 공학(Product Development) 
- Management 

<개발방법(종류)> PREI 
- Proactive Reactive Incremental

### [인공지능] 자기조직화 지도(Self-Organizing Map, = 코헤넨 맵, Kohonen map)

**[정의]**

대뇌피질의 시각피질의 학습 과정을 모델화한 인공신경망으로, 자율학습에 의한 클러스터링을 수행하는 알고리즘

**[핵심/키워드]**

&lt;특징&gt; 
- 비지도 학습
- 데이터의 고차원 구조를 저차원으로 변환
- 경쟁 학습(Competitive Learning)
- 연속적인 군집화 결과를 제공
 
&lt;핵심 개념&gt; 
- 뉴런(Neuron) 그리드
- 맵 크기(Grid Size, M×N)
- 승자 뉴런(BMU, Best Matching Unit)
- 가중치 업데이트
- 이웃 함수 (Neighborhood Function)

### [법제도] 개인정보 이노베이션 존

**[정의]**

데이터 처리 환경의 안전성을 높여 가명정보를 보다 유연하게 활용할 수 있도록 지원하는 공간

**[핵심/키워드]**

&lt;법적근거&gt;개인정보보호법 제28조의7 

&lt;주요기능&gt; 
- 개인정보 (가명정보)의 유연한 활용 지원 
  ㄴ가명처리 수준 완화 
  ㄴ 비정형데이터 활용 
  ㄴ 가명정보 장기보관 및 재사용 
- 개인정보보호 강화기술 (PET)실증 지원 
  ㄴ PET를 적용한 개인정보 처리 허용

### [소프트웨어공학] 도메인 주도 설계(Domain-Driven Design)

**[정의]**

복잡한 소프트웨어 설계에서 비즈니스 도메인(업무영역)을 중심으로 모델을 구축하는 설계 방법론

**[핵심/키워드]**

&lt;전략적 설계&gt; 기본설계,분석단계 
- 구성요소 
  ㄴ 도메인과 서브도메인
  ㄴ 유비쿼터스 언어
  ㄴ 바운디드 컨텍스트
  ㄴ 이벤트 스토밍
  ㄴ 헥사고날 아키텍처 매핑

&lt;전술적 설계&gt; 상세설계,설계단계

### [인공지능] 차원 축소 알고리즘 (Dimensionality Reduction Algorithms)

**[정의]**

고차원 데이터를 저차원으로 변환하여 데이터의 중요한 정보를 유지하면서 연산 비용을 줄이는 기법

**[핵심/키워드]**

&lt;차원축소 알고리즘&gt; 
- 선형 차원 축소 (Linear Dimensionality Reduction)
  ㄴ PCA (Principal Component Analysis, 주성분 분석)
  ㄴ LDA (Linear Discriminant Analysis, 선형 판별 분석)
  ㄴ FA (Factor Analysis, 요인 분석)

- 비선형 차원 축소 (Non-Linear Dimensionality Reduction)
  ㄴ t-SNE (t-Distributed Stochastic Neighbor Embedding)
  ㄴ UMAP (Uniform Manifold Approximation and Projection)
  ㄴ Isomap (Isometric Mapping)
  ㄴ LLE (Locally Linear Embedding, 국소적 선형 임베딩)

- 신경망 기반 차원 축소 (Deep Learning-Based Dimensionality Reduction)
  ㄴ Autoencoder
  ㄴ Variational Autoencoder (VAE)
  ㄴ RBM (Restricted Boltzmann Machine)

- 행렬 분해 기반 차원 축소 (Matrix Factorization)
  ㄴ SVD (Singular Value Decomposition, 특이값 분해)
  ㄴ NMF (Non-Negative Matrix Factorization, 비음수 행렬 분해)
  ㄴ MDS (Multidimensional Scaling, 다차원 척도법)

### [법제도] EU, AI ACT법

**[정의]**

EU 내 인공지능(AI)의 개발, 사용, 유통을 규율하는 규정

**[핵심/키워드]**

- 세계 최초의 포괄적인 AI 법률로, EU가 AI 분야에서 글로벌 리더십을 확보하기 위한 중요한 조치

### [소프트웨어공학] XP(eXtreme Programming, 익스트림 프로그래밍)

**[정의]**

짧은 주기의 반복을 통해 요구변화에 신속하게 대응하여 위험을 줄이고 고객 관점의 고품질 SW를 빠르게 전달하는 Agile 방법론

**[핵심/키워드]**

&lt;핵심가치&gt; 용단커피존 
- 용기, 단순성, 커뮤니케이션, 피드백, 존중 

&lt;12가지 실천사항&gt; 개관구환, 페공지 개짤메 간테리 4고코
- 개발원리: 페어프로그래밍, 공동책임, CI
- 관리원리: 개발계획,small Release, 구조
- 구현원리: 간략디자인,Test Driven, 리팩토링
- 환경요소: 40hour week, 고객상주, 코드표준화

&lt;구성&gt; 
- 유저스토리(User Story) 작성→구조적 스파이크(Architectural Spike)→릴리즈 계획(Release Plan)→반복(Iteration)→인수테스트(Acceptance Test)→작업 배포(Small Release)

### [인공지능] 의사결정나무(Decision Tree)

**[정의]**

분류함수를 의사결정규칙으로 표현할 때 타원, 직선, 사각형을 이용하여 나무형태로 그려서 분석하는 도구 

- 분류나무트리 → 범주형 
- 회귀나무트리 → 연속형

**[핵심/키워드]**

&lt;과정&gt; 변성가타분
1) 변수선택: 종속변수와 관계있는 독립변수 선택
2) 의사결정나무 형성: 분석목적과 자료의 구조에 따라 적절한 분리기준과 정지규칙을 정하여 의사결정나무 구조 작성 
3) 가지치기: 부적절한 가지제거
4) 타당성 평가: 이익, 위험, 비용 등을 고려하여 모델 평가 
5) 분류 및 예측: 분류 및 예측 수행  

&lt;마디 분리 기준&gt;
- 불순도: 다양한 범주들의 개체들이 얼마나 포함되어 있는가
- 순수도: 목표변수의 특정 범주에 개체들이 포함되어 있는 정도 

&lt;알고리즘&gt; 
- ID3, CHAID, CART, C4.5/C5.0

### [법제도] AI기본법(인공지능 발전과 신뢰 기반 조성 등에 관한 기본법) 시행령

**[정의]**

인공지능의 건전한 발전을 지원하고 인공지능사회의 신뢰 기반 조성에 필요한 기본적인 사항을 규정 한 시행령

**[핵심/키워드]**

&lt;내용&gt; 
- 국가 AI 거버넌스 확립 
  ㄴ 인공지능 기본계획의 수립 
  ㄴ 인공지능정책센터의 지정 
  ㄴ 인공지능안전연구소의 운영 

- AI산업 육성 지원 
  ㄴ 학습용데이터 지원 대상 사업의 기준 및 통합제공시스템 구축 
  ㄴ 인공지능집적단지 지정 기준 및 절차 

- 안전 신뢰 기반 조성 
  ㄴ 22조 인공지능 투명성 확보 의무의 이행 방법 및 예외 
  ㄴ 23조 인공지능 안전성 확보 의무의 대상 인공지능시스템 기준 
  ㄴ 24조 고영향 인공지능 확인 
  ㄴ 26조 고영향 인공지능 사업자 책무 
  ㄴ 27조 고영향 인공지능 영향평가의 포함사항

### [소프트웨어공학] 패어 프로그래밍(PairProgramming, 짝 프로그래밍)

**[정의]**

하나의 컴퓨터에서 두사람의 프로그래머가 개발을 진행하는 방식

**[핵심/키워드]**

&lt;역할&gt; 
- Driver: 실제 코딩을 수행하는 프로그래머, 지시를 수행하는 역할
- Partner: Driven에게 방향과 전략을 지시하는 네비게이터 역할

### [인공지능] 로지스틱 회귀분석(Logistic Regression Analysis)

**[정의]**

분석 대상들이 여러 집단으로 나누어진 경우, 독립변수의 선형 결합을 이용하여 개별 관측치가 어느 집단에 속하는지 확률을 계산하는 분류기법

**[핵심/키워드]**

1) 확률의 선형 모델 표시
2) 오즈(odds)적용: 양의값 무한대
3) 로짓(Logit)적용: 음의값 무한대
4) 판별 함수: 선형함수 사용
5) 시그모이드: 로짓함수의 역함수

### [법제도] 전자정부 프레임워크 5.0

**[정의]**

공공 정보시스템 구축 시 표준화·재사용·품질 향상을 목적으로 제공되는 JAVA기반 Spring 중심 오픈소스 Apache2.0
웹 애플리케이션 프레임워크 (25년 12월, 5.0버전 발표)

**[핵심/키워드]**

<5.0 버전 변경사항> 
- 생성형 AI 기반 RAG 적용 템플릿 
- 클라우드 네이티브 강화: Kubernetes + IStio도입 트래픽 보안 강화 
- 개발환경 (Eclipse): GitHub Copilot 공식 지원
- VSCode Extension지원: 프로젝트 템플릿 생성

### [소프트웨어공학] MDA(Model Driven Architecture)

**[정의]**

메타모델을 기반으로 구현환경에 독립적 모델을 자동으로 각 구현환경에 적합한 구현 종속적 모델로 변환하게 하는 SW개발 아키텍처

**[핵심/키워드]**

&lt;구성요소&gt; MUCX
- MOF: (메타모델)모델 정보에 대한 표준적인 저장소 제공 
- UML: (표기법)객체 및 컴포넌트 시스템을 표현하기 위한 표준언어
- CWM: (저장소)데이터베이스 모델과 스키마 변환 모델 
- XMI: (매핑)MOF 기반 모델을 XML로 매핑하기 위한 표준 사양 

&lt;모델&gt; 
- 비즈니스 모델(CIM) 
- PIM모델(PlatformIndependentmodel) 
- PSM모델(Platform Specific model)

### [인공지능] 앙상블 알고리즘 (Ensemble Algorithms)

**[정의]**

일련의 분류 기준을 구성한 후 예측 가중치 투표를 통해 새로운 데이터를 분류하는 방식

**[핵심/키워드]**

&lt;특징&gt;
- 성능 향상, 과적합 방지, 편향-분산 트레이드오프 최적화, 모델 안정성 향상

&lt;유형&gt; 
- 동일모델(데이터 다양성 부여): 보팅, 배깅(랜던포레스트), 부스팅
- 여러개 모델 결합(알고리즘 다양성 부여): 보팅, 스태킹, 블랜딩

### [법제도] ISO/IEC 33000

**[정의]**

소프트웨어 및 시스템 개발 프로세스의 평가 및 개선을 위한 국제 표준

**[핵심/키워드]**

- 표준구조: 모듈형 구조로 통일 
- 용어체계: 용어와 개념 정비 
- 적용분야: 다양한 산업 적용 가능 
- 개발방식: 애자일·DevOps 반영 
- 평가체계: 공통 평가 프레임 제공

### [소프트웨어공학] CI(Continuous Integration)/CD(Continuous Delivery)

**[정의]**

- CI: 여러명으로 구성된 팀이 개발한 SW를 지속적으로 통합하고 품질통제 하는 Agile Practice 

- CD: 변경된 요구사항에 대한 개발/통합/배포/테스트/릴리즈를 자동화하여 SW 개발과 운영을 통합하는 DevOps를 지원하는 연속적인 배포 출시 전략

**[핵심/키워드]**

&lt;단계&gt; 
- CI: Build→Unit/Integration Tests 
- CD: CI+Deploy to Stage + Acceptance Tests(Auto) → Deploy to Production(Manual)

### [인공지능] 혼동 행렬(Confusion matrix = 오분류표)

**[정의]**

분류 모델의 성능을 평가하는 데 사용되는 중요한 도구

**[핵심/키워드]**

&lt;구성요소&gt;
- 정확도(Accuracy): (TP + TN) / (TP + TN + FP + FN)
- 정밀도(Precision): TP / (TP + FP)
- 재현율(Recall): TP / (TP + FN)
- 특이도(Specificity): TN / (TN + FP)

### [법제도] ISO/IEC TS 42119-2:2025

**[정의]**

AI시스템의 생명주기와 리스크를 기반으로 테스트 수준·유형·설계 기법을 체계적으로 제시한 AI테스트 기술명세서 
- TS(TechnicalSpecification):준 표준

**[핵심/키워드]**

&lt;목적&gt;
- AI시스템의 신뢰성·안정성·일관성 확보
- AI개발·운영 과정에서 품질 리스크 최소화
- 조직 차원의 AI품질 관리체계 구축 지원 

&lt;적용 대상&gt;
- AI모델·AI기반 서비스·AI시스템을 개발·운영하는 조직
- 공공·민간,산업 분야 전반에 적용 가능
- 고위험·중요 AI활용 영역에서 특히 유효

### [소프트웨어공학] DI(Dependency Injection, 의존성 주입)

**[정의]**

각 클래스 사이의 의존관계를 Bean 설정 정보를 바탕으로 컨테이너가 자동적으로 연결해 주는 기술

**[핵심/키워드]**

<의존성 주입(DI) 방식>
1) 생성자 주입(Constructor Injection):생성자 이용하여 의존성 주입
2) 필드 주입(Field Injection):멤버 변수(필드)에 직접 주입
3) Setter 주입(Setter Injection):setter 메소드를 통해 의존성 주입 
4) 메소드 주입(Method Injection):특정 메소드 실행 시점에만 의존성 주입

&lt;구현 방법&gt;
- XML 기반 : 설정과 코드 분리
- Annotation 기반 : 간결한 설정
- XML + Annotation 혼합 : XML 가독성과 Annotation 편리함 결합

### [인공지능] 하이퍼파라미터 최적화(Hyperparameter Optimization)

**[정의]**

모든 기계학습 모델(알고리즘)은 고유한 하이퍼파라미터를 갖고 있고,그 값에 따라 성능 차이 발생 가능 

- 모델링할 때 '사용자가 직접 세팅' 해주는 값

**[핵심/키워드]**

&lt;구분&gt;
- 블랙박스 최적화(Black-Box Optimization) 
  ㄴ Grid Search (격자 탐색) 
  ㄴ Random Search (랜덤탐색) 
  ㄴ Bayesian Optimization(베이지안 최적화) 
  ㄴ Simulated Annealing(시뮬레이티드 어닐링) 
  ㄴ Genetic Algorithms(유전 알고리즘)

- 다중 충실도 최적화(Multi-Fidelity Optimization) 
  ㄴ Modeling Learning Curve (학습 곡선 모델링) 
  ㄴ Bandit Based (밴딧 기반 탐색) 
  ㄴ Successive Halving(순차적 절반 선택) 
  ㄴ Hyper-Band(하이퍼밴드 알고리즘)

### [법제도] ISO/IEC AWI TS 42119-7

**[정의]**

AI레드팀 테스팅에 대한 용어,절차,방법들을 정의한 AI레드팀에 대한 최초의 국제 공통 표준
- AWI(ApprovedWorkItem)상태로 개발 중

**[핵심/키워드]**

&lt;특징&gt;
- AI레드팀 테스팅 지침 제공
- 잠재적 위험 식별
- 기술 중립적

### [소프트웨어공학] SOAP(Simple Object Access Protocol)

**[정의]**

XML기반의 메시징 형식을 사용하여 플랫폼 및 프로그래밍 언어에 독립적인 방식으로 데이터 교환을 지원하는 웹서비스(WebService)간 메시지를 교환하기 위한 프로토콜

**[핵심/키워드]**

&lt;특징&gt; 
- XML기반 메시징 프로토콜,HTTP등 전송 프로토콜 지원,보안성 강함,트랜잭션 지원,REST대비 성능 낮음

&lt;동작과정&gt;
- WSDL을 통해 명확한 인터페이스를 공유하여 통신하는 구조
- WSDL(WebServicesDescriptionLanguage):서비스의 인터페이스,요청 및 응답 구조를 기술하는 XML문서

&lt;구성요소&gt;
- Envelope : SOAP 메세지의 루트요소
- Header : 인증,보안,트랜잭션 등의 메타데이터 포함
- Body : 실제 요청 또는 응답 데이터가 포함됨

### [인공지능] 손실함수(Loss Function = Cost Function)

**[정의]**

신경망(딥러닝 모델)의 예측값과 실제값(정답)간의 차이를 수치화하여 측정하는 함수

- 예측치와 실측치의 오차를 표현하는 함수

**[핵심/키워드]**

&lt;역할&gt; 
- 예측 성능 평가, 경사하강법 최적화, 오차 피드백

### [법제도] ISO/IEC 5230

**[정의]**

오픈소스 라이선스 컴플라이언스 관리에 관한 표준

**[핵심/키워드]**

&lt;목적&gt; 
- 소프트웨어 공급망 내에서 신뢰할 수 있는 오픈소스 라이선스 컴플라이언스 프로그램의 핵심 요구사항을 정의하여 조직 간의 신뢰를 구축하는 데 중점 

&lt;주요내용&gt; 
1\. 명확한 오픈소스 정책 수립.
2\. 라이선스 의무 식별 및 추적을 위한 프로세스 구현 (SBOM 생성 포함) 
3\. 컴플라이언스 산출물 생성 및 제공 

&lt;의의&gt; 
- 오픈소스 사용 시 발생할 수 있는 법적, 재정적, 평판적 위험을 줄이고 효율적인 라이선스
관리 체계를 구축

### [소프트웨어공학] 아키텍처 드라이버(Architecture Driver)

**[정의]**

아키텍처 결정에 영향을 주는 요구사항

**[핵심/키워드]**

&lt;구성요소&gt; 기제품 
- 기능 요구사항:시스템이 수행해야 할 핵심 기능
- 제약사항: 비기능 요구사항
- 품질속성: SW품질을 결정하는 주요 요소(품질 요구사항:성능,가용성,보안성,유지보수성)

### [인공지능] 기울기 소멸 문제(Vanishing Gradient)

**[정의]**

역전파 알고리즘을 학습을 통해 가중치를 수정할 때, 은닉층으로 오차가 거의 전달되지 않는 문제

**[핵심/키워드]**

&lt;발생원인&gt; 
- Data set 부족
- 컴퓨터 파워 부족
- 초기 가중치 값 오류
- 활성함수 선택 오류 
 
&lt;해결방안&gt; 
- Drop out, GPU 활용, ReLU 활성화 함수 적용, 사전학습, 데이터 스케일링

### [법제도] ISO/IEC 18974

**[정의]**

오픈소스 소프트웨어 보안 보증에 관한 표준

**[핵심/키워드]**

&lt;목적&gt; 
- 오픈소스 관리 체계를 '법적 준수'에서 '보안 보증'으로 확장 , 오픈소스 소프트웨어 사용과 관련된 보안 위험을 관리하기 위한 핵심 요구사항을 정의 

&lt;주요내용&gt; 
1\. 알려진 보안 취약점(예: CVE)에 대한 확인 및 관리 프로세스.
2\. SBOM(Software Bill of Materials)을 활용한 지속적인 보안 점검 
3\. 외부의 취약점 문의에 대응하는 방법 마련

&lt;의의&gt; 
- 소프트웨어 공급망 전반 걸쳐 오픈소스의 보안 취약점을 체계적 관리하고 대응 능력 강화

### [소프트웨어공학] 아키텍처 스타일(ArchitectureStyle)

**[정의]**

아키텍처 설계시 반복해서 발생하는 문제를 해결하고 만족시켜야 할 품질 속성을 달성할 수 있는 방법을 정리한 SW 아키텍처 Best Practice

**[핵심/키워드]**

&lt;대표 스타일&gt; RMCLDB
- Repository 
- MVC
- 클라이언트/서버구조 
- Data Flow
- Layered
- BlackBoard

### [인공지능] 변분 오토인코더(Variational Autoencoder, VAE)

**[정의]**

입력 데이터를 확률적 잠재 공간에서 학습하여 새로운 데이터를 생성하는 신경망 알고리즘

**[핵심/키워드]**

&lt;아키텍처&gt; 
- 입력층 (InputLayer)
- 인코더 (Encoder) 
- 잠재 변수 (LatentVariables,z) 
- 샘플링(Sampling,ReparameterizationTrick) 
- 디코더 (Decoder) 
- 출력층 (OutputLayer) 
- 손실 계산 (LossCalculation) 
- 모델 업데이트  

&lt;기술요소&gt; 
- 잠재 공간 (Latent

### [법제도] 제로트러스트 가이드라인 2.0(2024.12)

**[정의]**

기존 1.0(2023.7)의 원칙 기반 프레임워크를 바탕으로 국내 조직들이 실제 제로트러스트 보안 체계를 설계·구축·운영할 수 있도록 실질적 지침과 절차를 구체화한 개정판

**[핵심/키워드]**

&lt;주요내용&gt; 
- 성숙도 모델, 도입 절차 상세화 등으로 실질적인 Zero Trust 도입 장벽 낮춤 
- 성숙도 4단계로 세분화: 기존환경, 초기, 고급, 최적 
- 52가지 세부역량 및 평가 체크리스트 제공 
- 도입절차: 준비 > 계획 > 구현> 운영 > 피드백 및 개선(5단계 )

### [소프트웨어공학] ISO/IEC42010:2022

**[정의]**

아키텍처 표현을 위한 요소 및 이들 관계를 일반화하여, 다양한 SW 시스템에서 활용할 수 있도록 하는 아키텍처 명세를 정의하는 메타모델

**[핵심/키워드]**

&lt;구성요소&gt; 
-42010:2022 인민아스스아래 컴커커 뷰뷰아 모컴레 
- Environment(외부맥락), Entity of Interest(대상엔티티), Stakeholder(이해관계자), Stakeholder Perspective(이해관계자관점), Concern(관심사), Architecture(아키텍처), Architecture Description(아키텍처기술서), Architecture Rationale(설계근거), Architecture Viewpoint(관점템플릿), Architecture View(아키텍처시각), Model Kind(모델유형), View Component(뷰구성요소), Architecture Aspect(아키텍처관점), Correspondence(대응관계), Correspondence Method(대응방법), Legend(기호설명)

### [인공지능] 지식 그래프(KnowledgeGraph)

**[정의]**

개체-관계-속성 정보를 연결하여 그래프로 구조화한 지식 표현 방식의 거대한 데이터 베이스 

- LLM + KG = 자연어 이해와 지식 구조의 결합 → 환각 줄이고, 정확한 QA·추론·전문성·설명가능성 강화

**[핵심/키워드]**

&lt;특징&gt; 
- 그래프 구조·의미 기반·추론 가능·확장성·통합성 

&lt;표현 요소&gt; 온톨로지
- RDF(Resource Description Framework)
- OWL(Web Ontology Language)
- SPARQL(질의 언어)
- Embedding(지식 그래프 임베딩)
- Triple(주어–술어–목적어 구조) 

&lt;구성 절차&gt; 
- 지식 수집 (텍스트, DB, 로그 등에서 개체·관계 추출)
- 지식 정규화 (개체 통합, 관계 표준화)
- 그래프 구축 (노드/엣지로 모델링, Triple 생성)
- 지식 저장/관리 (그래프 DB, 예: Neo4j)
- 질의/추론 (SPARQL, 규칙 기반, 임베딩 활용)
- 지식 확장 (새로운 데이터 반영, 지속적 업데이트)

### [법제도] SBOM(Software Bill of Materials)

**[정의]**

SW 구성요소를 서술하는 일종의 메타 데이터로 SW 전체의 구성요소를 목록화한 것

**[핵심/키워드]**

&lt;필요성&gt; 
- 투명성, 책임성, 식별성, 보안관리
&lt;구성요소&gt; 
- 공급자명 
- 타임스탬프 
- 저작권자 
- 구성요소명 
- 버전 
- 고유 식별자 
- 종속성 관계

### [소프트웨어공학] CBAM(CostBenefit Analysis Method)

**[정의]**

경제적 의사결정에 대한 요구를 충족 시키기 위해 SEI에서 ATAM을 바탕을 SW 아키텍처 분석에 중점을 둔 경제적 모델링 방법

**[핵심/키워드]**

&lt;특징&gt; 
- ATAM강화(경제성),품질과 비용간이 균형 유지,ROI계산 

&lt;평가 프로세스&gt; 
시나리오 결정→효용-반응곡선 작성→아키텍처 접근법의 경제적 분석→아키텍처 접근법 선택 및 검증

### [인공지능] 휴머노이드 로봇 (Humanoid Robot)

**[정의]**

인간과 유사한 형태와 동작을 갖춘 로봇으로, AI·로보틱스·센서 기술이 결합되어 인간과 상호작용이 가능한 로봇

**[핵심/키워드]**

&lt;유형&gt; 
- 외형 기반 분류: 완전/부분/기능특화형 휴머노이드
- 기능 및 역할 기반 분류: 산업용/서비스/의료/연구 및 실험용 휴머노이드 
- 이동방식에 따른 분류: 이족보행형/바퀴기반/혼합형 
- 기타: 감정소통형 

&lt;기술요소&gt; 
- 센싱시스템: 카메라, 각종 센서 
- 인공지능 시스템: AI반도체, 시스템 SW, 애플리케이션 SW, LLM 
- 액추에이터 시스템: 서보시스템, 모터, 감속기, 제어기 
- 바디 및 기타시스템: 금속합금, 카본파이버, 플라스틱 파트, 배터리 팩

### [법제도] 개인정보중심설계 시범인증제도(2024.04)

**[정의]**

스마트 가전·IoT 제품 개발 시 PbD 원칙을 적용하여 71개 인증 항목 기반 기술·절차·조직 적합성을 검증하고, 보완 후 공식 인증을 부여하는 시범제도 (23년 시작, 현 4개 제품 인증) 
- 디바이스 중심의 Privacy engineering 도입

**[핵심/키워드]**

&lt;평가항목&gt;
1.기본요구사항: 개인정보 관련 기본사항 
2.적법성: 개인정보 처리의 적법성 
3.보안 및 조직체계: 정보보안 및 프라이버시 강화, 조직적 보호조치  
&lt;인증절차&gt; 
1단계: 선정 및 신청 
2단계: 기술평가 및 시험 
3단계: 보완 후 인증 부여

### [소프트웨어공학] 마이크로 서비스 아키텍처(Microservices Architecture,MSA)

**[정의]**

대용량 웹 서비스 개발에 맞는 구조로 사상이 경량화되고, 대규모 개발팀의 조직 구조에 맞도록 변형된 아키텍처
- 클라우드 네이티브 기본 사상

**[핵심/키워드]**

&lt;구성요소&gt; 
- 서비스(Services), APIGateway, 서비스 디스커버리(ServiceDiscovery), 메시지 브로커, 데이터 저장소, 컨테이너 오케스트레이션, 모니터링 및 로깅 
 
&lt;아키텍처 구분&gt;
- InnerArchitecture(내부 아키텍처): 서비스 실행 환경,서비스 메시,백엔드 서비스,모니터링/진단 등 MSA운영의 핵심 요소
- OuterArchitecture(외부 아키텍처): API

### [인공지능] 가디언 에이전트(Guardian Agent)

**[정의]**

AI시스템의 안전성,신뢰성,윤리성 확보를 위해 AI를 감시·감독·제어하는 보조 AI또는 시스템

**[핵심/키워드]**

&lt;모니터링 대상&gt;
- 입력 데이터 감시: 유해/비정상 입력 탐지 
- 출력 데이터 감시: 오류·편향된 결과 감지 
- 의사결정 과정 감시: 모델 내부 판단 흐름 추적 
- 상황 환경 감시: 외부 환경 변화 감지 
- 상황 인지 감시: 시스템 반응 및 판단 적절성 평가 
- 로그 및 감사 기록: 전체 행위 기록 및 사후 감사 용도

&lt;통제 대상&gt;
- 행동 중단: 위험 시 모델 동작 강제 중지 
- 행동 변경: 안전한 대안 행동으로 전환 
- 자동 복구: 장애 발생 시 자동 복원 조치 
- 모델 업데이트 제어: 검증되지 않은 업데이트 차단 또는 승인 필요 

&lt;주요 역할&gt;
- 패턴 분석: 이상 행위 탐지를 위한 입력·출력·행동 흐름 분석 
- 신뢰도 분석: 모델 판단의 일관성·안정성 평가 
- 설명가능성(XAI): 의사결정 과정에 대한 인간이해 가능한 설명 제공 
- 정책 기반 제어: 사전 정의된 정책에 따라 모델 행동 제약 또는 조정

### [법제도] 국가 인공지능(AI) 컴퓨팅센터

**[정의]**

대규모 GPU·AI반도체 기반의 슈퍼컴퓨팅 인프라를 민·관 합작으로 구축하여,산업·연구계의 AI연구개발 및 서비스 활용을 지원하는 국가 핵심 거점 인프라

**[핵심/키워드]**

&lt;AI 데이터 센터의 주요 기술요소&gt;
- GPU클러스터:대규모 GPU서버
- 고속 네트워크:NVLink,InfiniBand,400G/800G이더넷
- 전력 인프라:고밀도 전력 공급,UPS,PDU
- 냉각 시스템:수랭,공랭,액침,HVAC
- 스토리지 인프라:NVMe SSD,분산 파일시스템
- AI플랫폼/운영 SW:컨테이너,오케스트레이션,MLOps
- 운영/관리 자동화:DCIM,모니터링·관제,AI기반 장애 예측
- 보안 인프라:네트워크/데이터 암호화,접근통제,망분리
- 친환경/지속가능성:재생에너지(PPA등)
- 확장성/유연성:모듈형 데이터센터,스케일아웃 설계

### [소프트웨어공학] 파이썬(Python)

**[정의]**

1991년 프로그래머인 귀도 반 로섬 (GuidovanRossum)이 발표한 고급 프로그래밍 언어로,플랫폼 독립적이며 인터프리터식,객체지
향적,동적 타이핑 (dynamicallytyped)을 지원하는 대화형 언어

**[핵심/키워드]**

&lt;실행 환경&gt;
- 파이썬 인터프리터 
- 파이썬 표준 라이브러리 
- 패키지 관리자 (pip) 
- 파이썬 가상 환경 (venv, virtual env) 

<기능, 개발 관점 주요기능> 
- 기능 관점 
  ㄴ HumanLanguage 
  ㄴ 학습하기 쉬운 언어 
  ㄴ오픈소스 기반 GlueLanguage 
  ㄴ High-Level Language 
  ㄴ 자동 메모리 관리 

- 개발 관점 
  ㄴ DynamicTyping 
  ㄴ 객체 활용 
  ㄴ 해석 프로그램(인터프리터 기반) 
  ㄴ 개발 생산성

### [인공지능] 엣지 AI(Edge AI)

**[정의]**

데이터가 생성되는 디바이스 또는 인근 네트워크 엣지에서 AI 모델을 직접 실행하여 분석·처리하고, NPU·TPU·FPGA 등 전용 AI 가속기와 모델 경량화·최적화 기술을 활용하는 기술

**[핵심/키워드]**

&lt;엣지AI 기술요소&gt; 
- 하드웨어 기술 : 전용 AI 칩셋(NVIDIA Jetson, Google Edge TPU, 
Qualcomm AI Engine)
- AI 모델 경량화·최적화 : TensorFlow Lite, ONNX, PyTorch Mobile
- MEC 아키텍처: MEC 참조 아키텍처(ETSI)
- 실시간 데이터 처리·추론 최적화 : NVIDIA TensorRT,  Intel OpenVINO, 
Qualcomm SNPE
- 네트워크 융합 기술 : 5G·IoT·MEC 결합 

&lt;엣지 컴퓨팅 기반 생성형 AI 이점 &gt; 
- 실시간/저지연성
- 데이터 프라이버시·보안 강화
- 맞춤형 개인화
- 네트워크 비용 절감
- 에너지 효율성

### [법제도] 인공지능 행동계획(AI액션 플랜)

**[정의]**

약 98개 실행 과제로 구성된 국가 인공지능 마스터플랜으로, AI 3대 강국 실현을 목표로 생태계 조성–국가 대전환–글로벌 기여를 아우르는 전략(2025년 9월)

**[핵심/키워드]**

&lt;원칙&gt;
사람 중심·포용적 인공지능, 민관 한팀, 인공지능 친화적 체계, 인공지능 균형 발전

<3대 정책 축, 12대 전략 분야> 
1\. AI 혁신 생태계 조성 
- AI고속도로 구축, 차세대 AI기술 선점, AI핵심인재 확보, AI모델확보, AI규제 혁신 

2\. 범국가 AI기반 전환 
- 산업 AX, 공공 AX, 지역 AX, AI기반 문화강국, AI기반 국방강국 

3\. 글로벌 AI 기본사회 기여 
- AI기본사회, AI기본사회 이니셔티브

### [소프트웨어공학] 제안서(Proposal)

**[정의]**

기업이나 단체에서 프로젝트를 발주 할 때 수주업체의 개발경험이나 능력,기술적 특징 등을 분석하기 위하여 제출 받는 문서

**[핵심/키워드]**

&lt;원칙&gt; 보현구
보편성, 현실성, 구체성 

&lt;기술제안서 평가항목&gt; 방기성관지상 
- 전략 및 방법론 
- 기술 및 기능 
- 성능 및 품질 
- 프로젝트 관리 
- 프로젝트 지원 
- 상생협력 및 하도급 계약 적정성

### [인공지능] 셀프 어텐션(Self-Attention)

**[정의]**

입력 시퀀스 내 모든 단어가 서로의 관계를 학습할 수 있도록 하는 어텐션 메커니즘

**[핵심/키워드]**

&lt;특징&gt; 
- 적용모델: Transformer 
- 유사도기반: Query와 Key벡터 간 유사도 계산 
- 출력방식: Value에 가중치를 곱한 값 사용 
- 계산효율성: 병렬 연산 가능 
- 장점: 모든 단어가 서로 연관성 고려 가능 
- 한계: 연산량 증가 

&lt;알고리즘&gt; 
1) Query,Key,Value생성 
2) Query-Key유사도 계산 
3) Softmax 적용 (어텐션 분포 생성) 
4) Value가중합 (어텐션 값 생성)
5) 최종 출력 반환

### [법제도] 생성형 AI 데이터 품질관리 가이드 v2.0 (2025.02)

**[정의]**

생성형 AI 발전, 생성형AI 데이터 구축 중요성 증대에 따라 AI 데이터 품질관리 체계를 생성형으로 확장한 가이드 라인

**[핵심/키워드]**

&lt;합성 데이터 품질관리 프레임워크&gt; 
- 생성형AI 데이터 품질관리 프레임워크는 인공지능 학습용 데이터 품질관리 프레임워크를 기반으로 진행 

 
- 유사성: LLM 유사성 추가 
- 편향성: LLM 유해성 추가 
- 합성데이터: 안전성, 유용성 추가 
- 의미 정확성: LLM 일치성, 정렬성 추가

### [소프트웨어공학] 요구사항 추적표(Requirement Traceability Matrix)

**[정의]**

프로젝트의 요구사항이 프로젝트 진행 과정(설계,개발,테스트 단계)에서 일관되게 반영되고 충족되고 있는지를 추적하고 관리하기 위한 문서

**[핵심/키워드]**

&lt;목적&gt;
- 요구사항 누락, 불일치 방지 
- 품질보증 및 변경 영향 추적 
- 규제 산업에서 감사 근거 제공 

&lt;주요 작성내용&gt; 
- 요구사항ID, 설명, 출처, 상태 
- 설계 항목 및 구현코드 참조 
- 테스트케이스 매핑 정보 
- 변경 이력 및 검증 결과 

&lt;활용방법&gt; 
- 요구사항-산출물-테스트 간 추적성 확보 
- 변경 영향 분석 및 검증 근거 제공

### [인공지능] 트랜스포머(Transformer)

**[정의]**

RNN을 제거하고 Self-Attention을 활용하여 문맥을 학습하는 신경망 기반의 자연어 처리(NLP)모델

**[핵심/키워드]**

&lt;특징&gt; 
- RNN없이 병렬 연산 가능, Self-Attention만 사용, Encoder-Decoder구조 

&lt;구조&gt;
- 인코더/디코더
  ㄴ Self-Attention 
  ㄴ Multi-HeadAttention 
  ㄴ Position-wiseFeedForwardNetwork(FFN)
  ㄴ ResidualConnection&LayerNormalization 
  ㄴ PositionalEncoding

- 디코더 
  ㄴ Encoder-DecoderAttention 
  ㄴ MaskedSelf-Attention 
  ㄴ Softmax &LinearTransformation

### [법제도] 범용 인공지능 (GPAI) 위험 관리 프레임워크(2025.02)

**[정의]**

인간 수준 이상의 지능을 갖춘 범용 인공지능(GPAI)이 초래할 수 있는 예측 불가능하고 복합적인 위험 요소를 체계적으로 식별, 분석, 평가, 대응하기 위해 설계된 정렬 중심의 안전관리 체계

**[핵심/키워드]**

&lt;기반&gt; ISO 31000, ISO/IEC 23894 

&lt;단계별 주요 활동&gt; 
1\. 위험 식별(Risk Identify) 
2\. 위험 분석(Risk Analyse) 
3\. 위험 평가(Risk Evaluate) 
4\. 위험 대응(Risk Treat)

### [소프트웨어공학] COCOMO(Constructive Cost Model)

**[정의]**

시스템의 비용을 산정하기 위해 시스템을 구성하고 있는 모듈과 서브 시스템의 비용 합계를 계산하는 방식

**[핵심/키워드]**

&lt;COCOMO모델&gt; 
- 기본형(Basic) COCOMO 
- 중간형(Intermediate) COCOMO
- 발전형(Detailed) COCOMO 

&lt;COCOMO유형&gt; 
- 유기적 모드, 반결합 모드, 내장 모드 


- Applicationcompositionmodel(응용합성) (프로토타입)
- Earlydesignmodel(초기설계)
- Post-Architecturemodel(설계이후)

### [인공지능] 멀티모달 인공지능(Multimodal AI)

**[정의]**

텍스트와 시각적 정보, 소리, 영상, 촉감 등 인간의 다양한 감각기관을 통합하여 학습 후 새로운 창작물을 생성하는 차세대 AI기술

**[핵심/키워드]**

&lt;모델크기&gt; 소형중형 (수백만수십억 개의 파라미터) 
&lt;주요 예시&gt; CLIP,Flamingo,Kosmos-1 
&lt;연산량&gt; 일반적인 GPU학습 가능 
&lt;기술요소&gt; 
- 입력 모듈(InputModule): 데이터를 입력받아 전처리 및 인코딩 
  ㄴ 다양한 모달 데이터 처리 
  ㄴ 데이터 인코딩 (ModalityEncoding) 
  ㄴ 자연어 처리 (NLP 
  ㄴ 컴퓨터 비전 (CV)

- 융합 모듈(FusionModule): 데이터 통합하여 의미를 학습, 연관성 분석 
  ㄴ 멀티모달 Transforme 
  ㄴ Cross-ModalityLearning(교차 모달 학습) 
  ㄴ ContrastiveLearning(대조 학습) 
  ㄴ 분산 학습 (DistributedLearning) 
  ㄴ 지식 증류 (KnowledgeDistillation) 

- 출력 모듈 (OutputModule): 분석데이터 기반 텍스트, 영상 결과 생성 
  ㄴ 멀티모달 생성 (MultimodalGeneration)
  ㄴ Vision-Language

### [법제도] 인공지능 신뢰성 인증(Certification of Artificial Intelligence, CAT)

**[정의]**

AI 시스템의 거버넌스, 기술적 완결성, 법규 준수, 성능 안정성 등을 평가하여
인증서를 부여하는 제도

**[핵심/키워드]**

&lt;목적&gt; 
- AI 시스템의 신뢰성, 투명성, 책임성을 확보하여 사회적 수용성 제고 

 
- 2025년 6월9일 고도화로 심사 방식, 국제표준 기반 변경, 심사방식 고도화됨 

&lt;고도화 사항&gt; 
1\. 국제표준 기반글로벌 호환성 확보 
- ISO/IEC 23894 (AI 위험관리)
- ISO/IEC 42001 (AI 경영시스템)
- ISO/IEC 38507 (AI 거버넌스) 기준 반영 

2.검·인증 대상 확대 
① 인공지능 시스템 ② AI 사업자 ③ AI 이용자 

2\. 평가 기준 강화 
- 기능·성능 시험 강화, 실환경 기반 위험 대응 능력 평가

### [소프트웨어공학] SW품질

**[정의]**

주어진 요구사항을 만족시킬 수 있는 소프트웨어의 기능 및 특성 (IEEE)

**[핵심/키워드]**

&lt;소프트웨어 품질&gt; 
- Big Q: 고객의 만족, 사용자 관점 품질 
- Small q: 개발자 관점, 결함없는 요구에 부합되는 소프트웨어 
- 품질(Q) = 요구사항 충족도(P) / 요구사항 기대치(E)

### [인공지능] 근사 최근접 이웃탐색(Approximate Nearest Neighbor, ANN)

**[정의]**

고차원 벡터에서 입력한 벡터와 유사한 이웃을 빠르게 찾는 근사 검색 기법

**[핵심/키워드]**

&lt;알고리즘&gt; 
- HNSW: 계층형 그래프 기반 탐색으로 정확도 매우 높고 실시간 검색에 적합
- IVF: 벡터를 K-means 클러스터링하여 검색 범위를 줄이는 방식
- PQ: 벡터를 압축·양자화해 연산량 감소, IVF와 자주 병행
- ScaNN: IVF + PQ + Rerank(재정렬) 방식의 구글 고성능 벡터 검색 알고리즘
- ANNOY: 랜덤 트리 기반 디스크 검색, 속도 빠르나 정확도는 중간

### [법제도] AI 학습데이터 구축 안내서 (2025.10)

**[정의]**

AI학습데이터의 수집·정제·가공 과정을 전 국민이 이해하고 실무에서 바로 적용할 수 있게 구성된 종합 가이드

**[핵심/키워드]**

&lt;목적&gt; 
- 국민 누구나 AI 학습데이터를 쉽게 이해하고 활용 할 수 있는 안내서 마련 
- AI 학습데이터 구축 방법에 대한 방향성 

&lt;주요 내용&gt; 
- AI 학습 방식: 지도학습, 비지도학습, 준지도학습, 강화학습
- 활용 목적에 따른 AI 학습 유형: 사전학습, 미세조정,인스트럭션 튜닝, RLHF,안전성 튜닝
- 일반데이터와 AI 학습데이터 비교: 데이터의 목적, 구조, 활용 방식 등에서 차이 

&lt;AI 학습데이터 구축 절차&gt; 
① 구축계획 수립 
② 데이터 획득 · 수집 
③ 데이터 정제 
④ 데이터 가공 
⑤ 데이터 학습

### [소프트웨어공학] ISO/IEC25000(SQuaRE,Softwareproduct Quality Requirement&Evaluation)

**[정의]**

SW개발공정 각 단계에서 산출되는 제품이 사용자 요구를 만족하는지를 검증하기 위해 품질 측정과 평가를 위한 국제표준

**[핵심/키워드]**

&lt;표준통합&gt;
- SW 제품품질모델(9126) + SW제품품질평가지침(14598) + 패키지SW(12119) + System life cycle Process(15288) 

&lt;파트구성&gt; 요모관측평 
- 요구사항(Requirement): 15288 참조한 품질 요구
- 모델(Model): 9126-1 기반 데이터 품질모델
- 관리(Management): 14598-2 품질관리계획 
- 측정(Measurement): 9126-2,3,4 대응 품질측정요소
- 평가(Evaluation): 14598 평가 프로세스 
- 25051 Extention: 패키지 SW 포함

### [인공지능] 전문가 혼합 모델(Mixture of Experts, MoE)

**[정의]**

여러 개의 전문가 네트워크(ExpertNetwork)를 두고,GatingNetwork가 특정 입력에 적합한 전문가를 선택하여 최적의 결과를 도출하는 모델

**[핵심/키워드]**

&lt;MoE 아키텍처&gt; 
- Input Layer: 외부 입력을 벡터로 임베딩하거나 전처리)
- Gating Network: 입력을 분석해 적합한 Expert 후보를 Softmax 또는 Top-k 방식으로 선택
- Load Balancing Loss: 특정 Expert에 쏠림 방지를 위해 활용도를 균등하게 유지
- Top-k Routing: Gating 점수 상위 k개의 Expert만 선택해 활성화, 연산 효율성 확보
- Expert Layer: 선택된 Expert들이 독립적으로 연산 수행, MLP 또는 Transformer 블록 구성
- Inference Layer: 활성화된 Expert들의 출력값을 Gating 가중치로 통합
- Out Layer: 분류·생성 등 목적에 맞춘 최종 출력 생성

### [법제도] 인공지능(Al) 보안안내서(2025.12)

**[정의]**

AI 기술·서비스에 대한 정보보안 관점의 기준 마련을 위한 안내서

**[핵심/키워드]**

&lt;AI 보안 위협&gt; 
- AI 모델 취약점 공격 
- AI 서비스 공격 
- AI 악용 보안 위협 
- 데이터 유출 

&lt;AI의 보안 관점 역할&gt; 
- Security for AI(AI 시스템에 대한 보안) 
- Security by AI(AI에 의한 보안)

&lt;보호대상&gt; 
- AI 모델, 데이터, 배포·운영 환경, 인프라 

&lt;적용범위&gt; 
- AI 시스템 전 생애주기 적용
(계획 및 설계 → 데이터 수집 및 준비 → 모델개발 → 모델배포 → 모니터링 및 유지보수 → 파기)

### [소프트웨어공학] ISO/IEC 15504,SPICE(Software Process Improvement and Capability Etermination)

**[정의]**

여러 프로세스 개선 모델을 ISO국제표준으로 통합하여,SDLC프로세스에 대한 개선 및 능력 평가의 기준이 되는 SW 프로세스 모델(형식,프로세스)

- 12207의 how 부재, CMM 대항

**[핵심/키워드]**

&lt;프로세스 차원&gt;
- 5개 프로세스 카테고리와 40개 세부 프로세스로 구성 
- 12207 생명주기 프로세스 기반 
- 프로세스별 목적 달성 위한 기준 제시 

&lt;프로세스 수행능력 차원&gt; 
- 0~5까지 Capability Level로 구성 
- 9개의 PA(Process Attribute)로 구성 

&lt;프로세스 카테고리&gt; 고공지관조 
1) CUS(고객-공급자)
2) ENG(공학)
3) SUP(지원)
4) MAN(관리)
5) ORG(조직) 

&lt;Capability Level&gt; 불수관확예최 
- 0-불완전, 1-수행, 2-관리, 3-확립, 4-예측, 5-최적화

### [인공지능] AI기본법(인공지능 발전과 신뢰 기반 조성 등에 관한 기본법) 시행령

**[정의]**

인공지능의 건전한 발전을 지원하고 인공지능사회의 신뢰 기반 조성에 필요한 기본적인 사항을 규정 한 시행령

**[핵심/키워드]**

&lt;내용&gt; 
- 국가 AI 거버넌스 확립 
  ㄴ 인공지능 기본계획의 수립 
  ㄴ 인공지능정책센터의 지정 
ㄴ 인공지능안전연구소의 운영 

- AI산업 육성 지원 
  ㄴ 학습용데이터 지원 대상 사업의 기준 및 통합제공시스템 구축 
  ㄴ 인공지능집적단지 지정 기준 및 절차 

- 안전 신뢰 기반 조성 
  ㄴ 22조 인공지능 투명성 확보 의무의 이행 방법 및 예외 
  ㄴ 23조 인공지능 안전성 확보 의무의 대상 인공지능시스템 기준 
  ㄴ 24조 고영향 인공지능 확인 
  ㄴ 26조 고영향 인공지능 사업자 책무 
  ㄴ 27조 고영향 인공지능 영향평가의 포함사항

### [법제도] 공공부문 인공지능 윤리원칙(2025.11)

**[정의]**

인공지능(AI) 기술을 통한 행정혁신을 촉진하면서 인공지능 사용에 대한 국민의 신뢰를 확보할 수 있도록 '공공부문 인공지능 윤리원칙

**[핵심/키워드]**

&lt;목표&gt; 
- 공공 부문 인공지능을 통한 행정혁신 촉진과 국민신뢰 구축 

<국민, 행정, 기술 관점 6대 원칙 구성> 
- 국민: 공공성, 형평성
- 행정: 투명성, 책임성
- 기술: 안전성, 프라이버시 보호

### [소프트웨어공학] SW유지보수

**[정의]**

SW생명주기(SDLC)의 폐기 전 단계로 오류를 수정하고 사용자의 요구사항을 정정하며 기능과 수행력을 증진시키기 위한 활동

**[핵심/키워드]**

&lt;특징&gt; 
- 지속적인 활동, 비용 증가 요인, 기능개선 포함, 운영 환경 대응, 품질보장 

&lt;유지보수 형태&gt; 완적예교 계예응지 데프문시
1) 원인별
- 완전적, 적응적, 예방적, 교정적 유지보수
2) 시점별
- 계획, 예방, 응급, 지연 유지보수
3) 대상별
- 데이터, 프로그램, 문서, 시스템 유지보수

### [인공지능] AI 네이티브 개발 플랫폼(AI-Native Development Platforms)

**[정의]**

AI가 설계와 실행의 중심이 되어, 업무 흐름 전체를 지능적으로 자동화하는 소프트웨어 환경

**[핵심/키워드]**

&lt;특징&gt;
- AI중심 설계
- 인간과 AI에이전트의 협업
- 운영의 자율성 ·지능성 ·적응성 

&lt;AI네이티브 개발 플랫폼 도구&gt; 
- 클라우드 기반 AI 플랫폼 
- 개발자 도구 (AI코딩) 
- AI에이전트 개발 플랫폼 
- AI앱 생성 플랫폼

### [법제도] AI·SW 안전성 인증(Artificial Intelligence·Software Safety Certification, AISC)

**[정의]**

국제표준(ISO 5469, ISO/IEC 42001 등) 기반, AI·SW의 안전성·신뢰성·성능·공정성을 종합적으로 평가·인증하는 제도

**[핵심/키워드]**

&lt;특징&gt;
1) 자율주행·의료·금융 등 고위험 분야 AI 사고·해킹 증가
2) 영국 AI 안전 정상회의 등 국제적 규제·안전 요구 강화
3) ISO 기반 위험 관리 표준(ISO/IEC TR 5469) 발표
4) 국내에서도 AI 안전·신뢰 관련 법·제도 기반 마련 필요 

&lt;추진 주체&gt;
- Kiwa(네덜란드): 국제 인증기관, 인증서 발급
- AIWORKX(AI·SW 전문 검증기관), KOLAS(국제공인시험기관)
- FKII(한국정보산업연합회): 제도 기획·산업 확산·국내 연계
→ 3개 기관 공동 추진, 세계 최초 AI·SW 안전성 인증 모델 

 
- AI·SW 안전성 인증 
- AI 품질 검증 
- AI·SW 시험 
- AI 경영시스템(AIMS) 인증 
- AI 안전경영 (AIFSM) 인증 
- AI 사이버보안 SW Update 인증

### [소프트웨어공학] 3R(Reverse-Engineering, Re-Engineering, Re-Use)

**[정의]**

소프트웨어 역공학이나 재구조화 등의 기술을 이용하여 소프트웨어를 분석하고 정보를 추출하여 이를 다시 순공학을 사용하여 새로 구현함으로써 재사용성을 확보하는 작업

**[핵심/키워드]**

&lt;구성요소&gt; 
- 역공학(Reverse Engineering) 
- 재공학 (Re-Engineering)
- 재사용 (Reuse) 
- 순공학 
- 순환공학 
- 동기 순환공학 
- 비동기 순환공학

### [인공지능] AI 데이터센터 (AI Data Center, AIDC)

**[정의]**

초대규모 AI모델의 학습·추론을 위해 고성능 GPU/AI칩,초저지연 네트워크,고밀도 전력·냉각 시스템 등을 통합해 AI워크로드에 최적화한 데이터센터

**[핵심/키워드]**

&lt;특징&gt;
- 고성능 AI전용 하드웨어 : GPU·TPU·NPU등 AI가속기
- 초저지연·고대역폭 네트워크 : InfiniBand,Ultra Ethernet,NVLink 등 

&lt;기술요소&gt; 
- 하드웨어: AI가속기(GPU/TPU), 고대역폭 메모리(HBM), CXL(ComputeExpressLink) 
- 전력: 고밀도 전력 공급 인프라(PDU/HVDC) 
- 냉각기술: 수랭 냉각(LiquidCooling), 액침 냉각(ImmersionCooling) 
- 네트워킹: 초저지연 패브릭(Infiniband/NVLink), 고속 스토리지 네트워크(NVMe-oF)

### [법제도] 합성데이터 생성·활용 안내서(2024.12)

**[정의]**

합성데이터의 안전한 생성과 활용을 지원하기 위한 생성절차와 관련 법령 준수사항을 수록한 안내서

**[핵심/키워드]**

&lt;목적&gt; 
- AI 학습 고품질 데이터 확보, 민간 활용 촉진, 안전한 데이터 활용 

<합성데이터 생성·활용 절차> 
- 1단계: 사전준비 
- 2단계: 합성데이터 생성 
- 3단계: 안전성 및 유용성 검증 
- 4단계: 심의위원회 평가 
- 5단계: 활용 및 안전한 관리 

&lt;합성데이터의 안전성&gt;
- 생성된 합성데이터를 통해 원본데이터 내 개인 식별 가능성 검증  

&lt;합성데이터의 유용성&gt; 
- 합성데이터와 원본데이터의 분포 특성 유사성, 동일 목표 달성 가능성 검증

### [소프트웨어공학] 모듈화(Modularity)

**[정의]**

SW개발에 있어 기능을 분할하고 추상화하여 소프트웨어의 성능을 향상시키고 유지보수를 효과적으로 하기 위한 SW 설계 및 구현 기법

**[핵심/키워드]**

&lt;주요 특성&gt; 
- 결합도와 응집도 

&lt;특징&gt; 
- 분할과 지배, 정보은닉, 자료 추상화, 모듈 독립성 

&lt;모듈화 기법&gt;
- 설계: 모듈, 컴포넌트, 서비스 
- 구현: 매크로, Function, inline

### [인공지능] 중첩 학습(Nested Learning, NL)

**[정의]**

기존 딥러닝 모델의 망각 문제 극복 위해 계층적/연관 기억, CMS, HOPE 아키텍처 기반 지속 학습을 제공하는 인공지능 학습 패러다임

**[핵심/키워드]**

&lt;특징&gt; 
– 기존 학습 모델의 망각 문제 극복
– 불완전 데이터 지속적 적응력 향상
– 장/단기 기억을 다른 속도로 처리
– 장기적 복잡한 데이터 처리 개선 

&lt;매커니즘&gt; 
- 하이브리드 아키텍처, 신경망 학습 모듈 

&lt;기술요소&gt; 
- 구조/표현 관점: 계층적 다중 최적화, 연관 기억 기반 표현 
- 메모리/시간 척도 관점: 연속 메모리(CMS), 연속 학습/망각 완화 프레임 
- 학습 규칙/아키텍처 관점: 딥 옵티마이저(Deep Optimizers), HOPE 아키텍처(자가 수정 아키텍처)

### [법제도] 마이데이터 2.0

**[정의]**

금융·통신·공공 등 다양한 분야에서 개인이 자신의 데이터를 직접 통제하고 활용하며, 안전하고 편리하게 맞춤형 서비스를 받을 수 있도록 한 제도(금융 마이데이터 : 2022년 1월 전면 시행)

**[핵심/키워드]**

&lt;4대 핵심 방향&gt; 
①정보 확대 ②영업 활성화 ③이용자 편의성 ④ 정보보호 강화 

<2.0의 주요 개선사항> 
- 정보 확대: 전체 금융자산 조회, 결제내역 상세 제공, 공공 마이데이터 연계 
- 영업 활성화: 오프라인 접근 허용, 겸영·부수업무 완화, 정보 결합 기준 명확화 
- 이용자 편의성: 동의 절차 간소화, 통합 가입·탈퇴 관리, 가입유효기간 연장, 청소년 독립 이용 
- 정보보호 강화: 제3자 제공 보안, 장기 미사용 정보 폐기, 개별정보 삭제기능

### [소프트웨어공학] ISO26262(자동차 기능 안전 표준)

**[정의]**

자동차 전자·전기 시스템에서 기능 안전(FunctionalSafety)을 보장하기 위한 국제 표준

**[핵심/키워드]**

&lt;구성&gt; 
- 10개 파트 ,43개 프로세스로 구성 (3.0버전에서 11.반도체,12모터사이클 추가)

&lt;파트&gt;
용기
구시하소생
지아가
반모 


- ASIL A→B→C→D(가장 높은 수준)
- ASIL A:상대적으로 낮은 위험 수준의 시스템 
- ASIL B:중간 수준
- ASIL C:높은 수준
- ASIL D:가장 높은 수준의 안전 요구사항 적용→ADAS

