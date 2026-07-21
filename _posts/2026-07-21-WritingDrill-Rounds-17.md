---
layout: post
title: "WritingDrill_Rounds_17"
date: 2026-07-21
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

### [인공지능, 법/제도, ITPE모의고사 ] 협업필터링(Collaborative Filtering)

**[정의]**  

- 대규모의 기존 사용자 행동 정보를 분석하여 해당 사용자와 비슷한 성향의 사용자들이 기존에 좋아했던 항목을 추천하는 알고리즘  

**[핵심/키워드]**  

&lt;유형&gt;  
- 메모리 기반(Memory Based) 협업필터링  
  ㄴ사용자 기반(User Based) : 비슷한 사용자 구매 상품 추천  
  ㄴ아이템 기반(Item Based) : 구매 아이템 연관 상품 추천  

- 모델 기반(Model Based) 협업필터링  
  ㄴ행렬 분해 방식, 머신러닝 기반, 딥러닝 기반 방식  

&lt;유사도 알고리즘&gt;  
- 유클리디안 기반  
- 코사인 기반  
- 자카드 계수 기반  
- 피어슨 상관 계수  
- 맨해튼 거리  

&lt;문제점&gt;  
- 필터버블, 콜드 스타트, 계산 효율 저하  

### [인공지능, 법/제도, ITPE모의고사 ] XAI(eXplainable AI)

**[정의]**  

- 사용자가 인공지능 시스템의 동작과 최종 결과를 이해하고 올바르게 해석하여 결과물이 생성되는 과정을 설명 가능하도록 해주는 기술  

**[핵심/키워드]**  

<모델 내 설명 : XAI 내재형>
- 신경 회로망 노드에 설명 라벨링  
- 의사결정트리를 이용한 설명 모델 만들기  
- 통계적 방법을 이용하여 설명 모델 유추하기  

<모델 외 설명 : XAI 사후형>
- 모델 기반 기법  
  ㄴ화이트박스 모델(White-box Model)  
  ㄴ해석 가능한 신경망(Interpretable Neural Networks)  
  ㄴSurrogate Model(대리 모델)  
- 사후 설명 기법  
  ㄴLIME(Local Interpretable Model-agnostic Explanations)  
  ㄴSHAP(SHapley Additive exPlanations)  
  ㄴCounterfactual Explanations  
- 신경망 시각화  
  ㄴSaliency Map(살리언시 맵)  
  ㄴGrad-CAM(Gradient-weighted Class Activation Mapping)  
  ㄴFeature Attribution(특징 속성 분석)  
- 규칙 학습 기반  
  ㄴRule Extraction(규칙 추출)  
  ㄴDecision Trees Approximation(의사결정 트리 근사화)  
- 설명 가능성 강화 기법  
  ㄴAttention Mechanism(어텐션 메커니즘)  
  ㄴConcept Bottleneck Models  
- 대화형 AI 설명 기법  
  ㄴExplainable Chatbots(설명 가능한 챗봇)  
  ㄴInteractive Visualization(대화형 시각화)  

### [인공지능, 법/제도, ITPE모의고사 ] 차원 축소 알고리즘

**[정의]**  

- 고차원 데이터를 저차원으로 변환하여 데이터의 중요한 정보를 유지하면서 연산 비용을 줄이는 기법  

**[핵심/키워드]**  

&lt;필요성&gt;  
- 데이터 시각화, 노이즈 제거, 모델 성능 향상, 차원의 저주 해결을 위해 사용  

&lt;차원축소 알고리즘&gt;  
- 선형 차원 축소(Linear Dimensionality Reduction)  
  ㄴPCA(Principal Component Analysis, 주성분 분석)  
  ㄴLDA(Linear Discriminant Analysis, 선형 판별 분석)  
  ㄴFA(Factor Analysis, 요인 분석)  

- 비선형 차원 축소(Non-Linear Dimensionality Reduction)  
  ㄴt-SNE(t-Distributed Stochastic Neighbor Embedding)  
  ㄴUMAP(Uniform Manifold Approximation and Projection)  
  ㄴIsomap(Isometric Mapping)  
  ㄴLLE(Locally Linear Embedding, 국소적 선형 임베딩)  

- 신경망 기반 차원 축소(Deep Learning-Based Dimensionality Reduction)  
  ㄴAutoencoder  
  ㄴVariational Autoencoder(VAE)  
  ㄴRBM(Restricted Boltzmann Machine)  

- 행렬 분해 기반 차원 축소 (Matrix Factorization)  
  ㄴSVD(Singular Value Decomposition, 특이값 분해)  
  ㄴNMF(Non-Negative Matrix Factorization, 비음수 행렬 분해)  
  ㄴMDS(Multidimensional Scaling, 다차원 척도법)  

### [인공지능, 법/제도, ITPE모의고사 ] 의사결정나무

**[정의]**  

- 분류함수를 의사결정규칙으로 표현할 때 타원, 직선, 사각형을 이용하여 나무형태로 그려서 분석하는 도구  

**[핵심/키워드]**  

&lt;구분&gt; : 목표 변수에 따라  
- 분류나무트리 → 범주형  
- 회귀나무트리 → 연속형  

&lt;구성요소&gt;  
- 루트 노드, 내부 노드, 리프 노드, 분할 기준  

&lt;특징&gt;  
- 장점 : 해석쉬움, 특성선택 필요없음, 비선형관계 학습 가능, 교호작용 자동 반영  
- 단점 : 과적합 위험, 데이터 변화 민감, 분류 성능 제한적  

&lt;동작절차&gt; :  변성가타분  
1) 변수선택 : 종속변수와 관계있는 독립변수 선택  
2) 의사결정나무 형성 : 분석목적과 자료의 구조에 따른 분리기준과 정지규칙으로 구조 작성  
3) 가지치기 : 부적절한 가지제거  
4) 타당성 평가 : 이익, 위험, 비용 등을 고려하여 모델 평가  
5) 분류 및 예측 : 분류 및 예측 수행  

<마디 분리 기준(분할기준)>
- 불순도: 다양한 범주들의 개체들이 얼마나 포함되어 있는가  
- 순수도: 목표변수의 특정 범주에 개체들이 포함되어 있는 정도  

&lt;재귀적 분할 알고리즘&gt;  
- ID3, C4.5/C5.0, CHAID, CART  

### [인공지능, 법/제도, ITPE모의고사 ] 하이퍼파라미터 최적화(Hyperparameter Optimization)

**[정의]**  

- 모든 기계학습 모델들은 저마다의 하이퍼파라미터를 갖고 있고, 그 값에 따라 성능 차이 발생  

**[핵심/키워드]**  

&lt;하이퍼파라미터 개념&gt;  
- 모델링할 때 사용자가 직접 세팅해주는 값, 최적이 성능을 위한 최적화 필요  

&lt;구분&gt;  
- 블랙박스 최적화(Black-Box Optimization)  
  ㄴGrid Search(격자 탐색)  
  ㄴRandom Search(랜덤 탐색)  
  ㄴBayesian Optimization(베이지안 최적화)  
  ㄴSimulated Annealing(시뮬레이티드 어닐링)  
  ㄴGenetic Algorithms(유전 알고리즘)  

- 다중 충실도 최적화(Multi-Fidelity Optimization)  
  ㄴModeling Learning Curve(학습 곡선 모델링)  
  ㄴBandit Based(밴딧 기반 탐색)  
  ㄴSuccessive Having(순차적 절반 선택)  
  ㄴHyper-Band(하이퍼 밴드 알고리즘)  

### [인공지능, 법/제도, ITPE모의고사 ] 피지컬 AI(Physical AI)

**[정의]**  

- 인공지능(Al)이 물리적 환경에서 직접 동작하며, 감각, 학습,행동을 수행하는 시스템  

**[핵심/키워드]**  

&lt;특징&gt;  
- 3D가상공간(디지털트윈,메타버스)학습  
- 물리적 환경 실시간 학습 및 적응  
- 가상·현실 통합 모델  
- 다양한 물리 장치(카메라,Lidar,로봇 등)와 연동  

&lt;아키텍처 구성&gt;  
1) HW영역 : Perception Layer(인지 계층)  
- Visual Sensors(시각)  
- Tactile Sensors(촉각)  
- Position Sensors(위치)  
- Force Sensors(힘)  
- Sensor Fusion  

2) SW영역 : Cognitive Layer(생각·판단)  
- Physics Models  
- Decision Making  
- Adaptive Learning  

3) HW영역 : Action Layer(행동)  
- Motion Control  
- Robotic Actuators  
- Force Application  

&lt;기술요소&gt;  
- 센싱 시스템 : 카메라, Lidar, loT 센서  
- 컴퓨터 비전 : 온디바이스 비전 Al, 모델 경량화  
- 멀티모달지능 : VLA(Vision-Language-Action)­  
- 강화 학습 : 강화학습(RLHF, PPO)  
- 자연어 처리 : 소형 LLM(sLLM)  
- 엣지 AI : 온디바이스 AI, Al 전용 칩셋  
- 액추에이션 시스템 : 액추에이터 제어 기술  
- 통신 기술 : 5G/6G 통신, 초저지연 loT 네트워크  
- 피지컬 AI, 개발 F/W : LWM, Tokenizer, 디지털트윈, 메타버스, AI 가속기  
- 로보틱스 : SLAM(Simultaneous Localization&Mapping)  
- Sim2Real : DomainRandomization,TransferLearning  
- 데이터 베이스 : 벡터DB  
- 서비스 : 자율주행차, 휴머노이드 로봇  

### [인공지능, 법/제도, ITPE모의고사 ] OWASP Kubernetes Top 10 Risks

**[정의]**  

- 보안 담당자, 시스템 관리자, 소프트웨어 개발자가 쿠버네티스 생태계 전반의 위험 우선순위를 정하는데 도움을 주기 위해 만들어진 가이드  

**[핵심/키워드]**  

&lt;구성항목&gt;  
- K01 : 취약한 워크로드 설정(Insecure Workload Configurations)  
- K02 : 공급망 취약점(Supply Chain Vulnerabilities)  
- K03 : 과도한 RBAC 권한(Overly Permissive RBAC)  
- K04 : 중앙 정책 적용 부재(Lack of Centralized Policy Enforcement)  
- K05 : 로깅·모니터링 미흡(Inadequate Logging and Monitoring)  
- K06 : 인증 메커니즘 취약(Broken Authentication Mechanisms)  
- K07 : 네트워크 분리 미흡(Missing Network Segmentation Controls)  
- K08 : 비밀정보 관리 실패(Secrets Management Failures)  
- K09 : 클러스터 구성 오류(Misconfigured Cluster Components)  
- K10 : 취약한 구성 요소(Vulnerable Components)  

### [인공지능, 법/제도, ITPE모의고사 ] 데이터스페이스(Data Space)

**[정의]**  

- 데이터 제공자가 데이터 주권(소유·통제권)을 유지한 채, 신뢰·정책·표준에 기반하여 분산 환경에서 데이터를 안전하게 공유·활용하는 데이터 협력 체계  

**[핵심/키워드]**  

&lt;핵심원칙&gt;  
- 데이터 주권 보장 : 데이터 제공자가 접근·이용 조건을 직접 통제  
- 신뢰 기반 공유 : 참여자 간 인증·계약·감사로 신뢰 확보  
- 분산 아키텍처 : 중앙 저장소 없이 커넥터 기반 연계  
- 정책 기반 이용 통제 : 목적·기간·범위 등 Usage Control 적용  
- 상호운용성 : 공통 표준·인터페이스로 이기종 간 연계 지원  

&lt;구성요소&gt;  
- 데이터 제공자(Data Provider) : 데이터를 보유하고 공유 조건·정책을 설정하는 주체  
- 데이터 이용자(Data Consumer) : 정책에 따라 데이터를 활용하는 주체  
- 데이터 커넥터(Connector) : 데이터 교환·정책 집행을 수행하는 기술적 연결 요소  
- 카탈로그/메타데이터 : 데이터 검색·이해·선택을 위한 정보 관리  
- 신뢰 프레임워크 : 인증·계약·감사를 통한 참여자 신뢰 확보 체계  

&lt;기술기반&gt;  
- 표준 API·커넥터 : 이기종 시스템 간 데이터 연계  
- 식별·인증(ID & Trust) : 참여자·시스템 신원 검증  
- Usage Control : 이용 목적·기간·범위에 따른 데이터 사용 통제  
- 프로비넌스·감사 로그 : 데이터 사용 이력 추적 및 책임성 확보  

&lt;운영방식&gt;  
- 분산 연계 운영 : 데이터는 각 참여자에 유지, 필요 시 연계  
- 정책·계약 중심 관리 : 기술 + 법적 계약의 결합  
- 거버넌스 기반 협력 : 공통 규칙 하에서 자율적 참여  

&lt;활용 분야&gt;  
- 제조·공급망 : Catena-X 등 산업 데이터 연계  
- 공공·스마트시티 : 기관 간 데이터 협력  
- 에너지·헬스케어·모빌리티 : 민감 데이터의 안전한 공동 활용  

### [인공지능, 법/제도, ITPE모의고사 ] 에이전틱AI(Agentic AI)

**[정의]**  

- 사용자의 명확한 지시나 명령 없이도 스스로 작업을 수행하는 자율적인 소프트웨어(가트너2025)  

**[핵심/키워드]**  

&lt;특징&gt;  
- 자율성,목표지향성,계획 수립 능력,지속적 상호작용 및 피드백,학습 및 적응력  

&lt;구성요소&gt;  
- User(사용자)  
- AIAgent  
- LLM(대형 언어 모델)  
- Database(DB)  
- VectorDB(벡터 데이터베이스)  
- Action(행동 수행 모듈)  
- ModelCustomization(모델 맞춤화)  
- DataFlywheel(데이터 플라이휠)  

&lt;기술요소&gt;  
- 인식(Perceive) : 데이터 수집, 특징 추출, 멀티모달 데이터 처리, 실시간 데이터 스트리밍  
- 추론(Reason) : LLM 기반 추론, RAG, 지식 그래프, 강화학습, 상황 인식 AI  
- 행동(Act) : 목표 설정, API 연동, 클라우드 서비스 실행, 로봇 및 IoT 제어, 작업 자동화  
- 학습(Learn) : 피드백 루프, 데이터 큐레이팅, 모델 재훈련, 지속 학습, SaaS 기반 학습  
- 성능 관리(Self-Governance) : IoT연동, 자율의사결정, XAI, AI 보안 및 신뢰성, 데이터 거버넌스  

### [인공지능, 법/제도, ITPE모의고사 ] ISO/IEC TR 29119-11

**[정의]**  

- AI 기반 시스템을 도입하고 테스트하는 방법에 대한 지침을 제공하는 ISO/IEC의 기술 보고서(Technical Report)  

**[핵심/키워드]**  

&lt;필요성&gt;  
- AI 신뢰성 평가, 표준화된 검증, 인공지능 안정성  

&lt;구성요소&gt;  
1.Scope(적용 범위)  
2.Normativereferences(규범적 참조 문헌)  
3.Terms,definitionsandabbreviatedterms(용어,정의 및 약어)  
4.IntroductiontoAIandtesting(AI및 테스트 소개)  
5.AIsystemcharacteristics(AI시스템 특성)  
6.IntroductiontothetestingofAI-basedsystems(AI기반 시스템 테스트 소개)  
7.TestingandQAofMLsystems(머신러닝(ML)시스템 테스트 및 품질 보증)  
8.Black-boxtestingofAI-basedsystems(AI기반 시스템의 블랙박스 테스트)  
9.White-boxtestingofneuralnetworks(신경망의 화이트박스 테스트)  
10.TestenvironmentsforAI-basedsystems(AI기반 시스템의 테스트 환경)  

- 조합 테스트(Combinatorial Testing)  
- 백투백 테스트(Back-to-Back Testing)  
- A/B 테스트(A/B Testing)  
- 변성 테스트(Metamorphic Testing)  

- 뉴런 커버리지  
- 임계점 커버리지  
- 부호 변경 커버리지  
- 값 변경 커버리지  
- 부호-부호 커버리지  
- 레이어 커버리지  

### [인공지능, 법/제도, ITPE모의고사 ] 프론티어 AI(Frontier AI)

**[정의]**  

- 기존 AI기술을 넘어서는 기술로,인간의 복잡한 문제 해결 능력을 모방하거나 능가하는 AI  

**[핵심/키워드]**  

&lt;프론티어 AI 역량&gt;  
- 창발성, 활용성(다양한 활용 가능), 접근성(저렴한 API 비용)  

&lt;프론티어 AI의 위험성&gt;  
- 악용 가능성, 예측 불가능성, 환각/탈옥, 프라이버시 침해, 경제 불평등 야기  

&lt;프론티어 AI의 규제방안&gt;  
1\. 윤리적 교육 및 인식제고  
2\. 안전성 검증  
3\. 책임 강화  
4\. 데이터 투명성  
5\. 사용제한  
6\. 악의적 사용 금지  
7\. 지속적 관리  
8\. 글로벌한 거버넌스 및 체계  

### [인공지능, 법/제도, ITPE모의고사 ] ISO/IEC 25059

**[정의]**  

- AI 시스템을 위한 품질 모델 기반으로 AI 시스템의 품질을 규정, 측정 및 평가하기 위한 기준 제공 표준  

*ISO/IEC 25010(SQuaRE) 표준을 AI 특성에 맞게 확장  

**[핵심/키워드]**  

&lt;구성항목&gt; : 기신사효유이 + 보호  
- 기능적합성  
- 신뢰성  
- 사용성  
- 성능효율성  
- 유지보수성  
- 이식성  
- 보안  
- 호환성  

<품질 특성(신규/수정 사항)> : AI 시스템에 맞게 일부 수정(주특성/부특성)
- 기능 적합성 : 기능 정확성, 기능 적응성  
- 사용성 : 사용자 제어 가능성, 투명성  
- 신뢰성 : 강건성  
- 보안성 : 개입가능성  

### [인공지능, 법/제도, ITPE모의고사 ] 디지털 출처(Digital Provenance)

**[정의]**  

- 데이터·AI·소프트웨어 자산의 전 생애주기 변경 이력을 추적·검증하여 진위(Authenticity)·무결성(Integrity)·신뢰성(Trust)을 보장하는 기술적·관리적 신뢰 체계  

*AI위조(딥페이크),공급망 공격,생성형 AI신뢰성 문제를 대응하는 핵심 기반 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
- SBOM·워터마크로 진본성 검증  
- 조작·위조 탐지  

&lt;기술요소&gt;  
- 데이터·소프트웨어 출처 : SBOM, MLSBOM 기반  
- 콘텐츠 출처 인증 : C2PA 기반 워터마킹, 디지털 워터마킹  
- 이력 관리 : Provenance DB(출처·이력 DB), 데이터 라인리지 도구  
- 무결성 보장 : Immutable Ledger, 해시, 전자서명, PKI, WORM  
- 공급망 보안 : Supply Chain Security, SBOM 검증, 외부 라이브러리·모델 유입 리스크 통제  
- AI 신뢰성 : AI Model Provenance, 데이터 드리프트 확인, Provenance Certificate  
- 운영·거버넌스 : Policy & Compliance, Audit log, API Trace  
- 자산식별 : 메타데이터 스키마, UUID/DID, Data Catalog 기반  
- 정보수집 : ETL/Meta data, EXIF/XMP, SBOM/MLSBOM을 통해 정보 자동 수집  
- 위변조 검증 : 해시, 디지털 워터마킹, 전자서명, PKI  
- 진위성 확인 : Timestamp, 인증서 검증, 포렌식  
- 수정여부 판단 : 버전관리 시스템, 데이터 드리프트 확인  
- 출처 추적 : W3C PROV, 데이터 라인리지 도구, API Trace  
- 검증결과 저장 : WORM, Provenance Certificate, Audit log  

&lt;검증절차&gt;  
- 자산식별 출처정보 수집 → 위변조 검증 → 진위성 확인 → 수정여부 판단 → 출처추적 → 검증결과 저장 → 지속 모니터링  

&lt;참고&gt; 디지털 리니지(Digital Lineage)  
- 전사 데이터 신뢰성 확보위해 데이터 생명 주기 전과정 추적,관리하여 시각적으로 제공하는 기술  

### [인공지능, 법/제도, ITPE모의고사 ] 섀도우 AI(Shadow AI)

**[정의]**  

- 조직의 승인·통제 없이 직원이 개인적으로 사용하는 AI 도구/서비스(LLM, Copilot 등)  

**[핵심/키워드]**  

&lt;특징&gt;  
- 비인가 사용 : 공식 IT 거버넌스·보안 정책 미적용  
- 데이터 유출 위험 : 민감정보를 외부 AI에 입력  
- 가시성 부족 : 사용 현황 파악·통제 어려움  
- 생산성 유인 : 편의성·효율성 때문에 확산  

&lt;위험요소&gt;  
- 기밀·개인정보 유출, 저작권·컴플라이언스 위반  
- 잘못된 결과(환각) 의존으로 의사결정 오류  
- 로그·감사 부재로 책임 추적 어려움  

&lt;대응방안&gt;  
- 승인된 엔터프라이즈 AI 도입(접근통제·로깅)  
- 데이터 분류·마스킹 및 입력 가이드라인 수립  
- CASB/DLP/프록시 기반 사용 가시화·차단  
- 사용자 교육 및 정책(허용/금지 리스트) 명확화  
- AI 거버넌스  

### [인공지능, 법/제도, ITPE모의고사 ] 지식 증류(Knowledge Distillation)

**[정의]**  

- 대규모 모델(교사 모델, Teacher Model)이 학습한 지식을 소규모 모델(학생 모델, Student Model)로 전이하여, 성능은 최대한 유지하면서 모델의 크기와 계산 복잡도를 줄이는 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
- 모델 경량화  
- LLM 성능 유지  

&lt;과정순서&gt;  
① Teacher모델 준비  
② Student모델 설계  
③ SoftLabels생성  
④ Student모델 학습  
⑤ 모델 최적화  
⑥ 성능 평가 및 배포  

&lt;유형&gt;  
- 로지트 증류(LogitDistillation)  
- 특징 맵 증류(FeatureMapDistillation)  
- 관계 증류(RelationalDistillation)  
- 자기 지식 증류(Self-KnowledgeDistillation)  
- 멀티-Teacher증류(Multi-TeacherDistillation)  
- 교차 도메인 증류(Cross-DomainDistillation)  
- 온라인 증류(OnlineDistillation)  
- Attention증류(AttentionDistillation)  
- 데이터 증강 결합 증류(Data-AugmentedDistillation)  
- 비지도 증류(UnsupervisedDistillation)  

### [인공지능, 법/제도, ITPE모의고사 ] 정보보호 공시제도

**[정의]**  

- 기업이나 기관이 자율적으로 수행한 정보보호 수준과 정보보호 투자 현황 등을 외부에 공개하는 제도  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 「정보보호산업의 진흥에 관한 법률」 제13조(정보보호 공시), 동법 시행령 제8조(정보보호 공시)  

&lt;공시대상&gt;  
- 자율공시대상 : 정보통신망을 통해 정보를 제공하거나 매개하는 자  
- 의무공시대상  
  ㄴ사업분야 : ISP, IDC, 상급종합병원, CSP  
  ㄴ매출액 : 유가증권시장·코스닥시장 상장법인 중 매출액 3,000억 이상  
  ㄴ이용자수 : 정보통신서비스 일일 평균 이용자 수 100만명 이상(전년도말 3개월 기준)  

&lt;공시방법&gt; 매년 6월 30일까지 전년도 현황을 공시 포털(isds.kisa.or.kr) 게시  

&lt;공시항목&gt;  
① 정보보호 투자 현황  
② 정보보호 인력 현황  
③ 정보보호 관련 인증·평가·점검 사항  
④ 정보보호 활동 현황  

&lt;개정안&gt;  
- 2026.01.09 입법예고  
  ㄴ상장사 전체로 확대, ISMS 인증기업 포함, 예외 전면 삭제(일부 기관(공공·금융·소기업 등) 제외)  
- 2026년 5월 11일  
  ㄴ재입법 예고, 중소기업기본법에 따른 소기업은 준비 위해 2년 유예  

### [인공지능, 법/제도, ITPE모의고사 ] 릴레이션의 차수(Degree)와 카디널리티(Cardinality)

**[정의]**  

- 차수(Degree) : 릴레이션(테이블)에서 열(Column,속성)의 개수  
- 카디널리티(Cardinality) : 릴레이션(테이블)에서 행(Row,튜플)의 개수  

**[핵심/키워드]**  

<차수(Degree) 주요특성>
- 변화여부 : 스키마 변경 시에만 변함(정적)  
- 최소값 : - 1(최소 하나의 속성 필요)  
- 상한값 : DBMS 및 설계 제약에 따라 제한됨  
- 결정요인 : 스키마 설계 및 데이터 모델링  
- 저장구조 : 속성 수 증가 → 튜플 크기 증가 → 저장 비용 증가  
- 확장성 : 스키마 변경 필요(DDL), 변경 비용이 큼  
- 영향 : 튜플 구조, 데이터 표현 방식 및 설계 복잡도에 영향  

<카디널리티(Cardinality) 주요특성>
- 변화여부 : 데이터 삽입/삭제에 따라 변함(동적)  
- 최소값 : 0(공집합 릴레이션 가능)  
- 상한값 : 이론적 제한 없음(시스템 자원에 의존)  
- 결정요인 : 데이터 삽입/삭제, 트랜잭션 처리  
- 질의최적화 : 카디널리티 추정이 실행 계획 수립의 핵심 요소  
- 인덱스영향 : 카디널리티가 높은 컬럼일수록 인덱스 효율 증가  
- 선택도 : 조건절의 필터링 성능과 직접적으로 연관됨  
- 영향 : 저장 공간, 질의 처리 비용, 전반적인 성능에 영향  

* 카디널리티의 여러 의미  
- 관계 데이터 모델(릴레이션) : 릴레이션의 튜플(행) 개수  
- ER 모델(관계 대응 수) : 개체 간 관계(1:1, 1:N, M:N)  
- 쿼리 최적화(열 카디널리티) : 한 열의 서로 다른 값의 개수(성별 열 → 2, PK 열 → 행 수와 동일)  

### [인공지능, 법/제도, ITPE모의고사 ] 데이터 품질(DQ, Data Quality) 인증제도(2026. 02)

**[정의]**  

- 과학기술정보통신부가 지정한 데이터 품질인증기관이 데이터의 내용, 데이터의 구조를 포함한 관리체계 등을 진단하고 수준을 평가해 품질을 인증하는 제도  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 데이터 산업진흥 및 이용촉진에 관한 기본법(데이터 산업법) 제20조  

&lt;인증유형&gt;  
1) 데이터 내용 인증  
 - 인증대상 : 데이터 구조, 데이터 내용  ※ 정형/비정형 데이터로 구분  
 - 품질기준 : 정형/비정형 데이터(완전성, 유효성, 일관성, 정확성, 접근성, 유일성)  
 - 인증준용표준 : ISO/IEC 25012, ISO/IEC 25024, ISO/IEC 5259-2, TTAK.KO10.1344-Part2  
 - 데이터 구조 유형 : Simple-Type, Normal-Type, Complex-Type  
 - 인증등급 : Class A, Class B, Class C  
 - 유효기간 : 1년  

2) 데이터 관리체계 인증  
 - 인증대상 : 데이터 기반 사업, 데이터 시스템, 데이터 관리 조직  
 - 품질기준 : 완전성, 유효성, 일관성, 정확성, 보안성, 유용성, 접근성, 적시성, 다양성, 유일성  
 - 인증준용표준 : ISO 8000-61, ISO 8000-62, ISO/IEC 33020, ISO/IEC 5259-4  
 -  데이터 구조 유형 : 해당없음  
 - 인증등급 : Level 2, Level 3, Level 4, Level 5  
 - 유효기간 : 3년  

### [인공지능, 법/제도, ITPE모의고사 ] 액티브 러닝(Active Learning)

**[정의]**  

- 머신러닝 모델이 학습 과정에서 유의미한 데이터를 능동적으로 선택하여 학습하는 방법  

**[핵심/키워드]**  

&lt;핵심아이디어&gt;  
- 중요한 데이터를 모델이 선택 후 인간 개입 라벨링  

&lt;라벨생성방식&gt;  
- 사람이 직접 라벨을 붙임(Active Query)  
- 사람의 라벨링 수를 최소화하는 데 초점(더 적은 라벨로 최대 성능)  

&lt;절차&gt;  
1\. 데이터 수집  
2\. 데이터셋 분할  
3\. 모델 학습  
4\. 데이터 선택  
5\. 학습 중단 기준 마련  

&lt;대표알고리즘&gt;  
- Uncertainty Sampling(불확실성 샘플링)  
- Query By Committee(QBC)  
- Expected Model Change(EMC)  

### [인공지능, 법/제도, ITPE모의고사 ] 자기지도 학습 (Self-Supervised Learning)

**[정의]**  

- 라벨이 없는 데이터(Unlabeled Data) 에서 자신이 스스로 라벨을 만들어 학습하는 방식  

**[핵심/키워드]**  

&lt;핵심아이디어&gt;  
- 모델이 라벨 없이 스스로 학습 과제 생성,대조학습  

&lt;라벨생성방식&gt;  
- 모델이 데이터 관계로부터 스스로 라벨 생성  
- 라벨 없이 표현(Representation) 학습하는 데 초점  

&lt;절차&gt;  
1\. 사전 과제 정의(Pretext Task)  
2\. 자기 생성 라벨 구성(Synthetic Label)  
3\. 모델 입력 및 학습  
4\. 표현학습(Representation)  
5\. 다운스트림 활용  

&lt;대표알고리즘&gt;  
- Context Prediction : BERT,GPT계열  
- Contrastive Learning(대조 학습) : SimCLR, MoCo, BYOL, CLIP  
- Generative(생성 기반) : VAE, AE, MAE  
- Clustering/Prototype Learning : SwAV, DeepCluster  
- Predictive Coding(예측 부호화) : CPC  
- Transformation Prediction : RotNet  

### [인공지능, 법/제도, ITPE모의고사 ] ITIL v4.0

**[정의]**  

- 2019년초 릴리즈 된 ITIL의 버전으로 데브옵스,애자일,린 접근을 포함한 실용적 지침 기반의 ITSM모델  

**[핵심/키워드]**  

- 라이프사이클 → 서비스 가치 시스템(SVS)전환  
- 애자일·DevOps 연계, 7가지 원칙 도입  
- 유연한 프랙티스 제공  

&lt;특징&gt;  
- 서비스 가치 시스템 도입,애자일·DevOps 연계, 7가지 원칙 추가, 서비스 가치 체인 포함, 34개 프랙티스 적용  

<서비스 관리의 4차원 모델(Four Dimensions of Service Management)>
- 조직과 사람(Organizations&People)  
- 정보와 기술(Information&Technology)  
- 파트너와 공급자(Partners&Suppliers)  
- 가치 흐름과 프로세스(Value Streams&Processes)  

<서비스가치시스템(Service Value System,SVS)>
- 기회/수요(Opportunity/Demand)  
- 서비스 가치 사슬(Service Value Chain)  
- 가이드 원칙(Guiding Principles)  
- 거버넌스(Governance)  
- 관리 실행(Practices)  
- 지속적 개선(Continual Improvement)  
- 가치(Value)  

<서비스 가치 사슬(Service Value Chain)>
- 계획(Plan) → 참여(Engage) 설계 및 전환(Design&Transition) → 획득 및 구축(Obtain&Build) → 운영(Deliver&Support) → 개선(Improve)  

<가이드 원칙(GuidingPrinciples)>
- 가치 중심으로 일하라  
- 현재 상태에서 시작하라  
- 반복적으로 피드백을 적용하라  
- 협업하고 투명성을 유지하라  
- 전체론적 사고를 가져라  
- 단순하게 유지하고 실용적으로 하라  
- 자동화를 적극 활용하라  

<프랙티스(Practices)>
- 일반 관리 실행(14개) → IT서비스뿐만 아니라 조직 운영과 전략 수립까지 포함  
- 서비스 관리 실행(17개) → IT서비스 운영 및 장애 대응 중심  
- 기술 관리 실행(3개) → IT인프라,배포,소프트웨어 개발 중심  

### [인공지능, 법/제도, ITPE모의고사 ] AI Alignment

**[정의]**  

- AI의 행동과 결과가 인간의 가치·의도·목표와 일치하도록 만드는 기술·연구 분야  

**[핵심/키워드]**  

- 라이프사이클 → 서비스 가치 시스템(SVS)전환  
- 애자일·DevOps 연계, 7가지 원칙 도입  
- 유연한 프랙티스 제공  

&lt;특징&gt;  
- 서비스 가치 시스템 도입,애자일·DevOps 연계, 7가지 원칙 추가, 서비스 가치 체인 포함, 34개 프랙티스 적용  

<서비스 관리의 4차원 모델(Four Dimensions of Service Management)>
- 조직과 사람(Organizations&People)  
- 정보와 기술(Information&Technology)  
- 파트너와 공급자(Partners&Suppliers)  
- 가치 흐름과 프로세스(Value Streams&Processes)  

<서비스가치시스템(SVS, Service Value System)>
- 기회/수요(Opportunity/Demand)  
- 서비스 가치 사슬(Service Value Chain)  
- 가이드 원칙(Guiding Principles)  
- 거버넌스(Governance)  
- 관리 실행(Practices)  
- 지속적 개선(Continual Improvement)  
- 가치(Value)  

<서비스 가치 사슬(Service Value Chain)>
- 계획(Plan) → 참여(Engage) 설계 및 전환(Design&Transition) → 획득 및 구축(Obtain&Build) → 운영(Deliver&Support) → 개선(Improve)  

<가이드 원칙(Guiding Principles)>
- 가치 중심으로 일하라  
- 현재 상태에서 시작하라  
- 반복적으로 피드백을 적용하라  
- 협업하고 투명성을 유지하라  
- 전체론적 사고를 가져라  
- 단순하게 유지하고 실용적으로 하라  
- 자동화를 적극 활용하라  

<프랙티스(Practices)>
- 일반 관리 실행(14개) →I T서비스뿐만 아니라 조직 운영과 전략 수립까지 포함  
- 서비스 관리 실행(17개) → IT서비스 운영 및 장애 대응 중심  
- 기술 관리 실행(3개) → IT인프라, 배포, 소프트웨어 개발 중심  

### [인공지능, 법/제도, ITPE모의고사 ] ISO/SAE 21434

**[정의]**  

- 차량 기획 단계부터 시작해 생산 및 포스트 프로덕션(Post Production) 과정까지의 사이버보안 활동에 관한 프로세스를 정의하는 것을 목적으로 만들어진 국제 표준  

**[핵심/키워드]**  

- 자동차 사이버보안 위험 관리 프로세스에서 보안 위협을 분석하고 그 위험의 정도를 평가하는 핵심적인 활동  

&lt;파트구성&gt;  
- 1~4 파트 : 발간 배경에 대한 요약, 참고 문헌, 용어 및 약어, 일반적인 고려사항  
- 5~15 파트 : 기업 관리, 차량 생산 프로세스 관리, 공급망 사이버보안 활동  

1\. 개요  
2\. 참고문헌  
3\. 용어 및 약어 정의  
4\. 일반적인 고려사항  
5\. 조직 사이버보안 관리  
6\. 프로젝트 사이버보안 관리  
7\. 분산 사이버보안 활동  
8\. 지속적인 사이버보안 활동  
9\. 제품 개념 설계  
10\. 제품 개발  
11\. 사이버보안 검증  
12\. 제품 생산  
13\. 운영 및 유지  
14\. 기술 지원 및 보증 종료  
15\. 위험 분석 및 위험 평가 방법  

### [인공지능, 법/제도, ITPE모의고사 ] K-평균 알고리즘(K-Means Clustering)

**[정의]**  

- 데이터의 유사성을 기반으로 최적의 중심점을 찾아 K개의 그룹으로 분류하는 방법  

*데이터(Training Set)를 기준점(Code-vector)을 중심으로 유클리디안 거리가 최소가 되도록 K개의 묶음으로 구분하는 클러스터링 알고리즘  

**[핵심/키워드]**  

&lt;매커니즘&gt;  
1) 군집 수 K를 정의하여 임의 위치 지정(initial Centroids)  
2) 모든 데이터들의 거리 계산 후 가장 가까운 중심점 기준으로 군집화  
3) 각 군집마다 계산하여 새로운 중심 계산  
4) step 2~3을 반복, 클러스터가 변경되지 않으면 학습 완료  

&lt;활용&gt;  
- 시장과 고객 패턴인식, 공간데이터 분석, 텍스트 마이닝 등  
- 데이터가 불규칙하고 내부 특징이 알려지지 않은 분류 초기 단계에 적합  

### [인공지능, 법/제도, ITPE모의고사 ] K-중앙객체 알고리즘(K-Medoids Clustering)

**[정의]**  

- 군집에서 가장 중심에 위치한 객체인 medoid를 사용하여 n개의 객체중에서 k개의 군집을 찾는 알고리즘  

*중심점(centroid) 대신 실제 데이터 포인트(medoid)를 대표점으로 사용  

**[핵심/키워드]**  

&lt;매커니즘&gt;  
1) K개의 대표객체(medoids)를 지정  
2) 나머지 객체를 가까운 대표객체에 배속  
3) 새로운 임의의 객체를 대표 객체로 선정  
4) 총 비용과 현재의 총비용을 비교하여 작을 경우를 최종 선택  

&lt;장단점&gt;  
- 장점 : 실 데이터를 중심점으로 하여 노이즈 처리 우수  
- 단점 : 계산량 많음  

### [인공지능, 법/제도, ITPE모의고사 ] DBSCAN(Density-Based Spatial Clustering of Applications with Noise)

**[정의]**  

- 노이즈가 있는 애플리케이션을 위한 밀도에 근거한 공간적인 군집화  

*데이터 포인트의 밀도를 이용해 군집을 형성하고, 이상치(Noise)를 효과적으로 식별하는 방법  

**[핵심/키워드]**  

&lt;구성요소&gt;  
- 밀도 : 반경(엡실론)  
- MinPts : 최소 좌표점 갯수  
- 코어 : 일정기준 이상의 밀도를 갖는 데이터 집합  
- 노이즈 : 일정 기준 미만의 밀도를 갖고 군집에 소속되어 있지 않은 데이터  
- 보더 : 일정 기준 미만의 밀도를 갖지만, 군집에 소속되어 있는 데이터  

&lt;매커니즘&gt;  
1) 좌표 공간에 학습 데이터 표시  
2) 해당 점에 밀도가 MinPts 이상이면 core, 미만이면 noise로 정의  
3) 클러스터 구성 후 이웃점을 차례로 방문하면서 core인지 판단  

&lt;장단점&gt;  
- 장점 : 노이즈에 강건, 군집수 미설정  
- 단점 : 밀도 반경과 최소이웃수가 민감하게 작용, 군집별 밀도가 서로 다른 경우 적용 어려움,  
           유동적e 사용하는 OPTICS(Ordering Points To Identify the Clustering Structure)  

### [인공지능, 법/제도, ITPE모의고사 ] 자기조직화지도, SOM(Self-Organizing Map)

**[정의]**  

- 대뇌피질의 시각피질의 학습 과정을 모델화한 인공신경망으로, 자율학습에 의한 클러스터링을 수행하는 알고리즘  

*입력 벡터를 훈련 집합에서 일치되도록 가중치를 조정하여 인공신경망에 기초한 자율학습의 한 방법  

**[핵심/키워드]**  

&lt;특징&gt;  
- 비지도 학습, 데이터의 고차원 구조를 저차원으로 변환, 경쟁 학습(Competitive Learning), 연속적인 군집화 결과를 제공  

&lt;핵심키워드&gt;  
- 뉴런(Neuron) 그리드  
- 맵 크기(Grid Size, M×N)  
- 승자뉴런(BMU, Best Matching Unit)  
- 가중치 업데이트  
- 이웃 함수 (Neighborhood Function)  

- 순방향연결과 측방향 연결, 측방향 연결은 뉴런간 경쟁 생성에 사용  
- 활성화 수준이 가장 높은 뉴런이 승자  
- 경쟁에서 진 뉴런들의 활성은 억제됨  

&lt;동작절차&gt;  
1\. 초기화(Initialization)  
2\. 데이터 입력(Input Data)  
3\. 승자 뉴런 찾기(BMU, Best Matching Unit)  
4\. 가중치 업데이트 (Weight Update)  
5\. 이웃 영향 감소(Neighborhood Decay)  
6\. 반복(Iteration&Convergence)  

### [인공지능, 법/제도, ITPE모의고사 ] 생체정보 보호 가이드라인

**[정의]**  

- 생체정보에 대한 개념 및 범위를 명확하게 하고, 생체인식정보 보호조치를 구체적으로 제시한 가이드라인  

**[핵심/키워드]**  

&lt;생체정보 개념&gt;  
- 개인의 신체적, 생리적, 행동적 특징에 관한 정보로서 특정 개인을 인증·식별하거나 개인에 관한 특징(연령·성별·감정 등)을 알아보기 위해 일정한 기술적 수단을 통해 처리되는 정보  

&lt;생체인식정보 개념&gt;  
- 생체정보 중 특정 개인을 인증 또는 식별할 목적으로 일정한 기술적 수단을 통해 처리되는 정보  
  ㄴ원본정보 : 생체인식정보 중 입력장치 등을 통해 수집·입력된 특징정보 생성에 이용되는 정보  
  ㄴ특징정보 : 원본정보로부터 특징점을 추출하는 등의 일정한 기술적 수단을 통해 생성되는 정보  

&lt;생체인식정보 특성&gt;  
- 유일성/불변성, 민감정보 추출 가능성, 위/변조 가능성  

&lt;생체정보보호 6대 원칙&gt;  
- 비례성, 적법성, 목적제한, 투명성, 안전성, 통제권 보장  

&lt;생체정보보호 조치사항&gt;  
1) 기획/설계 단계 : PbD, 대체수단 마련, 개인정보 영향평가 수행  
2) 수집단계 : 적법한 수집, 위/변조 탐지, 다중인증, 전송/저장 시 암호화  
3) 이용/제공 단계 : 목적 범위 내 이용, 통제 수단 제공, 단말에서 처리  
4) 보관/파기 단계 : 저장 시 암호화, 목적 달성 시 파기, 원본정보 분리 보관  
5) 상시점검 : 개인정보 처리방침 공개, 관리/감독  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능 준비 데이터(AI Ready Data)

**[정의]**  

- AI 활용 사례에 적합한 고품질 최적화 데이터셋(가트너 2025 AI 하이프사이클 핵심 기술)  

*AI 모델 개발 및 훈련에 즉시 사용할 수 있도록 전처리되고 최적화된 데이터(DataOps 연계)  

**[핵심/키워드]**  

&lt;목표&gt;  
- 고품질 AI 학습데이터로 즉시 사용가능(DataOps연계)  

&lt;3가지 핵심요소&gt;  
- Quality : 정확성·완전성·적합성을 확보  
- Align : 맥락에 맞게 데이터를 정렬구성  
- Govern : 생애주기에서 신뢰·통제·책임을 보장하는 거버넌스 체계 구축  

&lt;특징&gt;  
- 데이터 품질 : 완전성·정확성·일관성·고유성  
- 구조화·접근성 : 중앙집중화, 표준화 형식, 실시간 활용 가능성  
- 보안·거버넌스 : 접근 제어, 데이터 보안, 버전 관리  

&lt;구현전략&gt;  
- 1단계 : 데이터 인프라 구축(데이터 패브릭, 데이터 레이크)  
- 2단계 : 품질 관리 체계(자동화 검증, 스키마 검증)  
- 3단계 : 메타데이터 관리(카탈로그, 큐레이션)  

&lt;기술 요소&gt;  
- 데이터 패브릭(Data Fabric) : 분산 데이터를 통합·연결하여 일관된 접근 지원  
- AI 데이터 레이크(Data Lake) : 대규모 원천 데이터 저장·분석  
- 메타데이터 카탈로그 : 데이터셋의 위치·속성·사용이력 관리  
- FinOps for AI : 클라우드 기반 AI 비용 효율적 관리  

*DataOps → MLOps → ModelOps(선택적) 순으로 AI Ready Data 활용 구조  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능 투명성 확보 가이드라인

**[정의]**  

- 이용자가 AI 기반 서비스 이용 사실과 결과물의 AI 생성 여부를 명확히 인식하도록 하여 혼동을 방지하고 사회적 신뢰를 확보하기 위해 정의된 가이드라인  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 인공지능 기본법 제31조 “인공지능 투명성 확보 의무”  
- 시행령 제23조, 인공지능 투명성 확보 의무 이행  

&lt;적용대상&gt;  
- 최종 서비스 제공 사업자, API 활용 서비스 사업자, 모델 개발자(직접 제공 시), 해외 사업자  

&lt;제외 대상&gt;  
- 단순 이용자, 결과물 활용자, 콘텐츠 제작자 등  

&lt;법조항 세부내용&gt;  
- 법 제31조 제1항 : 사전 고지 의무  
  ㄴ고영향 AI 및 생성형 AI를 이용한 제품·서비스 제공 시 제품·서비스가 고영향 AI 또는 생성형 AI 기반으로 운영된다는 사실을 사전에 고지  

- 법 제31조 제2항 : 표시 의무  
  ㄴ생성형 AI 및 이를 이용한 제품·서비스 제공 시 결과물이 AI에 의해 생성되었다는 사실을 표시  

- 법 제31조 제3항 : 딥페이크 생성물 표시 의무  
  ㄴ AI 시스템으로 실제와 구분하기 어려운 가상의 생성 결과물 제공 시 해당 생성 결과물이 AI로 생성되었다는 사실을 고지 또는 표시  

&lt;시행령 투명성 의무별 상세&gt;  
- 제23조 제1항 : 사전 고지 방법(문서 기재, 화면·단말 표시, 제공 장소 게시, 인정 방식)  
- 제23조 제2항 : 표시 방법 (표시 방식, 안내 의무)  
- 제23조 제3항 : 딥페이크 생성물 표시 의무 관련 고려사항(인식 용이성, 이용자 특성 고려)  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능 안전성 확보 가이드 라인(고성능 AI 안전성 확보 가이드라인)

**[정의]**  

- 인공지능 안전성 확보 의무를 실제 이행하는 데 필요한 기준과 절차를 체계적으로 정리한 참고 문서  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 인공지능 기본법 제32조 “인공지능 안전성 확보 의무”  
- 시행령 제24조 “인공지능 안전성 확보 의무”  

&lt;가이드라인 구성&gt;  
1\. 적용 대상 및 의무 주체 판단  
2\. 수명주기 전반 위험관리  
3\. 위험관리 체계 구축  
4\. 보고 및 제출  

&lt;가이드라인 세부내용&gt;  
5\. 적용 대상 및 의무 주체 판단  
  1) 적용 대상 판단  
  - 연산량 10^26 FLOPs 이상  
  - 최첨단 기술 적용  
  - 생명·안전·기본권 중대 영향 가능성 기준 충족  

  2) 의무 주체 판단  
  - 적용 대상 AI가 되게 한 원인 행위 수행자에게 의무 부여  
  - AI를 설계·학습·구현·제공한 개발사업자  
  - 기존 AI를 실질 변경하여 고위험 AI로 전환한 변경사업자  

6\. 수명주기 전반 위험관리  
  1) 위험 식별  
  - 기획, 데이터 수집·전처리, 모델 설계·학습, 검증·평가, 배포·운영·종료 단계에서 위험 식별  
  - 기능 오류, 데이터 편향, 보안 취약점 등 기술적 위험 식별  
  - 절차 : 준비 → 정보 수집 → 위험 발굴 → 기록 관리 → 검증 → 갱신  

  2) 위험 평가  
  - 심각성, 중대성, 실현 가능성, 빈도, 관리 가능성 기준 평가  
  - 각 항목 1~3점 측정  
  - 최종 위험 점수 산정  

  3) 위험 완화  
  - 완화 조치 수립 및 실행  
  - 결과 문서화  
  - 긴급 대응 계획 수립  

7\. 위험관리 체계 구축  
  1) 안전사고 대응 및 예방  
  - 대응 조직 구성  
  - 대응 절차 수립  
  - 교육·훈련 수행  

8\. 보고 및 제출  
  1) 안전성 확보 결과 제출  
  - 적용 대상 인지 후 초기 제출  
  - 추가 사유 발생 시 추가 제출  

  2) 사고 발생 시 보고:  
  - 24시간 내 최초 보고, 7일 내 초동조치 보고, 15일 내 처리 결과 보고  

<적용 대상 판단 기준 : 누적 연산량 확인 방식>
  1) 이론적 계산식  
  - 인공지능 모델의 설계 정보나 모델 구조를 기반으로 수학적으로 연산량을 추정하는 방식  
  - 세부 방식 : 설계 정보 기반 방식, 모델 구조 기반 방식  

  2) 경험적·통계적 추정식  
  - 학계·산업계의 경험적 수치를 기반으로 파라미터 수, 토큰 수 등 일부 지표만으로 연산량을 예측하는 방식  
  - 세부 방식 : 경험적 계수 기반 방식, 시퀀스 기반 방식  

  3) GPU 사용량 기반 추정식  
  - GPU·TPU 등 하드웨어 자원의 실제 사용량을 기반으로 연산량을 계산하는 실측 중심 방식  
  - 세부 방식 : 단일 GPU 장비 기반 방식, 다중 GPU 장비 기반 방식  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능 영향평가 가이드라인

**[정의]**  

- 사업자가 인공지능 제품·서비스가 인간의 존엄성과 기본권에 미치는 잠재적 영향을 사전에 식별·분석하고, 이를 존중·보호하는 방향으로 개선방안을 마련·이행하도록 유도하는 가이드라인  

**[핵심/키워드]**  

&lt;인공지능 영향평가 개념&gt;  
- 고영향 AI 제품·서비스 제공 전, 인간의 기본권에 미치는 영향을 사전 평가하는 절차  

&lt;법적근거&gt;  
- 인공지능 기본법 제35조(고영향 인공지능 영향평가): 영향평가 수행 노력 의무, 국가기관은 평가 수행 제품 우선 고려  
- 시행령 제28조(수행 방법 등)  

&lt;평가대상&gt;  
- 고영향 AI 제품·서비스 제공 사업자 중심  
- 사전 고영향 여부 판단 필요(필요 시 정부 확인 요청)  
- 법은 고영향 중심이나 모든 AI 서비스 자율 수행 권장  

&lt;평가시기&gt;  
- 신규 서비스 출시 전 수행,  기능/대상 변화 시 재평가 권장  
- 기존 서비스도 필요 시 자율 수행  

&lt;평가수행주체&gt;  
- AI 사업자 직접 수행 또는 제3자 위탁 가능  

&lt;영향 평가 절차&gt;  사본사  
① 사전 준비 단계 : 평가 필요성 검토, 평가 대상 정의  
② 본 평가 수행 단계 : 피영향자 분석, 작동원리 분석, 기본권 영향 식별 및 분석  
③ 사후 단계 : 후속 조치, 문서 관리 및 공개  

### [인공지능, 법/제도, ITPE모의고사 ] LiteLLM

**[정의]**  

- 다양한 LLM을 하나의 API로 호출할 수 있는 오픈소스 Python 라이브러리 및 프록시 서버  

**[핵심/키워드]**  

&lt;특징&gt;  
- 연동 복잡성 제거 : 여러 인공지능 모델 연계(OpenAI, Anthropic 등)  
- 개발 생산성 : 멀티 모델 환경에서 빠른 연계 및 개발 생산성 향상  
- Python SDK : 단일 코드로 다양한 모델 호출 가능  
- Proxy Server(AI Gateway) : 중앙 관리 및 라우팅  

&lt;기능요소&gt;  
1) 핵심기능  
- API 표준화 : 여러 LLM의 API를 하나의 형식으로 통합  
- 요청 라우팅 및 모델 전환 : 요청 상황에 따라 적절한 모델로 자동 분기 및 전환  
- 자동 fallback : 장애 발생 시 다른 모델로 자동 대체 호출하여 안정성 확보  

2) 운영기능  
- 비용 추적 : 사용량 기반 비용 및 과금 내역 관리  
- Rate Limit / Budget 관리 : 요청 제한 및 예산 설정으로 비용 통제  
- 로깅 및 모니터링 : 요청/응답 기록 및 시스템 상태 추적  

3) 연계기능  
- 다양한 LLM 연동 : 100개 이상의 모델과 연동 지원  
- OpenAI 호환 API : 기존 OpenAI 코드 그대로 사용 가능  
- Load Balancing / Failover : 트래픽 분산 및 장애 대응을 통한 안정적인 서비스 운영  

### [인공지능, 법/제도, ITPE모의고사 ] 자율주행 AI

**[정의]**  

- 인공지능 기술을 활용하여 인간 운전자의 개입 없이 차량이 스스로 주변 환경을 인식하고, 판단하며, 주행 경로를 결정하여 운행하는 기술 체계  

**[핵심/키워드]**  

&lt;기술유형&gt;  
- 규칙 기반(Rule-based) : 사람이 정의한 규칙에 따라 차량 제어  
  ㄴ기술요소 : FSM(Finite State Machine), Rule-based Control  

- 모듈형(Modular AI) : 인식·예측·계획·제어를 분리한 파이프라인 구조  
  ㄴ기술요소 : CNN 기반 인식, SLAM, EKF, Planning 알고리즘(A*, MPC)  

- End-to-End AI : 센서 입력부터 제어까지 하나의 신경망으로 처리  
  ㄴ기술요소 : Deep Neural Network, Transformer 기반 모델  

&lt;기술요소별 알고리즘&gt;  
1) 센싱  
 - 카메라 : CNN, Vision Transformer(ViT)  
 - 라이다(LiDAR) : PointNet, VoxelNet  
 - 레이더(Radar) : FMCW Radar, CFAR  
 - 초음파 : Time-of-Flight(ToF)  

2) AI 알고리즘  
 - 인식(Perception) : YOLO, Faster R-CNN  
 - 센서퓨전 : BEVFormer  
 - 위치추정(Localization)  : EKF, SLAM  
 - 예측(Prediction) : Transformer  
 - 경로계획/제어 : A*, MPC  

### [인공지능, 법/제도, ITPE모의고사 ] 알파마요 AI

**[정의]**  

- 기존 자율주행 AI가 패턴 인식에 의존하던 한계를 넘어, 인간처럼 원인과 결과를 추론(Chain-of-Causation)하여 주행 결정을 내리는 추론 기반 자율주행 오픈소스 AI 모델 패밀리  

**[핵심/키워드]**  

&lt;구성요소&gt;  
- Alpamayo R1 : 10B 파라미터 추론형 VLA 모델  
- AlpaSim : 오픈소스 시뮬레이션 프레임워크  
- Physical AI AV Dataset : 대규모 주행 데이터셋  

&lt;특성&gt;  
- 성능특성 : 주행안전성, 자율주행 수준(레벨2++수준 구현)  
- 학습특성 : 시뮬레이션 기반 학습, 데이터 규모(약 100만 시간 실제 +가상 데이터 활용)  
- 기술특성: 센서 구성(약 100만 시간 실제 +가상 데이터 활용), 인지방식(라이다 미사용,HD맵 의존 제거), 구조특징(비용 절감 +글로벌 확장성 확보 구조)  

### [인공지능, 법/제도, ITPE모의고사 ] 하네스 엔지니어링(Harness Engineering)

**[정의]**  

- 프롬프트 단계를 넘어 AI에게 도구, 메모리, 제어 환경을 제공하여 실수를 방지하고 결과물의 품질을 높이는 엔지니어링 기술  

*강력한 AI 에이전트(LLM)가 안전하고 안정적으로 작업을 수행하도록 감싸는, 스캐폴딩(구조)과 피드백 루프를 설계하는 기술  

**[핵심/키워드]**  

&lt;필요성&gt;  
- 모델의 범용화, 에이전트의 프로덕션 전환, 에이전트의 프로덕션 전환  

&lt;구성요소&gt;  
- 파일시스템&저장소 : 상태 유지 및 작업 기록  
- 코드 실행&샌드박스 : 안전한 코드 실행 환경 제공  
- 컨텍스트 관리 : 컨텍스트 부패(Context Rot) 방지  
- 서브 에이전트 : 작업 분리 및 컨텍스트 격리  
- Hook : 사전/사후 동작 자동 삽입 → 자동 검증 및 정책 적용  
- Backpressure : 처리 과부하 시 실행 속도 자동 조절 → 파이프라인 안정성 및 처리량 보장  

&lt;설계전략&gt;  
- 최소 개입(Minimal Intervention) : 모델이 스스로 교정할 수 없을 때만 개입  
- 점진적 공개(Progressive Disclosure) : 최소 권한으로 시작, 필요에 따라 확장  
- 빠른 실패와 복구(Fail-fast with Recovery) : 실패를 빠르게 감지하고 fallback(대체 동작) 메커니즘 제공  
- 단순하게 시작(Start Simple) : 복잡한 제어 흐름 지양, 원자적 도구 제공  
- 삭제를 위해 구축(Build to Delete) : 모듈식 아키텍처, 새 모델에 맞춰 교체 가능  

Start Simple                   → 단순하게 시작  
      ↓  
Progressive Disclosure  → 필요할 때만 권한 확장  
      ↓  
Minimal Intervention      → 모델 자율성 최대한 존중  
      ↓  
Fail-fast + Fallback        → 실패 시 빠르게 감지·복구  
      ↓  
Build to Delete               → 언제든 교체 가능하게 모듈화  

### [인공지능, 법/제도, ITPE모의고사 ] OWASP Top 10:2025

**[정의]**  

- 웹 애플리케이션에서 가장 빈번하고 치명적인 보안 취약점 Top 10을 정리한 글로벌 표준 가이드  

*개발·운영 전 단계에서 보안 설계 및 취약점 대응 기준으로 활용  

**[핵심/키워드]**  

&lt;2025의 변화&gt;  
- 근본 원인(Root Cause) 중심 재분류  
- S/W 공급망 보안 실패(A03) 신규 강조  
- 예외 조건 처리 미흡(A10) 신규 항목 추가  

&lt;구성항목&gt; : 접설공암인설인무로예  
A01:2025 - Broken Access Control(취약한 접근 제어)  
A02:2025 - Security Misconfiguration(보안 설정 오류)  
A03:2025 - Software Supply Chain Failures(소프트웨어 공급망 실패)  
A04:2025 - Cryptographic Failures(암호화 실패)  
A05:2025 - Injection (인젝션)  
A06:2025 - Insecure Design(안전하지 않은 설계)  
A07:2025 - Authentication Failures(인증 실패)  
A08:2025 - Software or Data Integrity Failures(소프트웨어 또는 데이터 무결성 실패)  
A09:2025 - Logging & Alerting Failures(로깅 및 경고 실패)  
A10:2025 - Mishandling of Exceptional Conditions(예외 처리 오류)  

### [인공지능, 법/제도, ITPE모의고사 ] 맘바(Mamba)

**[정의]**  

- 선택적 상태공간모델(SSM, Selective State Space Model) 기반으로 긴 시퀀스를 효율적으로 처리하도록 설계된 시퀀스 모델  

**[핵심/키워드]**  

&lt;특징&gt;  
- 선택적 SSM(Selective SSM) : 상태기반 처리  
- Attention-Free : 어텐션 없이도 긴 문맥 파악  
- 선형(O(n)) 시간 복잡도 : 문장 길어져도 속도 일정  
- 고정 크기 상태 : 메모리 사용량 예측 가능  
- 하드웨어 친화적 : GPU 활용도 극대화한 설계  
- Selective Scan : 중요한 정보만 골라 기억하는 매커니즘  

&lt;구성요소&gt;  
- SSM 모듈 : 상태 기반 처리  
- Selective Scan : 정보 선택 최적화  
- MIMO 구조 : 다중 입출력  

*트랜스포머의 구조적 병목현상  
- O(n²)증가, KV캐시 증가, Decode병목  

### [인공지능, 법/제도, ITPE모의고사 ] 오픈클로(OpenClaw)

**[정의]**  

- 셀프 호스팅이 가능한 멀티채널 AI 에이전트 프레임워크  

*Node.js 기반으로 구동되며, MIT 라이선스를 따르는 오픈소스 프로젝트  

**[핵심/키워드]**  

&lt;특징&gt;  
- 자가 호스팅(Self-Hosting) : 로컬/개인서버에서 구동되는 AI 허브  
- 상시 실행형(Always-on) : 24시간 실행중인 데몬 프로세스  
- 확장성 : 멀티 메신저 연동 + 툴 호출 + 지속 실행 구조 결합 - 라이선스 : 자유로운 수정 및 배포 가능한 MIT 오픈소스  
- Gateway 중심구조  

&lt;핵심기능&gt;  
- 멀티채널 : 통합 채널 관리  
- 스킬 시스템 : Tool 기반 실행  
- 자동화 : 스케줄링(Cron)  
- 기억 : 퍼시스턴트 메모리  

&lt;활용사례&gt;  
- 개인 생산성 :일정관리,이메일,반복 업무 자동화  
- DevOps /개발 :코드 리뷰,CI파이프라인 모니터링,로그 분석, 알림  
- 기업 내부 :사내 문서 검색 (RAG),헬프 데스크 자동응답,프로젝트 요약  

&lt;오픈클로 보안취약점 및 대응방안&gt;  
- 프롬프트 주입 공격(PromptInjection) : Allow List 기본 적용  
- Tool오남용 : 최소 권한 원칙  
- API키 노출 : DM 페어링 정책(기기와 상호인증)  

### [인공지능, 법/제도, ITPE모의고사 ] 몰트북(Moltbook)

**[정의]**  

- 인간이 아닌, AI 에이전트만 활동하는 전용 SNS로써, 게시글, 댓글 생성, 토론을 수행하는 AI 전용 소셜 네트워크 플랫폼  

*AI Agent가 활동주체인 Agent-Native 플랫폼  

**[핵심/키워드]**  

&lt;운영핵심요소&gt;  
- 자율성 : 에이전트가 스스로 커뮤니티 생성 및 투표 수행 → 인간은 관찰자 역할 모든 활동 주체는 인공지능  
- 신원 레이어 : Identity Token 기반의 고유 식별 체계 → Identity Token 구조를 통해 각 에이전트의 평판(Karma)을 관리  
- Heartbeat : 주기적인 실행을 통한 지속적인 참여 루프 형성  

&lt;상세특징&gt;  
- 주요목적 : AIAgent가 활동주체인 Agent-Native플랫폼  
- 상호작용구조 : AI↔AI 자율 토론·게시·평가  
- 실행방식 : 주기적(Heartbeat)자동실행  
- 지능구조 : 다중 에이전트 협업·역할 기반 구조  
- 데이터생성 : AI가 스스로 콘텐츠 생산  
- 서비스사례: 몰트북,봇마당(국내)  

### [인공지능, 법/제도, ITPE모의고사 ] SDD(Spec-Driven Development)

**[정의]**  

- 명세를 단일 진실 공급원(SSoT)으로 활용하여 AI가 구현·테스트·문서를 생성하고, 사람은 설계·검증·개선을 담당하는 개발 방식  

**[핵심/키워드]**  

&lt;부각이유&gt;  
- 명세를 단일 기준으로 코드-명세 불일치 최소화  
- AI 기반 구현·자동화·코드 생성 확산  
- 개발 역할이 구현 중심 → 설계·검증·관리 중심으로 전환  

&lt;개념변화&gt;  
- 개발 중심이 코드 작성 → 명세 기반 구현으로 이동  
- 명세 중심 개발 패러다임으로 재편  

&lt;핵심원칙&gt;  
- Spec First : 구현 이전에 명세를 먼저 정의  
- Spec as Source of Truth : 명세를 단일 기준(SSoT)으로 관리  
- AI Guided by Explicit Rules : AI가 이해 가능한 구조화된 명세 기반 수행  
- Feedback Back to Spec : 결과·피드백을 명세에 지속 반영  

&lt;수행절차&gt;  
① 스펙정의 : 요구사항·기능·제약을 명세로 구체화  
② 계획수립 : 구현 범위·일정·자원 계획 수립  
③ 가드레일 설정 : 규칙·검증·제약 조건 정의  
④ AI 구현생성 : 명세 기반 코드·테스트·문서 자동 생성  
⑤ 검증·피드백 : 결과 검증 후 명세 개선 및 반복 적용  

### [인공지능, 법/제도, ITPE모의고사 ] RX(Robot Transformation)

**[정의]**  

- 로봇에 AI, 빅데이터, 클라우드, IoT, 자율제어 기술을 결합하여 단순 반복 작업 수행 로봇에서 상황인지 → 판단 → 자율 행동 → 학습이 가능한 지능형 로봇으로 전환하는 패러다임  

**[핵심/키워드]**  

&lt;특징&gt;  
- 워크플로우 재설계  
- 피지컬 AI(Physical AI)와의 결합  
- 공간 및 시스템 아키텍처 설계  
- AX(AI 전환)의 완성  

&lt;기술요소&gt;  
1\. 센싱 시스템(Perception & Sensing)  
 - 시각 센서 : RGB-D 카메라, 스테레오 카메라, LiDAR(2D/3D), ToF 센서  
 - 환경/상태 센서 : IMU(가속도/자이로), 초음파 센서, 토크 센서(Torque)  

2\. 인공지능 HW 및 시스템 SW(Computing & Platform)  
 - AI 가속기/반도체 : NVIDIA Orin/Thor, NPU(Neural Processing Unit), TPU  
 - 운영체제 및 미들웨어 : ROS2(Humble/Foxy), RTOS(FreeRTOS, QNX), 무선 통신(5G/6G)  

3\. 인공지능 SW 및 모델(Intelligence & Model)  
 - 인지/판단 SW : SLAM(위치 추정 및 지도 작성), YOLO(객체 인식), Open-Vocabulary 감지  
 - 로봇 파운데이션 모델 : VLA(Vision-Language-Action) 모델, RT-2, PaLM-E  
 - 학습 및 시뮬레이션 : 디지털 트윈(NVIDIA Isaac Sim, MuJoCo), 데이터 증강  

4\. 액추에이션 및 제어 시스템(Drive & Control)  
 - 모빌리티/모터 : 고출력 BLDC 모터, 중공축 모터(Frameless Motor), 인휠 모터(In-wheel)  
 - 정밀 감속기 : 하모닉 드라이브(Strain Wave Gearing), RV 감속기(사이클로이드)  
 - 제어 알고리즘 : MPC(모델 예측 제어), 임피던스/어드미턴스 제어, 심층강화학습(DRL)  

5\. 로보틱스 바디 및 인프라(Structure & Energy)  
 - 신소재/경량화 : 탄소섬유 복합재(CFRP), 고강도 알루미늄, 엔지니어링 플라스틱  
 - 에너지 시스템 : 고밀도 배터리 팩, BMS(배터리 관리 시스템), 자동 도킹 충전 스테이션  
 - 디자인 구조 : 휴머노이드 아키텍처, 4족 보행 구조, 다관절 협동 로봇(Cobot) 링크 구조  

### [인공지능, 법/제도, ITPE모의고사 ] RLHF(Reinforcement Learning from Human Feedback)

**[정의]**  

- 인간 평가자가 모델 출력에 대해 선호/품질 피드백을 제공하고 이를 강화학습에 반영하는 학습 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
- 인간 기준 정렬(HumanAlignment), 안전성·윤리성 확보에 유리  

&lt;동작구조&gt;  
1\. 관찰(Observation)  
2\. 행동(Action)  
3\. 보상예측기(Reward Predictor)  
4\. 인간피드백(Human Feedback)  
5\. 예측된 보상(Predicted Reward)  

*인간 피드백 수집 →보상모델 학습 →RL로 모델 최적화  

&lt;장점&gt;  
- 결과 신뢰성 높음, 인간 의도 반영 정확  

&lt;한계&gt;  
- 비용 높음(라벨링 인력 필요), 확장성 제한  

<참고 : RLAIF(Reinforcement Learning from AI Feedback)>
- AI 모델이 다른 모델의 출력에 대해 자동 평가/피드백을 생성하고 이를 강화학습에 활용  
 → RLHF의 피드백 주체는 인간 평가자, RLAIF는 AI평가 모델임  

### [인공지능, 법/제도, ITPE모의고사 ] 개인정보 이노베이션 존

**[정의]**  

- 데이터 처리 환경의 안전성을 높여 가명정보를 보다 유연하게 활용할 수 있도록 지원하는 공간  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 개인정보보호법 제28조의7  

&lt;도입시기 및 현황&gt;  
- 연구자와 기업들이 양질의 데이터를 보다 안전하게 활용할 수 있는 기반을 마련하기 위해 지난 2024년 도입  
- 통계청, 국립암센터, 한국사회보장정보원, 더존비즈온, 한국도로공사 등 5곳이 지정  

&lt;주요기능&gt;  
1) 개인정보(가명정보)의 유연한 활용 지원  
  - 가명처리 수준 완화  
  - 비정형데이터 활용, 국가통계 특화형 안심구역 운영  
  - 가명정보 장기보관 및 재사용  

2) 개인정보보호 강화기술(PET) 실증 지원  
  - PET를 적용한 개인정보 처리 허용  

&lt;기대효과&gt;  
- 장기활용(5년+추가연장), 재사용 제3자 제공 가능, 빅데이터 샘플링 검사 허용, 결합키 다양화  

### [인공지능, 법/제도, ITPE모의고사 ] 데메테르의 법칙(Law of Demeter)

**[정의]**  

- 객체가 자신과 직접 관련된 객체하고만 상호작용하도록 제한하는 최소 지식 원칙(Principle of Least Knowledge)  

*객체 간 결합도를 낮추고 캡슐화를 강화하기 위한 객체지향 설계 원칙  

**[핵심/키워드]**  

&lt;활용&gt;  
- 마이크로서비스 : 다른 서비스의 내부 데이터 구조에 의존하지 않고 공개 API로만 연계  
- 객체지향 설계 : 객체가 다른 객체의 내부 구조를 직접 탐색하지 않도록 설계  

&lt;목적&gt;  
- 객체 간 결합도 감소  
- 캡슐화 강화  
- 유지보수성과 변경 대응력 향상  

&lt;데메테르의 법칙 설계 원칙&gt;  
- 핵심원칙 : 객체가 직접 알고 있는 대상과만 상호작용하도록 하여 최소 지식 원칙과 연쇄 호출 지양  
- 호출가능 대상 : 객체자신, 매개변수, 직접생성객체, 직접 관리하는 멤버객체, 접근 가능 전역 객체  
- 구현기법 : 위임은닉, Tell Don’t Ask, 정보전문가, 파사드패턴, 내부구 조 노출과 객체 간 결합 최소화  

### [인공지능, 법/제도, ITPE모의고사 ] 지식재산 기본법

**[정의]**  

- 지식재산의 창출ㆍ보호 및 활용을 촉진하고 그 기반을 조성하기 위한 정부의 기본 정책과  추진 체계를 마련하여 우리 사회에서 지식재산의 가치가 최대한 발휘될 수 있도록 하는  법률(2011.7.20. 최초 시행)  

*지식재산(IP)관련 기반 법률  

**[핵심/키워드]**  

&lt;지식재산권의 유형&gt;  
- 산업재산권 : 특허권, 실용신안권, 디자인권, 상표권  
- 저작권 : 협의의 저작권, 저작인접권  
- 신지식 재산권 : 첨단 산업 재산권, 산업저작권, 정보재산권, 기타  

&lt;FRAND 원칙 정의&gt;  
- Fair(공정), Reasonable(합리), Non-Discriminatory(비차별)의 약자로, 표준필수특허(SEP) 보유자가 타 기업에 공정하고 합리적이며 비차별적인 조건으로 라이선스를 제공해야 한다는 원칙  
- 주요요소 : 공정성, 합리성, 비차별성  

### [인공지능, 법/제도, ITPE모의고사 ] ISO/IEC 33000

**[정의]**  

- 소프트웨어 및 시스템 개발 프로세스의 평가 및 개선을 위한 국제 표준  

*ISO/IEC15504(SPICE)를 개정,프로세스 품질 특성 평가와 조직 성숙도 측정을 위한 프레임워크를 제공  

**[핵심/키워드]**  

- 조직의 IT 및 소프트웨어 프로세스를 정량화 해 0~5단계로 평가하는 국제 프로세스 역량 모델 표준  

- 표준 구조 : 모듈형 구조로 통일  
- 용어체계 : 용어와 개념 정비  
- 적용분야 : 다양한 산업 적용 가능  
- 개발방식반영 : 애자일·DevOps 반영  
- 평가체계 : 공통 평가 프레임 제공  

### [인공지능, 법/제도, ITPE모의고사 ] 생성형 AI 산출물 저작권

**[정의]**  

- 생성형 AI가 단독으로 생성한 산출물은 현행법상 저작권법의 보호를 받을 수 없음  

*저작권 인정의 핵심 기준: '인간의 창작적 기여'  

**[핵심/키워드]**  

&lt;생성형 AI 학습 데이터 저작권 문제&gt;  
- 데이터 무단 수집 및 이용에 따른 침해 가능성, 공정이용 여부의 불확실성, 생성물에 대한 저작권 귀속 문제가 핵심, 공정이용(Fair Use) 논란 – 법원 판례와 정책 논의중  

&lt;생성형 AI 결과물 분류&gt;  
- 인간의 창작적 기여 있음 : GAI 활용 저작물  
- 인간의 창작적 기여 없음 : GAI 산출물  

&lt;저작권 인정 여부&gt;  
- 인정 않됨 : 원칙  
- 인정 가능 : 인간의 창의성이 담긴 편집, 배열, 수정 등의 작업을 가하여 창작을 더했다면 인정  

&lt;인간의 창작적 기여 판단 방안&gt;  
- 통제가능성, 예측가능성  

### [인공지능, 법/제도, ITPE모의고사 ] CISO(Chief Information Security Officer, 정보보호최고책임자)

**[정의]**  

- 조직 내 정보보호 및 보안 전반을 총괄하는 최고 책임자로, 정보보호 정책 수립, 위험관리, 보안 사고  
대응, 보호대책 운영 등을 담당하는 임원급 역할  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 정보통신망법, 제45조의3(정보보호 최고책임자의 지정 등)  

&lt;지정의무&gt;  
- 정보통신서비스 제공자는 정보보호 최고책임자(CISO)를 지정 및 과기정통부에 신고해야 함  
- 자산총액, 매출액 등 대통령령 기준에 해당하는 기업은 신고 예외 가능  

&lt;주요업무&gt;  
- 정보보호 계획 수립 및 개선  
- 정보보호 실태 감사 및 개선  
- 위험 식별 및 대책 마련  
- 정보보호 교육·훈련 계획 수립 및 시행  

&lt;정보통신망법 개정에 따른 CISO 변화&gt;  
- 2026년 3월 24일 의결, 9-10월 시행 예정  
- 임원급 지정 의무화  
- 업무에 정보보호 인력 관리, 예산 편성이 명문화  
- 이사회 보고 의무  

<참고 : CPO(Chief Privacy Officer, 개인정보보호책임자)>
- 개인정보 보호 업무 전반을 총괄하고 체계적으로 관리·감독하는 책임자  
- 조직 내 개인정보 보호계획 수립·시행, 처리 실태 개선, 내부 통제, 교육, 파일 관리·감독 등 수행  

### [인공지능, 법/제도, ITPE모의고사 ] 다단계 페이지 테이블(Multi-level Page Table, = 계층적 페이징)

**[정의]**  

- 페이지 테이블을 여러 단계(2~4단계)로 분리해 주소 변환 수행하는 구조  

**[핵심/키워드]**  

&lt;특징&gt;  
- 페이지 디렉터리 → 페이지 테이블 → 프레임 번호  
- 가상주소의 상위/하위 Page Number를 단계별 분할 사용  

&lt;구성요소&gt;  
- 가상주소(Virtual Address) : 페이지 번호와 오프셋(Offset)으로 구성된 논리적 주소  
- 페이지 디렉터리(Page Directory) : 상위 레벨 테이블로, 하위 페이지 테이블의 위치를 가리키는 엔트리 집합  
- 페이지 테이블(Page Table) : 가상 페이지 번호를 물리 프레임 번호로 매핑하는 하위 레벨 테이블  
- 페이지 테이블 엔트리(PTE) : 프레임 번호와 유효 비트, 보호 비트(읽기/쓰기/실행) 등을 포함  
- 프레임(Frame) : 실제 물리 메모리의 고정 크기 블록  
- TLB(Translation Lookaside Buffer) : 최근 주소 변환 결과를 캐시하여 주소 변환 속도 향상  

&lt;주소변환 과정&gt;  
1\. 가상주소 분해 : CPU가 생성한 가상주소를 상위 Page Number / 하위 Page Number / Offset으로 분리  
2\. TLB 조회 : 먼저 TLB에서 해당 가상주소 매핑 존재 여부 확인  
3\. 히트 : 즉시 물리주소 생성  
4\. 미스 : 페이지 테이블 탐색 수행  
5\. 페이지 디렉터리 접근 : 상위 Page Number로 페이지 디렉터리 엔트리(PDE) 조회 → 하위 페이지 테이블 위치 확인  
6\. 페이지 테이블 접근 : 하위 Page Number로 페이지 테이블 엔트리(PTE) 조회 → 프레임 번호(Frame Number) 획득  
7\. 유효성 검사 : PTE의 Valid/Protection 비트 확인  
8\. 무효 시 : 페이지 폴트(Page Fault) 발생 → OS 개입  
9\. 물리주소 생성 : 프레임 번호 + Offset 결합 → 최종 물리주소 생성  
10\. TLB 갱신 : 변환 결과를 TLB에 캐시하여 이후 접근 속도 향상  

&lt;다단계 페이지 테이블의 개선 효과 &gt;  
- 필요한 영역만 테이블 생성하여 메모리 사용량 대폭 감소  
- 대규모 가상주소 공간에서도 확장성 확보  
- 희소한 주소 공간(Sparse Address Space)에 효율적  
- TLB와 결합 시 성능 저하를 최소화하면서 현대 OS 표준 구조로 정착  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능 기본법

**[정의]**  

- 인공지능 기술의 발전과 활용에 따라 발생하는 다양한 사회적, 윤리적, 법적 문제를 해결하기 위해 제정된 법률  

**[핵심/키워드]**  

&lt;법체계&gt;  
- 인공지능 발전과 신뢰 기반 조성 등에 관한 기본법 제6장 43조로 구성  

&lt;용어정의&gt;  
- 고영향 AI, 생성형 인공지능, 고성능 AI(안전성 확보 의무대상)  

&lt;주요내용&gt;  
- 인공지능 기본계획 수립  
- 인공지능 윤리 원칙  
- 인공지능 투명성/안전성 확보 의무  
- 고영향 인공지능 영향 평가  

&lt; AI 기본법 추진 일정&gt;  
- 2026.01.20 : 개정 법률 확정 <= 사전 개정  
- 2026.01.22 : 기본법 시행 및 일부 즉시 시행  
- 2026.05.21~06.19 : 시행령 입법예고  
- 2026.07.21 : 하위법령 포함 본격 시행  
→ 단계적 제도 정착 구조  

&lt;AI 기본법 개정 목적&gt;  
- AI 산업 육성 기반 강화  
- 공공분야 AI 도입·활용 촉진  
- AI 연구소 설립·운영 근거 마련  
- AI 취약계층 접근성 보장 및 비용 지원  
- AI 창업·전문인력·학습용 데이터 활용 지원  

- 제3조 제5호(AI 취약계층 정의 : 이용 어려운 자 정의)  
- 제7조 제2항·제3항(국가 AI 전략위원회 : 위원·부위원장 확대)  
- 제8조 제1항(전략위원회 기능 : AI 정책 심의·의결 확대)  
- 제16조 제3항(공공분야 AI 도입 : AI 제품·서비스 우선 고려)  
- 제16조 제4항(공공 AI 면책 : 고의·중과실 없으면 담당자 책임 면제)  
- 제17조의2(AI 비용 지원 : 이용 비용 지원 가능)  
- 제18조 제3항(AI 창업 지원 : 모태펀드 활용 지원)  
- 제18조 제4항 제2호(AI 창업 민간 펀드 : 민간 참여 펀드 근거)  
- 제21조 제1항(AI 전문인력 지원 : 인력 양성 시책 추진),  
- 제22조의2(AI 연구소 설립 : 대학·기업 연구소 설립 근거),  
- 제2조 제12호(학습용 데이터 정의 : AI 개발·활용 데이터 정의),  
- 제6조 제2항 제4호의2(공공데이터 학습용 제공 : 제공 기준·절차 마련),  
- 제6조 제3항(행안부 협의 : 공공데이터 제공 협의 규정)  

### [인공지능, 법/제도, ITPE모의고사 ] 디지털 포용법

**[정의]**  

- 디지털포용 증진과 관련 산업의 육성에 관한 사항을 규정함으로써 사회구성원의 삶의 질 향상과 사회통합에 이바지함을 목적으로 하는 법률  

**[핵심/키워드]**  

제1장 총칙  
- 제3조(국가 및 지방자치단체 등의 책무)  
- 제4조(대체수단의 제공)  
- 제5조(지능정보기술의 부작용 예방·해소)  
- 제6조(지능정보사업자의 책무)  

제2장 디지털포용 정책의 추진체계  
- 제8조(디지털포용 기본계획)  
- 제9조(디지털포용 시행계획)  
- 제11조(실태조사 등)  
- 제12조(디지털포용 영향평가)  

제3장 디지털역량의 함양  
- 제15조(디지털역량센터의 지정 등)  
- 제18조(디지털취약계층의 사회 참여 지원)  

제4장 지능정보서비스 등의 이용환경 보장  
- 제19조(지능정보서비스 등에 대한 접근성 보장)  
- 제20조(무인정보단말기 이용 편의 제공)  
- 제22조(접근성 품질인증의 신청 등)  
- 제23조(접근성이 보장된 지능정보제품의 우선구매)  

제5장 지능정보기술 등의 포용적 활용 촉진  
- 제26조(디지털포용기술·서비스의 표준화)  
- 제28조(디지털포용 관련 기술·서비스의 연구·개발)  
- 제30조(디지털포용기술·서비스의 수출지원)  

### [인공지능, 법/제도, ITPE모의고사 ] ISMP(Information Strategy Management Planning)

**[정의]**  

- 정보 시스템 구축을 위한 업무 및 기술 현황과 사용자 요구를 분석해 목표 시스템의 기능적·기술적 요구를 정리하는 활동  

**[핵심/키워드]**  

&lt;배경&gt;  
- ISP의 형식적 수립과 정보화사업 구축ㆍ운영 부실화 등 문제 제기  
- 데이터 표준화 미준수, 정보시스템 활용률 저조 등 부실 운영  
- 기존 정보시스템 재활용 미흡, 중복구축 사업 추진 등 예산 낭비  

&lt;필요성&gt;  
- ISP·ISMP 수립 절차 정립, 필요 공통사항과 기본요건 규정  
- 정보화사업 계획 단계 및 예산 편성·집행의 내실화  

&lt;ISMP 수립방법&gt;  
1\. 프로젝트 착수 및 참여자 결정  
2\. 정보시스템 방향성 수립  
3\. 업무 및 정보기술 요건 분석  
4\. 정보시스템 구조 및 요건 정의  
5\. 정보시스템 구축 사업 이행방안 수립  

- 소규모 정보시스템 구축 사업계획수립 안내(ISP,ISMP수립 의무 면제)  
- 클라우드 기술 적용 우선 검토  

- 총 4개 분야, 6개 검토항목  
- 분야 : 사업타당성, 실현가능성, 클라우드 우선 적용, 규모 적정성  
- 검토항목 : 필요성, 시급성, 중복성, 사업추진 여건, 기술적 구현성, 총구축비 적정성  

### [인공지능, 법/제도, ITPE모의고사 ] Sim2Real(Simulation-to-Reality)

**[정의]**  

- 시뮬레이션 환경에서 생성된 경험과 학습된 지능을 현실 세계로 이전하여, 실제 물리 환경에서도 안정적이고 신뢰성 있게 동작하는 행동 능력(Behavior Capability)으로 구현하는 전이(Transfer) 메커니즘  

**[핵심/키워드]**  

&lt;비교개념&gt;  
- 패스스루 : XR 헤드셋의 카메라로 촬영한 현실 영상을 디스플레이하고 가상객체를 결합하는 현실 시각화 기술  
→ Sim2Real은 가상에서 학습한 지능을 현실로 이전 기술, 패스스루는 현실을 XR 장치 안에 보여주는 기술  

&lt;핵심 기술요소&gt;  
- 합성 경험 생성:  물리 시뮬레이션, 디지털 트윈, 합성 데이터 생성  
- 도메인 랜덤화 : 시각 랜덤화, 동역학 랜덤화, 자동 도메인 랜덤화  
- 현실 적응 : 영상 변환, 도메인 적응, 특징 정렬  
- 물리 정합성 확보 : 동역학 보정, 시스템 식별, 적응형 시뮬레이션  
- 강건 정책 학습 : 강건 정책 학습, 고수준 정책 학습, 강건 강화학습  
- 현실 검증·보정 : 실제 환경 시험, 폐쇄루프 피드백, 모델·정책 미세조정  

### [인공지능, 법/제도, ITPE모의고사 ] 제로트러스트 가이드라인 2.0

**[정의]**  

- 기존 1.0(2023.7)의 원칙 기반 프레임워크를 바탕으로 국내 조직들이 실제 제로트러스트 보안 체계를 설계·구축·운영할 수 있도록 실질적 지침과 절차를 구체화한 개정판  

**[핵심/키워드]**  

&lt;주요내용&gt;  
- 발간시기 : 2024년 12월  
- 성숙도 모델, 도입 절차 상세화 등으로 실질적인 Zero Trust 도입 장벽 낮춤  
- 성숙도 4단계로 세분화  
- 52가지 세부역량 및 평가 체크리스트 제공  

<제로트러스트 2.0 성숙도 모델> : 성숙도 수준 4단계
- 최적(Optimal)  
- 고급(Advanced)  
- 초기(Initial)  
- 기존 환경(Traditional)  

<참고 : 제로트러스트 1.0 성숙도 모델>
- 기존(Traditional) > 향상(Advanced) > 최적화(Optimal)  

### [인공지능, 법/제도, ITPE모의고사 ] 국가망보안체계(N²SF, National Security Strategy Framework)

**[정의]**  

- 각급기관의 업무정보·정보시스템을 식별하고, 업무 중요도에 따라 기밀(Classified), 민감(Sensitive), 공개(Open)  
등급으로 분류하여 등급별로 차등적인 보안통제를 적용하는 보안 프레임워크  

**[핵심/키워드]**  

&lt;목표&gt;  
- 보안 패러다임 전환 : 모든 데이터 연계 및 융합, 민간 혁신 기술 활용 용이  
- 스마트 업무환경 : AI, 클라우드 등 연계 보장, 장소 및 시간 제약 없는 업무 수행  
- 최적화된 정책 : 해외 정책 비교 분석, 국내 설정에 적합한 정책 개발  
- 안정적인 정책 안착 : 새로운 보안 정책 공표 및 적용, 평가 및 검증 등 점진적 변화  
- 다양한 산업의 시장경제 창출 : 보안 신기술 개발 및 수요 창출, AI 및 데이터 산업 등 시장 확대  

&lt;등급체계&gt;  
- 등급 분류(C/S/O) : 기밀(Classified), 민감(Sensitive), 공개(Open) 등급으로 정보 구분  

&lt;적용절차&gt;  
1\. 준비(Prepare)  
2\. C/S/O 등급분류(Categorize)  
3\. 위협식별(Identify)  
4\. 보안대책 수립(Select)  
5\. 적절성 평가·조정(Assess)  
6\. 보안성 검토  

&lt;6개 통제영역&gt;  
-  권한·인증·분리·통제·데이터·정보자산 각 영역별 대응 수준 차등 적용  

&lt;정보서비스 모델&gt;  
- 인터넷 단말 업무, 생성형 AI, 외부 클라우드, R&D 환경 등 8~9개 사례 제시  

### [인공지능, 법/제도, ITPE모의고사 ] EU 사이버복원력법(CRA, Cyber Resilience Act)

**[정의]**  

- 디지털 요소를 포함하는 제품(Product with Digital Elements)에 대해 설계·개발·운영·유지보수 전 과정에서 사이버보안 요구사항을 준수하도록 규정한 EU의 제품 중심(Product-Centric) 보안 규제  

**[핵심/키워드]**  

&lt;추진배경&gt;  
- 공급망 공격 증가, IoT·연결기기 확산, 디지털 주권 확보, 규제 표준화 요구, 제품 보안성 및 소비자 보호 강화  

&lt;CRA 주요 요구사항&gt;  
- 보안 내재화 : 보안 설계(Secure by Design), 기본 보안 설정(Secure by Default)  
- 취약점 관리 : 제품 수명주기 전반의 취약점 관리 및 보안 업데이트 제공  
- 정보 공개 : 보안사고 보고, 기술문서 작성 및 SBOM 관리  
- 검증 : 제품 적합성 평가 및 CE 인증 수행  

&lt;대응전략&gt;  
- 보안개발체계 구축전략 : SSDLC 도입, 위협 모델링, 보안 설계 적용  
- 공급망보안 강화전략 : SBOM 구축, 오픈소스 취약점 관리, 공급망 위험관리 체계 구축  
- 인증대응체계 확보전략 : 적합성 평가 준비, 기술문서 관리, CE 인증 확보  

### [인공지능, 법/제도, ITPE모의고사 ] 마이데이터 2.0

**[정의]**  

- 금융·통신·공공 등 다양한 분야에서 개인이 자신의 데이터를 직접 통제하고 활용하며, 안전하고 편리하게 맞춤형 서비스를 받을 수 있도록 한 제도(금융 마이데이터 : 2022년 1월 전면 시행)  

**[핵심/키워드]**  

&lt;특징&gt;  
- 전체 금융자산 조회 : 모든 금융상품 일괄 조회  
- 오프라인 가입·조회·활용 : 대면 점포 에서 마이데이터 ①가입, ②조회, ③활용 가능  
- 어카운트 인포 연계 : 계좌 해지 기능을 사용할 수도록 연계  
- 동의 절차 간소화 : 1단계로 간소화  
- 본인정보 관리 강화 : 가입 내역 및 제공 내역을 조회·관리 시스템 구축  
- 유효기간 연장 : 1년에서 최대 5년까지 선택  
- 청소년 이용 개선 : 14세 이상 청소년은 마이데이터를 스스로 이용  
- 미활용 데이터 삭제 : 선택적으로 삭제 가능  

&lt;추진방향&gt;  
① 정보 확대  
- 전체 금융자산 조회, 결제내역 상세 제공, 공공 마이데이터 연계  
② 영업 활성화  
- 오프라인 접근 허용, 겸영·부수업무 완화, 정보 결합 기준 명확화  
③ 이용자 편의성  
- 동의 절차 간소화, 통합 가입·탈퇴 관리, 가입유효기간 연장, 청소년 독립 이용  
④ 정보보호 강화  
- 제3자 제공 보안, 장기 미사용 정보 폐기, 개별정보 삭제기능  

### [인공지능, 법/제도, ITPE모의고사 ] AISC(AI·SW 안전성 인증, Artificial Intelligence·Software Safety Certification)

**[정의]**  

- 민·관·국제 협력 체계(FKII, AIWORKX, KIWA) 통해, ISO 5469 및 ISO/IEC 42001을 기반으로 AI와 SW의 안전  
성, 성능, 공정성을 종합 평가하는 인증 제도  

**[핵심/키워드]**  

&lt;참여기관&gt;  
- 한국정보산업연합회(FKII, 운영/총괄), Kiwa(글로벌 인증/심사), AIWORX(KOLAS 시험)  

<인증·평가 체계>
- 3대 인증 영역 기반, 6종 세부 인증 서비스 운영  

&lt;절차&gt;  
- 신청/접수 → 시험·심사(AIS/API/AIAPI 기준) → 인증 부여 → 사후·갱신 심사  
- 12개월 주기 사후 관리, 3년 주기 갱신 심사  

&lt;기반 국제표준&gt;  
- ISO/IEC 5469 : AI 시스템 기능 안전 국제 표준  
- ISO/IEC 42001 : 인공지능 경영시스템 국제 표준  

&lt;3대 인증 영역&gt; : 안전성(AISL), 성능(AIPL), 공정성(AIFL)  
1\. 안전성(AISL, Safety Levels)  
  - 7개 수준(4, 3, 2, 1, 0.2, 0.1, 0) 분류  
  - 고위험군(4, 3레벨)은 시스템 재설계 권고  
2\. 성능(AIPL, Performance Levels)  
  - 성능·유용성 지표 충족 여부 기준  
  - Level 2~0 분류  
3\. 공정성(AIFL, Fairness Levels)  
  - 차별·편향성 대응 및 공정성 확보 여부 기준  
  - Level 2~0 분류  

&lt;6종 세부 인증&gt;  
- AI·SW 안전성 인증 : AI 개발 기업 및 적용 제품의 안전성 확보 여부 검증  
- AI 품질 검증 : 학습 데이터 적정성 및 모델 구현 여부 검증  
- AI·SW 시험 : AI 기반 SW·시스템·모바일/웹 구현 적합성 검증  
- AI 경영시스템 인증 : ISO/IEC 42001 기반 AI 경영시스템(AISMS) 구축 여부 검증  
- AI 안전경영 인증 : AI 안전경영시스템(AIFSM) 구축 여부 검증  
- AI 사이버보안 & SW Update 인증 : 보안 체계 및 SW 업데이트 시 안전성 확보 여부 검증  

### [인공지능, 법/제도, ITPE모의고사 ] 글로벌 CBPR

**[정의]**  

- 국경 간 개인정보 이전의 안전성과 신뢰성을 확보하기 위한 국제 인증제도  

**[핵심/키워드]**  

&lt;특징&gt;  
- 기업의 개인정보 보호 체계를 글로벌 협의체가 심사·인증  
- 2011년 APEC 지역 출범, 2022년 글로벌 협의체로 확대  

&lt;주요내용&gt;  
- 시행국가 :  한국, 미국, 일본 등 주도  
- 국내시행일 : 2025년 6월 2일 (KISA 공식 시행)  
- 목적 : 국경 간 안전한 개인정보 이전 촉진 , 전자상거래 활성화 , 인증 기업의 국제 신뢰도 제고  
- 요건 : 개인정보 관리체계 등 심사 필요 , 인증 시 타 국가로 개인정보 원활 이전 가능  
- 효과 : 해외 진출 시 기업 신뢰도 향상 , 기존 APEC CBPR 인증 기업(12개국)은 자동 전환 부여  

&lt;인증기준&gt;  
1\. 개인정보 관리 체계 수립(2)  
2\. 개인정보 수집(9)  
3\. 개인정보 이용·위탁·제공(7)  
4\. 정보주체 권리보장(9)  
5\. 무결성(5)  
6\. 보호 대책(16)  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능과 머신러닝 공급망 위험 및 완화방안 가이드라인

**[정의]**  

- AI/ML 공급망보안 중요성 강조하고 AI시스템을 개발하거나 구매할 때 고려해야 할 주요 위험과 완화 방안 제시하는 가이드라인  

**[핵심/키워드]**  

&lt;배경&gt;  
- AI/ML 활용 확대, AI 도입 증가, AX 확산 → AI/ML 공급망 보안 중요성 증가  

&lt;관리영역&gt;  
- AI 데이터 보안 : 학습·추론 데이터 보호 및 무결성 확보  
- ML 모델 보안 : 모델 탈취·조작·공격 방어  
- AI SW 보안 : AI 애플리케이션 취약점 및 코드 보안  
- 제3자 서비스 보안 : 외부 API·플랫폼 공급망 리스크 관리  
- AI 인프라/HW 보안 : GPU, 서버, 네트워크 등 인프라 보호  

- 저품질·편향된 데이터 : 학습 데이터 품질 저하 및 편향으로 모델 성능 왜곡  
- 데이터 오염 : 악의적 데이터 삽입(데이터 포이즈닝)으로 모델 학습 결과 훼손  
- 학습 데이터 노출 : 민감정보 포함 데이터 유출로 개인정보·기밀 침해 발생  

- 수집 및 생성 : 표준화된 데이터 수집·생성 절차 수립, 데이터 검토 및 전처리 강화  
- 반입 및 정제 관리 : 데이터 격리 및 테스트 수행, 데이터 정제(필터링·이상치 제거) 적용  
- 출처 및 무결성 관리 : 신뢰할 수 있는 데이터 출처 확보, 데이터 검증 및 출처 추적 관리  
- 노출 및 이상 대응 : 앙상블 기법 적용으로 이상 영향 완화, 학습 데이터 난독화로 정보 노출 방지  

&lt;ML 모델 공급망과 관련 주요 위험요소&gt;  
- 모델 직렬화 공격 : Pickle 등 직렬화 포맷을 악용해 로드 시 악성코드 실행 및 모델 탈취  
- 모델 오염 : 학습·파인튜닝 단계에 악성 데이터 삽입으로 모델 동작 왜곡(백도어·포이즈닝)  
- 모델 기반 은닉형 악성코드 : 모델 내부(가중치·트리거)에 악성 로직 은닉, 특정 조건에서 공격 수행  
- 회피 공격 : 입력 변조(Adversarial)로 탐지 우회 및 잘못된 예측 유도  

&lt;ML 모델 공급망과 관련 주요 위험 완화 방안&gt;  
- 반입·형식 안전성 확보 : 안전한 파일 형식 사용, 모델 정제, 보안 도구 적용  
- 출처 및 구성요소 신뢰성 확보 : 신뢰 가능 출처 확보, 모델검증 및 출처추적, 재현가능 빌드 적용  
- 성능 및 복원력 검증 : 성능 테스트 수행, 앙상블 기법 적용, 입·출력 모니터링 및 필터링  
- 노출 및 이상 대응 : 모델 설명 가능성 및 투명성 확보, 적대적 학습 적용  

### [인공지능, 법/제도, ITPE모의고사 ] GSaaS(Ground Station as a Service)

**[정의]**  

- 위성 통신, 관제, 데이터 처리, 서비스 제공 기능을 통합하여 지상국 인프라, 안테나를 빌려서 사용하는 서비스  

**[핵심/키워드]**  

&lt;구성요소&gt;  
- 우주 영역 : 방송위성, 통신위성, 항법위성(GNSS) 기반 데이터 송수신 및 위치정보 제공  
- 안테나 영역 : 안테나, 위성모뎀, 안테나 제어시스템, 관리서버 기반 지상-위성 통신 I/F 제공  
- 지상국 영역 : 탑재체 DB, 데이터 수신·처리, 관측요청 접수, 분석·시각화, 미션운영 등 수행  
- 클라우드 영역 : 예약 및 스케줄링 시스템, DB 서버, API 서버 기반 서비스 제공 인프라  
- 위성 활용 서비스 영역 : 위성항법, 위성통신(스마트 선박·저궤도 이동통신·인터넷)등 서비스 제공  

&lt;서비스 유형&gt;  
- 서비스 유형 1 : 지상국 인프라 전체를 클라우드로 구현하여 GSaaS 형태로 제공  
- 서비스 유형 2 : 지상국은 직접 구축하고, 예약·스케줄링 등 운영 기능만 클라우드로 활용  
- 서비스 유형 3 : 지상국 구축 후 데이터 전달 경로(백홀/연계망)만 서비스로 활용  

### [인공지능, 법/제도, ITPE모의고사 ] 시각언어행동(VLA, Vision Language Action)

**[정의]**  

- Vision·Language·Action을 통합하여 보고-이해-행동을 수행하는 피지컬 AI 핵심 모델  

**[핵심/키워드]**  

&lt;진화흐름&gt;  
- LLM : 텍스트 이해·생성  
- VLM : 시각+언어 기반 객체 인식·설명  
- VLA : 물리적 상호작용·동작 제어까지 확장  

- Perception(인지) → VLM  
- Evaluation/Planning(판단·계획) → LLM  
- Action(행동) → VLA  

&lt;특징&gt;  
- 초기 융합 모델 : 시각·언어 표현 통합(CLIP 등)으로 의미 일관성 유지  
- 이중 시스템 아키텍처 : 고속 제어 시스템 + 고차원 추론(LLM) 분리·결합  
- 자체 수정 프레임워크 : 실패 감지 시 보조 경로로 복구·재계획 수행  
- 경량화·추론 최적화 : LoRA·양자화·병렬 디코딩으로 속도·효율 향상  

&lt;기술요소&gt;  
- 멀티모달 인코딩 : Vision·Language 통합 표현 학습  
- 행동 생성(Action Head) : 로봇 제어·모터 명령 생성  
- 정책 학습(Policy Learning) : 강화학습·모방학습 기반 행동 최적화  
- 계획·추론(Planning/CoT) : 작업 분해·순서 결정  
- 센서 융합(Sensor Fusion) : 카메라·LiDAR·IMU 등 환경 인지 통합  
- 폐루프 피드백(Closed-Loop) : 실행 결과 기반 지속 보정·재행동  
- 실시간 제어(Real-time Control) : 저지연 제어 루프  
- 자기 수정(Self-Correction) : 실패 감지 및 재계획  
- 시뮬레이션/Sim2Real : 가상 학습 → 현실 적용  
- 경량화·최적화 : LoRA·양자화·엣지 추론 최적화  

### [인공지능, 법/제도, ITPE모의고사 ] 도시 디지털 트윈

**[정의]**  

- 도시 환경을 디지털 공간에 구현하여 실시간 모니터링·분석·시뮬레이션으로 도시 관리·의사결정을 지원하는 지능형 시스템  

**[핵심/키워드]**  

&lt;구조&gt;  
- 현실세계 ↔ 가상세계(Digital Model) 실시간 연동  
- 데이터 기반 분석 → 예측·진단 → 제어·최적화  

&lt;3대 구성요소&gt;  
- 물리적 실체 : 건물·도로·시설 등 실제 도시 자산  
- 가상 실체 : 물리 자산을 디지털로 복제한 모델  
- 데이터 연결 : 센서 기반 양방향 연계(실시간 동기화)  

&lt;활용 방향&gt;  
- 도시 계획 및 공간 설계 : 3D 시뮬레이션, 건축물 밀도 관리, 시민참여 확대  
- 도시 인프라 통합 운영 : BIM·IoT 기반 통합운영, 마이크로그리드 관리, 통신망 과부하 조정  
- 통합 교통관리 : AI 기반 교통 예측, 고해상도 영상 분석  
- 도시환경 관리 : 대기질 센싱·모델링, 열섬 완화 및 녹지 최적화  
- 자원순환 관리 : RFID 기반 자재 추적, 하수처리 지능형 제어  

&lt;활성화 방안&gt;  
- 인프라 및 데이터 : 대규모 실시간 데이터 처리 체계 강화, 표준화 및 상호운용성 확보  
- 사용자 중심 : AI 기반 지능화 강화, 참여 플랫폼 고도화  
- 제도 및 정책 : 개인정보 보호 및 보안 체계 강화, 통합 거버넌스 구축  
- 투자 및 법제 : 지속 가능한 투자·재원 확보, 관련 법·제도 정비  
- 사회적 수용성 : 시민참여·소통 활성화, 적용지역 확대  

### [인공지능, 법/제도, ITPE모의고사 ] HOTL(Human On The Loop)

**[정의]**  

- 시스템이 자율적으로 수행하되, 인간이 전체 동작을 감시·모니터링하며 필요 시 개입하는 통제 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
- 인간은 실시간 직접 제어가 아닌 감독자 역할  
- 이상 상황 발생 시 개입 및 수정 가능  
- 자동화 효율성과 인간 통제의 균형 확보  

&lt;비교 포인트&gt;  
- HITL(Human In The Loop) : 인간이 의사결정에 직접 참여  
- HOTL(Human On The Loop) : 인간은 감시·통제 중심  
- HOOTL(Human Out Of The Loop) : 인간 개입 없음  

### [인공지능, 법/제도, ITPE모의고사 ] 미끼 효과(Decoy Effect)

**[정의]**  

- 열등한 옵션(미끼) 추가로 특정 선택지가 상대적으로 더 매력적으로 보이게 유도하는 현상  

* 선택지 간 비교 구조를 활용한 의사결정 유도  

**[핵심/키워드]**  

<참고 : 정박 효과(Anchoring Effect)>
- 최초 제시된 정보(가격·수치)가 기준점(anchor)이 되어 이후 판단에 영향을 미치는현상  
- 초기 정보에 의해 의사결정이 왜곡되는 현상  

&lt;핵심차이&gt;  
- 미끼 효과 : 선택지 간 비교 기반 유도  
- 정박 효과 : 초기 기준값 기반 판단 영향  

### [인공지능, 법/제도, ITPE모의고사 ] 데이터센터 냉각기술

**[정의]**  

- 서버, 스토리지, 네트워크 장비 등 IT 장비에서 발생하는 열을 효과적으로 제거하여 시스템의 안정적인 운영과 에너지 효율을 유지하기 위한 열 관리(Thermal Management) 기술  

**[핵심/키워드]**  

&lt;성능지표&gt;  
- 냉각·에너지 효율 평가(PUE·WUE·CUE·DCiE) + 에너지 재사용/총효율 지표(ERE·TUE)  

&lt;전통 데이터센터 냉각기술 유형&gt;  
- CRAC : 공기 순환 기반 냉각(항온항습기)으로 구조 단순·저밀도 환경 적합  
- CRAH : 냉각수(Chilled Water) 기반 공기 냉각으로 CRAC 대비 효율 향상  
- Containment : Cold/Hot aisle 분리로 냉기 집중 공급 및 열기 분리 배출  
- Raised Floor : 이중 바닥 구조로 하부 냉기 공급하여 공기 분배 효율 향상  
→  전통 냉각은 공기 기반, AI 데이터센터는 액체 기반(직접·침지)으로 고효율·고밀도 대응 진화  

&lt;인공지능 데이터센터 냉각기술 유형&gt;  
- 직접칩냉각(D2C) : Cold Plate 통해 칩에 직접 냉각수 순환, 고발열 GPU 대응 고효율 냉각  
- 액침냉각 : 서버를 절연유에 직접 담가 냉각, 공기냉각 제거 및 초고밀도 환경 최적  
- 후면 열교환 : 랙 후면 열교환기로 열 직접 제거, 기존 환경 적용 용이  
- 랙 인접 냉각(In-Row) : 랙 사이 냉각 장치 배치로 국부 고열 구간 집중 냉각  

### [인공지능, 법/제도, ITPE모의고사 ] 고영향 인공지능 판단 가이드라인

**[정의]**  

- 사업자가 고영향 인공지능 해당 여부 및 책무 유무를 스스로 판단할 수 있도록 기준과 예시를 제공하는 가이드라인  

**[핵심/키워드]**  

&lt;고영향 인공지능의 개념&gt;  
- 사람의 생명, 신체의 안전 및 기본권에 중대한 영향을 미치거나 위험을 초래할 우려가 있어, AI 기본법에서 지정한 특정 영역에서 활용되는 인공지능시스템  

&lt;법적근거&gt;  
- 인공지능기본법 제33조제3항 : 고영향 AI 기준·예시 가이드라인 수립  
- 시행령 제24조 : 고영향 AI 해당 여부 확인 절차 규정  

<적용대상(주체)>
- 개발사업자 : AI를 개발·제공  
- 이용사업자 : AI 기반 제품·서비스 제공  
- 이용자 : AI 서비스 직접 사용  
- 영향받는자 : AI로 안전·권리에 영향 받는 자  

<고영향 AI 판단 기준(2단계)>
1) 1단계(영역 조건) : 특정 중요 영역에서 활용되는 AI  
  - 적용 영역 : 에너지, 먹는물 관리, 보건의료·의료기기, 원자력, 범죄 수사·체포(생체인식 포함), 채용·대출 심사 등 개인 평가, 교통, 공공서비스, 교육  
2) 2단계(위험 조건) : 사람의 생명·신체·기본권에 중대한 영향 또는 위험 초래 가능성  
    → 1단계 + 2단계 충족 시 = 고영향 인공지능  

&lt;확인절차&gt;  
- 사업자 확인 요청서 제출  
- 과기정통부 검토  
- 필요 시 전문위원회 자문  
- 30일 이내 판단·회신(연장 가능)  
- 이의 시 10일 내 재확인 요청 가능  
- 재확인 시 전문가 자문 후 30일 내 재회신  

&lt; 주요 고려사항&gt;  
- 활용 영역 및 목적  
- 생명·안전·기본권 영향(영향·중대성·빈도)  
- 사업자의 사전 검토 결과  
- 전문가 자문 결과  
- 기타 필요 자료  

&lt;고영향 AI 사업자 의무&gt;  
1) 고지 의무 : 고영향 AI 사용 사실 사전 안내  
2) 안전·신뢰 확보 조치  
  - 위험관리 방안 수립·운영  
  - 결과 도출 기준 및 데이터 설명 가능성 확보  
  - 이용자 보호 방안 마련  
  - 인간 감독 체계 구축  
  - 안전성 검증 문서 작성·보관  
  - 기타 위원회 요구사항 반영  

&lt;책임구조&gt;  
- 개발사업자 중심 책임 부과  
- 이용사업자는 일부 책임 면제 가능(중대한 기능 변경 없을 경우)  
- 기능 변경 시 → 개발사업자 수준 책임 적용  

### [인공지능, 법/제도, ITPE모의고사 ] 우주시스템 모델

**[정의]**  

-  우주 자산(위성 등)과 이를 제어하는 지상 인프라, 그리고 이들 간의 데이터 연결 고리를 포함하는 인프라 체계  

**[핵심/키워드]**  

&lt;구성요소&gt;  
- 지상국(위성데이터센터·관제/운영센터·통신센터) + 위성망(지상국 안테나·위성망·통신단말) + 위성체(위성본체·탑재체)  

&lt;우주시스템 보안 필요성&gt;  
- 국가 안보 및 전략적 관점 : 비대칭 전력 위협 증가 대응 + 국가 핵심 인프라 마비 방지 필요  
- 경제 및 사회적 관점 : 핵심 서비스 연속성 보장 + New Space 시대 자산 보호 필요  
- 기술적 및 환경적 관점 : 우주 환경 특성상 물리적 수리 불가로 사전 보안 강화 필수  

&lt;보안대책&gt;  
- 지상국 보안 대책 : 접근통제(Zero Trust·MFA) + 악성코드 차단(EDR·패치·메일보안)  
                             + 네트워크 분리/관제(SIEM) + 내부자 통제 + 물리보안 강화  
- 위성망 보안 대책 : 통신 암호화(TLS/IPSec) + 인증 기반 통신(상호인증·PKI)  
                             + 재전송 공격 방지(Nonce·Timestamp) + 네트워크 침입탐지(IDS/IPS)  
- 위성체 보안 대책 : Secure Boot + 펌웨어 무결성 검증 + 명령어 인증/암호화  
                             + Anti-jamming/Anti-spoofing + 장애 대응(Fault Tolerance)  

### [인공지능, 법/제도, ITPE모의고사 ] CSAP(Cloud Security Assurance Program)

**[정의]**  

- 클라우드 서비스 제공자가 제공하는 서비스에 대해 정보보호 기준의 준수여부 확인을 인증기관이 평가·인증하여 이용자들이 안심하고 클라우드 서비스 이용할 수 있도록 지원하는 제도  

**[핵심/키워드]**  

&lt;법적근거&gt;  
- 클라우드컴퓨팅 발전 및 이용자 보호에 관한 법률(클라우드법) 제23조의2  

&lt;적용 대상&gt;  
- 공공기관 도입 클라우드 서비스(IaaS, SaaS 등)  

&lt;보안성 검토 개념&gt;  
- 공공기관 정보시스템 구축 시 보안 적정성을 사전 검토하는 절차  

&lt;보안성 검토 법적근거&gt;  
- 전자정부법 제56조  
- 국가정보원 「정보보안 기본지침」 등 하위 규정  

&lt;보안성 검토 적용 대상 및 관점&gt;  
- 공공기관 정보화사업 전반, 수요자(발주기관) 중심 검토  

&lt;CSAP와 보안성 검토 이중규제 발생 원인&gt;  
- 이중규제 구조 : CSAP 인증 받은 클라우드라도 → 공공기관 도입 시 보안성검토 재수행  
- 법적 충돌 지점 : 클라우드법 vs 전자정부법 체계 병행 적용  
- 문제 : 절차 중복, 도입 지연, 비용 증가  

&lt;이중규제 대응방안&gt;  
- 법제도 개선: 법제도 일원화 + 클라우드 규제 거버넌스 정립을 통한 규제 체계 통합  
- 공공시장 개편 : 클라우드 도입 절차 간소화 + 의무요건 완화를 통한 시장 활성화  
- 책임공유모델(SRM) : 책임범위 명확화 + SLA 기반 역할 분담 체계 확립  
- 관리체계 일원화 : 제도 통합 + 중복 보안항목 제거로 관리 효율화  
- 규제 통합 DB : 인증 공통 DB 구축 + 보안 프레임워크 통합으로 중복 심사 제거  
- 인증항목 상호연계 : API 기반 연동 + 인증항목 매핑으로 상호 인정 체계 구축  
- 표준아키텍처 개발 : 국가 보안프레임워크 표준화 + CSMP 기반 통제 체계 적용  
- 위험 기반 보안체계 : Risk 기반 통제 + 지속적 공격표면 관리로 동적 보안 구현  

### [인공지능, 법/제도, ITPE모의고사 ] 양자 컴퓨터 유형

**[정의]**  

- 큐비트 중첩·얽힘 기반 병렬 계산 수행하는 차세대 컴퓨팅  

**[핵심/키워드]**  

&lt;양자 컴퓨터 유형&gt;  
1) 게이트 기반(Universal QC)  
- 양자게이트로 회로 구성, 범용 계산 가능  
- IBM, Google 방식  

2) 어닐링 기반(Quantum Annealing)  
- 최적화 문제 특화(에너지 최소화)  
- D-Wave 방식  

3) 광자 기반(Photonic QC)  
- 빛(광자) 이용, 상온 동작 가능  

4) 이온트랩(Ion Trap)  
- 이온을 전자기장에 가두어 정밀 제어, 높은 정확도  

5) 초전도 기반(Superconducting)  
- 초전도 회로 사용, 현재 가장 상용화 근접  

### [인공지능, 법/제도, ITPE모의고사 ] ISO/IEC 5230, ISO/IEC 18974

**[정의]**  

: 라이센스 준수  
- 소프트웨어를 배포하는 기업이 올바른 오픈소스의 활용을 위해 준수해야 할 최소한의 핵심 요구사항을 정의한 오픈소스 컴플라이언스를 위한 국제 표준  

**[핵심/키워드]**  

: 보안 리스크 관리  
- 조직이 오픈소스 소프트웨어(OSS)의 보안 위험을 체계적으로 관리할 수 있도록 하는 요구사항 제공하는 표준  
  *ISO/IEC 5230(OpenChain 컴플라이언스 표준)과 연계하여 보안 관점 보완  

&lt;12가지 요구사항&gt; : 프업검컴커규  
1) 프로그램 설립  
- 보안 정책(Policy)  
- 역할 및 책임(Competence)  
- 보안 인식(Awareness)  
- 프로그램 범위(Program Scope)  

2) 관련 업무 정의 및 지원  
- 보안 실무 구현(Standard Practice Implementation)  
- 업무 정의 및 리소스 지원(Relevant Tasks & Resources)  

3) 오픈소스 콘텐츠 검토 및 승인  
- SBOM 관리(Software Bill of Materials)  
- 보안 검토 및 승인(Security Review & Approval)  
- 보안 보장(Security Assurance)  
- 규격 요구사항 준수(Adherence to the Guideline Requirements)  

4) 규격 요구사항 준수  
- 완전성(Completeness)  
- 지속성(Duration)  

5) 오픈소스 커뮤니티 참여 이해  
- 오픈소스 기여 이해(Contributions)  

6) 규격 요구사항 준수  
- 적합성 평가(Conformance)  
- 지속성(Duration)  

### [인공지능, 법/제도, ITPE모의고사 ] AP2

**[정의]**  

-  AI Agent 간 또는 Agent ↔ 서비스 간 자동 결제/정산을 수행하는 프로토콜(개념)  

**[핵심/키워드]**  

&lt;목적&gt;  
- AI Agent가 자율적으로 서비스 호출  
- API 사용  
- 작업 수행 대가 지급  
→ 경제 활동 자동화  

&lt;구성요소&gt;  
- Agent Identity : 에이전트 식별/인증  
- Payment Mechanism : 결제 방식(토큰, API billing 등)  
- Settlement : 정산 및 기록  
- Smart Contract(선택) : 자동 계약 기반 실행  

&lt;동작흐름&gt;  
- Agent 요청 → 서비스 수행 → 비용 산정 → 자동 결제 → 정산  

### [인공지능, 법/제도, ITPE모의고사 ] OSPO(Open Source Program Office)

**[정의]**  

- 조직 내 오픈소스 활용·기여·정책을 통합 관리하는 전담 조직(거버넌스 조직)  

**[핵심/키워드]**  

&lt;목적&gt;  
- 오픈소스 리스크 관리(라이선스·보안)  
- 조직 차원의 오픈소스 전략 및 활용 최적화  
- 개발 생산성과 협업 문화 강화  

&lt;역할&gt;  
- 오픈소스 정책 수립 및 가이드라인 제공  
- 라이선스 검토 및 컴플라이언스 관리  
- 오픈소스 사용 승인 및 관리 프로세스 운영  
- 내부/외부 기여 전략 수립 및 커뮤니티 참여  
- 보안 취약점 관리(SBOM, CVE 대응 등)  

&lt;구성요소&gt;  
- 정책/가이드라인(Policy)  
- 컴플라이언스 관리(License Compliance)  
- 보안 관리(Security Governance)  
- 커뮤니티/기여 관리(Community Engagement)  

&lt;특징&gt;  
- 기술 조직 + 법무 + 보안 협업 구조  
- DevOps/개발 프로세스와 연계  
- 기업 오픈소스 전략의 중심 조직  

&lt;기대효과&gt;  
- 라이선스 리스크 최소화  
- 오픈소스 활용 효율성 증가  
- 개발 속도 및 혁신성 향상  

### [인공지능, 법/제도, ITPE모의고사 ] 팹리스(Fabless)

**[정의]**  

- 반도체 설계 수행 + 제조는 파운드리에 위탁 후 칩 판매까지 수행하는 기업 모델  

**[핵심/키워드]**  

&lt;특징&gt;  
- 설계 중심(EDA, SoC, IP 활용)  
- 생산은 파운드리(TSMC 등)에 외주  
- 제품(칩) 판매로 수익 창출  

&lt;수익구조&gt;  
- 칩 판매(제품 매출)  

&lt;대표&gt;  
- NVIDIA, Qualcomm  

<참고 : 칩리스(Chipless) 개념>
- 반도체 설계(IP)만 제공하고 칩 생산·판매 없이 로열티로 수익을 얻는 기업 모델  

&lt;칩리스 특징&gt;  
- IP 설계 전문(아키텍처, 코어 설계)  
- 생산·제품 판매 없음  
- 라이선스 + 로열티 기반 수익  

&lt;칩리스 수익구조&gt;  
- IP 라이선스, 로열티  

&lt;칩리스 대표&gt;  
- ARM  

### [인공지능, 법/제도, ITPE모의고사 ] 약한 엔티티 타입(Weak Entity Type)

**[정의]**  

- 독자적인 식별자(Primary Key)를 가지지 못하고, 다른 엔티티(Owner)에 의존하여 식별되는 엔티티  

**[핵심/키워드]**  

&lt;특징&gt;  
- 자체 PK 없음 → 부분키(Partial Key)만 존재  
- 반드시 소유 엔티티(Strong Entity)와 관계 필요  
- 식별은 (소유자 PK + 부분키) 조합으로 구성  
- 존재 의존성(Existence Dependency) 가짐  

&lt;구성요소&gt;  
- 소유 엔티티(Owner Entity)  
- 부분키(Discriminator)  
- 식별 관계(Identifying Relationship)  

<표현(ERD)>
- 약한 엔티티 : 이중 사각형(Double Rectangle)  
- 식별 관계 : 이중 다이아몬드(Double Diamond)  

&lt;예시&gt;  
- 주문(Order) – 주문상세(Order Item)  
→ 주문상세는 주문 없이는 존재 불가  

### [인공지능, 법/제도, ITPE모의고사 ] 가트너2026

**[정의]**  

2023 : 복원력·지속가능성·관찰성·AI 보안  
2024 : AI 중심 개발 혁신과 산업별 플랫폼 진화  
2025 : 자율적 AI, 차세대 컴퓨팅, 인간-기계 융합  
2026 : AI 네이티브 전환·산업 심화·디지털 주권 강화  

&lt;가트너 기술전략&gt;  
- Gartner가 매년 선정하는 향후 3~5년 내 기업에 가장 큰 영향을 미칠 것으로 예상되는 핵심 기술 방향성  

**[핵심/키워드]**  

&lt;가트너 2026&gt;  
① The Architect(설계자)  
- AI 네이티브 개발 플랫폼 : SDLC 전반에 AI 내재화, 자동 코드 생성·테스트·배포 환경 구축  
- AI 슈퍼컴퓨팅 플랫폼 : 대규모 LLM·HPC 인프라, GPU/HBM 기반 고성능 처리  
- 기밀 컴퓨팅 : HW 기반 메모리 암호화, TEE·동형암호·PET 적용  

② The Synthesist(융합자)  
- 다중 에이전트 시스템(MAS) : 협업형 자율 AI, MCP/A2A 기반 오케스트레이션  
- 도메인 특화 언어모델(DSLMs) : 산업 특화 데이터 학습, RAG·MoE 활용 고정밀 모델  
- 물리적 AI(Physical AI) : VLA·Embodied AI 기반 자율 제어 시스템  

③ The Vanguard(선봉장)  
- 선제적 사이버 보안 : AI 기반 위협 예측·차단, CTEM·SIEM·SOAR 연계  
- 디지털 출처 검증 : C2PA·디지털 워터마킹 기반 콘텐츠 진위 검증  
- AI 보안 플랫폼 : AI TRiSM·제로트러스트 기반 AI 거버넌스 체계  
- 지오페이셔레이션(Geopatriation) : 데이터 주권·규제 대응 위한 Sovereign Cloud 전략  

### [인공지능, 법/제도, ITPE모의고사 ] F-분포

**[정의]**  

- 두 개의 독립적인 카이제곱 분포 변수의 비율로 정의되는 연속 확률분포  

*두집단의 산포를 비교하는데 이용  

<img src="data:image/png;base64,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cP8j8E8pGoXIdevWkc2COb3//vsLFizImDFjvXr1Jk+e8tFHdS1Fe+yxx8iWkSRbtGjR8uXLyZ8tWbJk9+7dCRIkSJ48ORiR/UJIpzVq1KhPn+CKFSrEiBEDO8TrlVdegZ+ReDt37lyaNGmYEjNmTBQcrl27Wrdu3Q7t22PEGcH/gw8+gAKSRcuePfvKlStr1679xhtvdOnaddWqH6l+4iMiCAgCgsAjhIAcVRAQBB5YBO6col29enXFDysaN2lMYbFt27YQoDJlygQHB38zZUq/vn2LFClC2szCQrGya9euefPmnThxYrly5UqWLAnrypQpE7PKhUwqAAAQAElEQVTgT/jAz2hTpUpF9+233ylUqJDldhiRJEmSRIkSJWfOnBMmTFi4cCH0jnpo9erVEydJkihRIh103RGoeObJk6dHjx6TJ0/u27fve++9R/COHTu+V6FC8+bN58+ff+nSJWKKCAKCgCAgCAgCgoAgcD8jcB2/ua2NXrhwYfyE8UOHDKXEWbhwYUjY0KFDKD5mzZYtilvfJNrVK1c2b97866+/pk+fnjQblUoyaiEhIU8++SRECof+/fv36dNn06ZNECnsWKxs3br1sy6ftW7dun379kQ+dOgQZVCI12efffapey1esvjY0ePTpk1r164dPq1atUIn02anU/FkiTp16gwaNBDWWKpUqf379g93r/B/9ZqdIu19iIBsSRAQBAQBQUAQeGQRuHOKFjVqlBQpUlBwBDu40W+//bZt2/YL58/T9eTylSuQsCZNmnTo0GHs2LHrflqntIodOzZVzkmTJo0YMYJ2xYoVZODixo0bJ04cb+LevXtJuTHlyy+/nDt3brJkyeB2M2fOHD16tDVC2lKlSgk7HDduHJYxY8asWrXq8uXLXgSU8+fP79y5C4J47Ngx8nBUSB9//PHo0aMzJCIICAKCgCAgCAgCjyYCD8qp75yixYwZi2rjyJEjKXTu2bOn2+efV61atdL778O6Dh48aFNi8KEcOXI8++yzlCmfeuqpAgUKkGbr3qN748aNGzZs2LJly27dutG+8MILFECrVKlC4dICR1V0+LDhX331FUSN+iZkbuDAgRQu8SeR1rt37wFfDBgyZMjYMWO+/vprHGhr164dL148d7oDJyOpVrduXWJS5SRLV7p06UGDBjVq1Agu6PpIIwgIAoKAICAICAKC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" alt="embedded_DR_78_Def_img_1.png" style="max-width: 100%; height: auto; margin: 16px 0;" />

### [인공지능, 법/제도, ITPE모의고사 ] 카이제곱 분포

**[정의]**  

- 정규분포를 따르는 독립 변수의 제곱합이 따르는 분포  

*정규화 된 오차의 크기를 측정  

<img src="data:image/png;base64,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" alt="embedded_DR_79_Def_img_1.png" style="max-width: 100%; height: auto; margin: 16px 0;" />

### [인공지능, 법/제도, ITPE모의고사 ] AI Inference(추론)

**[정의]**  

- 모델이 학습된 패턴으로 결과를 계산/예측하는 추론  

**[핵심/키워드]**  

&lt;특징&gt;  
- “기계적 추론” : 바로 답  
- 전처리, 전방향 전파, 역전파 학습  
- 확률기반, 패턴기반, 직관적 사고  

<참고 : AI Reasoning(리즈닝)>
- 단계적 사고를 통해 논리적으로 결론 도출하는 추론  
- “사고 기반 추론” : 생각해서 답  
- 논리기반, 분석적 사고, 단계적 사고  

&lt;관계성&gt;  
- Reasoning ⊂ Inference(확장 개념)  
  → Reasoning은 Inference 중 고급 형태(추론 강화)  
- Inference는 “결과 생성”, Reasoning은 “생각해서 결과 도출”하는 고도화된 추론 방식  

### [인공지능, 법/제도, ITPE모의고사 ] MSSP(Managed Security Service Provider)

**[정의]**  

- MSP :  IT 인프라 운영 관리 서비스  
- MSSP : 보안 관제·대응 중심 전문 서비스  

**[핵심/키워드]**  

&lt;관리대상&gt;  
- MSP : 서버·네트워크·클라우드·사용자 시스템  
- MSSP : 보안 장비·로그·위협 이벤트  

&lt;주요기능&gt;  
- MSP : 인프라 구축·운영·유지보수·장애 대응·성능 관리  
- MSSP : 보안 관제(SOC)·침해 탐지·대응·취약점 관리·위협 분석  

&lt;기술영역&gt;  
- MSP : ITSM·클라우드·네트워크·시스템  
- MSSP : SIEM·SOAR·EDR·Threat Intelligence  

### [인공지능, 법/제도, ITPE모의고사 ] 커크호프의 원리 (Kerckhoff’s Principle)

**[정의]**  

- 암호 시스템의 안전성은 알고리즘이 아니라‘ 키의 비밀성’에 의존해야 한다는 보안 원칙  

*PQC는 커크호프 원리를 유지한 채, 양자컴퓨팅 환경까지 확장한 차세대 암호 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
- 키를 제외한 시스템의 다른 모든 내용이 알려지더라도 암호체계가 안전해야한다는 원리  
- 공개 알고리즘 사용 가능, 키만 비밀로 관리, 알고리즘 검증성 확보, 보안의 투명성/신뢰성 확보  

&lt;적용예시&gt;  
- AES / RSA 등 국제표준, 자체 암호 알고리즘  

### [인공지능, 법/제도, ITPE모의고사 ] 모바일 신분증 KYC(Know Your Customer)

**[정의]**  

- 금융기관 등이 고객의 신원·거래 목적·자금 출처를 확인하여 불법행위를 예방하는 절차  

**[핵심/키워드]**  

&lt;목적&gt;  
- 자금세탁(AML), 테러자금조달 방지  
- 금융거래의 투명성·신뢰성 확보  

&lt;구성요소&gt;  
- 고객 식별(CIP) : 신분증, 개인정보 확인  
- 고객 검증(CDD) : 거래 목적, 직업, 자금 출처 확인  
- 강화 검증(EDD) : 고위험 고객 추가 심사  

&lt;절차&gt;  
- 고객 정보 수집 → 신원 검증 → 위험 등급 평가 → 지속적 모니터링  

&lt;적용기술&gt;  
- eKYC(비대면 인증), OCR, 생체인증(안면인식 등), AI 이상탐지, 전자서명  

*KYC(Know Your Customer, 고객신원확인)  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능(AI) 보안 안내서(2025.12)

**[정의]**  

- 외부의 사이버 위협으로부터 AI 모델과 서비스를 보호하기 위해 개발자, 서비스 제공자, 이용자가 준수해야 할 보안 요구사항 및 수칙을 담은 안내서  

**[핵심/키워드]**  

&lt;배경&gt;  
- 기존 AI 지침이 신뢰성 중심이거나 보안 관점의 구체성 부족  
- AI 보안(Security)에 특화된 실무 기준의 필요성 대두  

&lt;목적&gt;  
- AI 기술·서비스에 대한 정보보안 관점의 기준 마련  
- AI 시스템을 대내외 위협으로부터 보호  

&lt;초점&gt;  
- Security for AI 중심 접근  
- AI를 활용한 보안이 아닌, AI 시스템 자체 보호에 중점  

&lt;보호대상&gt;  
- AI 모델, 데이터, 배포·운영 환경, 인프라  

&lt;적용범위&gt;  
- AI 시스템 전 생애주기 적용(6단계로 변경, “파기“ 단계가 추가됨 )  
(계획 및 설계 → 데이터 수집 및 준비 → 모델개발 → 모델배포 → 모니터링 및 유지보수 → 파기)  

&lt;보안목표&gt;  
- 기밀성(Confidentiality) 확보, 무결성(Integrity) 유지  
- 가용성(Availability) 보장 + 책임 추적성(Accountability)  

&lt;적용대상자&gt;  
- AI 개발자 : 소프트웨어 개발자·엔지니어 또는 개발 조직(팀·회사)  
- AI 서비스 제공자 : 업으로서 AI 서비스 또는 AI 부수 서비스를 제공하는 자  
- AI 서비스 이용자 : AI 서비스 또는 AI 부수 서비스를 제공하지 않고 이용만 하는 사람  

&lt;적용 AI 유형&gt;  
- 예측형 AI(Pred AI)와 생성형 AI(Gen AI)에 맞게 구별하여 검증항목을 제시  

### [인공지능, 법/제도, ITPE모의고사 ] 국가데이터 통합 연계를 위한 데이터 카탈로그 표준 가이드v1.0

**[정의]**  

- 공공과 민간에 파편화된 데이터 플랫폼 간 상호운용성을 확보하고 범국가 차원의 데이터 통합·연계를 지원하는 지침  

**[핵심/키워드]**  

&lt;국가 데이터 통합플랫폼 개념&gt;  
- 범부처·분야에 걸쳐 데이터의 원활한 연계·활용을 지원하는 제도적, 기술적 기반을 제공하는 국가 최상위 플랫폼  

&lt;국가 데이터 통합플랫폼 주요기능&gt;  
- 소재정보의 통합관리, 유통·거래지원, 분야 간 데이터 활용 생태계 조성을 위한 지원시스템, 표준 및 참조모델 등을 포함  

&lt;국가 데이터 카탈로그&gt;  
- 범국가 차원의 데이터 탐색, 유통, 활용을 지원하기 위해, 국내 공공과 민간이 보유한 분야별 데이터 자산에 대한 설명과 주요 구성 내용을 체계적으로 정리한 목록  

&lt;국가 데이터 카탈로그 주요 구성&gt;  
- 데이터 카탈로그 제목, 데이터 카탈로그 설명, 데이터 셋, 데이터 서비스, 데이터 배포, 확장 속성  

### [인공지능, 법/제도, ITPE모의고사 ] AI-Ready 공공데이터 관리 체계 가이드라인

**[정의]**  

- AI가 별도의 추가 정제나 가공 없이 즉시 공공데이터를 학습·분석·추론에 활용할 수 있도록 지원하는 데이터 관리 기준  

**[핵심/키워드]**  

- AI 모델의 학습·추론·평가에 쉽게 활용되도록 품질, 표준 구조, API, 버전 관리, 고유식별자, 상세 메타데이터, 라이선스, 윤리적 위험관리 체계를 갖춘 공공데이터  

- 기계가독·상호운용성 : 오픈 포맷, 명시적 스키마, 표준 API·식별자 제공  
- 메타데이터·문서화 : 데이터 설명, 수집·가공 이력, 품질지표, 활용 조건 명시  
- 내용 품질·대표성 : 정확성·최신성·완결성 확보, 편향·불균형 최소화  
- 거버넌스 : 라이선스·개인정보·AI 윤리 준수, 변경 이력·책임 주체·대응 절차 관리  

- 기계 판독 기반 : 오픈 포맷, 기계 판독 가능 구조, 플랫형 데이터 구조  
- 표준화 기반 : 명확한 스키마, 표준 코드·형식, 결측치 표준 표기  
- 처리 효율 기반 : 컬럼형 저장 구조  

- 표준 접근 기반 : RESTful API와 URI 기반 자원 식별  
- 적시·선택 접근 기반 : 오픈 API와 부분 조회 지원  
- 대용량 활용 기반 : 높은 요청 한도, 스트리밍, 메타데이터 연계 제공  

- 기본 설명정보 : 데이터 관리 메타데이터, 고유식별자, 배포·접속 메타데이터  
- 활용 맥락정보 : 시간·공간·연계 메타데이터, 데이터 이용 메타데이터  
- 이력·신뢰정보 : 데이터 계보 메타데이터, 데이터 품질 메타데이터  
- 유형별 상세정보 : 데이터 유형별 메타데이터 및 문서화  

- 데이터 충분성 : 완전성, 충분성, 대표성·균형성  
- 데이터 정합성 : 일관성, 의미적 일관성, 정확성  
- 데이터 최신성 : 적시성, 개념·분포 변화 관리  
- 처리 안정성 : 유효성, 구조·형식 유효성, 값·범위 유효성  
- 중복 통제 : 유일성  

### [인공지능, 법/제도, ITPE모의고사 ] 중첩 학습

**[정의]**  

- 딥러닝 모델을 하나의 단일 최적화 문제로 보는 기존 관점탈피, 중첩, 다단계, 병렬적 최적화 문제 등 모델을 표현하는 새로운 패러다임  

**[핵심/키워드]**  

&lt;배경&gt;  
- 기존 딥러닝의 망각 문제(Catastrophic Forgetting)를 극복  
- 모델을 서로 중첩된 다수의 소규모 최적화 문제 계층 구조로 설계  

&lt;원리&gt;  
- 하나의 학습 과정 안에  또 다른 학습/최적화 과정이 포함됨  
  → Outer Optimization 안에 Inner Optimization이 들어가는 구조  
- 망각 문제 : 새로운 학습이 기존 지식을 파괴하는 현상  

&lt;학습 매커니즘에 적용 가능한 알고리즘&gt;  
1) 구조·표현 관점  
- 계층적 다중 최적화(Hierarchical Multi-level Optimization), 연관 기억 기반 표현(Associative Memory-based Representation)  

2) 메모리·시간 관점  
- 연속 메모리 구조(Continuum Memory System), 망각 완화 프레임(Catastrophic Forgetting Mitigation), 다중 시간척도 학습(Multi-timescale Learning)  

3) 학습 규칙·아키텍처 관점  
- 메타 최적화/딥 옵티마이저(Meta-Optimization/Deep Optimizers), 하이브리드 최적화·가소성 엔진(Hybrid Optimization & Plasticity), 자기 수정 아키텍처(Self-modifying Architecture)  

### [인공지능, 법/제도, ITPE모의고사 ] 온톨로지(Ontology)

**[정의]**  

- 특정 도메인의 개념·속성·관계·제약조건을 명시적으로 정의한 지식 표현 체계 (사람과 시스템이 동일한 의미로 데이터를 이해·공유·추론하도록 하는 의미 모델)  

**[핵심/키워드]**  

&lt;핵심 구성요소&gt;  
- 클래스(Class) : 사람, 제품, 조직 등 개념  
- 인스턴스(Instance) : 홍길동, 제품A 등 실제 개체  
- 속성(Property) : 이름, 가격, 소속 등 개체의 특성  
- 관계(Relation) : 포함, 소유, 상속, 연관 등 개념 간 연결  
- 공리·제약(Axiom) : 반드시 만족해야 하는 규칙과 조건  

&lt;표현구조&gt;  
- 개념 정의 → 계층화 → 속성·관계 설정 → 규칙·제약 적용 → 추론  

&lt;핵심기술&gt;  
- RDF : 주어–술어–목적어 기반 지식 표현  
- RDFS : 클래스·속성·계층 구조 정의  
- OWL : 복잡한 관계·제약·논리 표현  
- SPARQL : RDF·온톨로지 기반 질의  
- Reasoner : 정의된 규칙으로 새로운 지식 추론  

### [인공지능, 법/제도, ITPE모의고사 ] Silly Window Syndrome(SWS, 작은 윈도우 증후군)

**[정의]**  

- 슬라이딩 윈도우 환경에서 송신 또는 수신 측이 매우 작은 데이터 단위로 윈도우 크기를 조절하여, 패킷 분절과 ACK 교환이 과도하게 발생하고 전송 효율이 급격히 저하되는 현상  

**[핵심/키워드]**  

&lt;발생원인&gt;  
- 애플리케이션이 소량의 데이터를 반복적으로 생성  
- 수신 측이 현재 수신 가능한 데이터 크기를 아주 작게 송신 측에 전달  
- 송·수신 측의 비효율적인 윈도우 크기 조절  

&lt;문제특성&gt;  
- 작은 세그먼트 다량 전송  
- 헤더 오버헤드 증가  
- 네트워크 대역폭 낭비 및 처리 성능 저하  

&lt;대응기법&gt;  
- 송신 측 : Nagle 알고리즘(작은 데이터 묶음 전송)  
- 수신 측 : Clark 해결책(충분한 버퍼 확보 시까지 윈도우 광고 지연)  
- 송신 버퍼 최적화 : 일정 크기 이상 데이터 누적 후 전송  
- 애플리케이션 단에서 데이터 묶음 처리  

### [인공지능, 법/제도, ITPE모의고사 ] 인공지능 데이터센터 산업 진흥에 관한 특별법

**[정의]**  

- AI 데이터 센터를 단순 IT 시설이 아니라 국가 AI 경쟁력을 좌우하는 전략 인프라로 보고 구축·운영·입지·전력·인허가·재정지원까지 종합적으로 지원하기 위한 법령  

**[핵심/키워드]**  

&lt;주요내용&gt;  
- 산업 육성 : 사업자 신고제를 통해 진입 절차 간소화  
- 인허가 혁신 : 복합 인허가 일괄처리로 행정 효율성 강화  
- 규제 완화 : 타임아웃제를 통한 인허가 지연 방지  
- 지원 체계 : 전담기관 운영으로 사업 추진 지원  
- 특구 운영 : 규제특례 제도를 통한 실증·사업화 촉진  

&lt;핵심 지원정책&gt;  
- 전력 지원 : PPA 특례와 전력 계통 연계 지원  
- 인프라 지원 : 용수·도로·통신시설 구축 지원  
- 재정 지원 : 금융·보조금 지원  
- 입지 지원 : 특구 지정 및 사업 부지 확보  
- 인력 지원 : AI 데이터센터 전문인력 양성  

&lt;기대효과&gt;  
 - AI 인프라 확충, 비수도권 데이터센터 활성화, 민간 투자 촉진, AI 반도체·클라우드·전력 산업 연계  

&lt;고려사항&gt;  
- 전력 수급, 탄소중립, 지역 수용성, 보안, 재난 대응, 에너지 효율성  

