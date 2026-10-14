---
layout: post
title: "WritingDrill_Rounds_20"
date: 2026-10-14
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

## [인공지능] ANI (Artificial Narrow Intelligence, 제한적 인공지능)



**[정의]**

- 특정 기능이나 업무에 한정된 범위 내에서 최적의 성능을 보이는 AI

**[핵심/키워드]**

Vertical AI는 ANI의 한 유형

&lt; 필요성 &gt;  
→ 생산성 향상 및 자동화의 필수 요소  
- 기술적 측면 : 특정 작업 자동화로 효율성 향상  
- 경제적 측면 : 비용 절감, 생산성 향상, 산업 자동화  
- 사회적 측면 : 단순 반복 작업을 AI가 대체하여 인간의 부담 감소  
- 과학·연구 측면 : 대규모 데이터 분석 및 예측 가능  
- 위험성 및 윤리적 고려 : 위험성 낮음, 기존 법·윤리 체계 내 통제 가능

- 지능 수준 : 제한적, 특정 작업에 특화  
- 학습 및 적응 : 특정 데이터셋을 기반으로 학습, 도메인 제한적  
- 작업 범위 : 특정 도메인 서비스 (음성인식, 번역, 이미지 분석 등)  
- 실제 존재 여부 : 현재 상용화됨  
- 예시 모델 : Sora(영상 AI), Vivo, AlphaFold(단백질 구조 예측)  
- 위험성 : 낮음 (도메인 제한으로 안전)

## [인공지능] AI 인지한계이론 중 프레임 문제



**[정의]**

- AI가 환경변화 속에서 어떤 정보가 중요한지 판단하기 어려운 문제(상황·맥락 판단 문제)

**[핵심/키워드]**

&lt; 활용분야 &gt;  
지식표현, AI Planning(예: 자율주행 상황 판단, 로봇 경로 계획)

모폴프기상: AI 인지한계 이론  
1) 모라벡의 역설(Moravec's Paradox): 인간에게 쉬운 지각·운동능력은 AI에게 어렵고, 인간에게 어려운 논리·계산능력은 AI에게 쉬운 역설  
2) 폴라니의 역설(Polanyi's Paradox): '우리는 말할 수 있는 것보다 더 많이 안다'는 개념  
→ 인간의 암묵지(Tacit Knowledge)는 규칙·알고리즘으로 표현하기 어려움  
3) 프레임 문제(Frame Problem): AI가 환경변화 속에서 어떤 정보가 중요한지 판단하기 어려운 문제(상황·맥락 판단 문제)  
4) 기호접지 문제(Symbol Grounding Problem) : AI가 사용하는 기호(Symbol)가 실제 세계 의미와 연결되지 않는 문제  
5) 상식 추론 문제(Common Sense Reasoning) : 인간은 일상적 상식 기반 판단 가능하지만 AI는 이를 표현·학습하기 어려움

## [인공지능] 전문가 시스템



**[정의]**

- 전문가가 지닌 전문 지식과 경험, 노하우 등을 컴퓨터에 축적하여 전문가와 동일한 또는 그 이상의 문제 해결 능력을 가질수 있도록 만들어진 시스템  
- 특정 도메인에서 전문가의 지식을 규칙과 데이터로 변환하여 의사결정을 지원하는 AI시스템

**[핵심/키워드]**

&lt;특징&gt;  
- 특정 도메인 적용, 지식베이스,추론엔진, 정확성과 신뢰성, 규칙 기반(If-Then)추론→복잡한 문제 해결

* 추론방법  
1) 순방향 추론(Forward Chaining) : 주어진 사실(데이터)에서 출발하여 결론을 도출  
- 귀납적 추론 (Inductive Reasoning):원인 → 결과  
2) 역방향 추론 (Backward Chaining) : 목표(결론)를 설정한 후,이를 만족하는 원인을 역으로 추적  
- 연역적 추론 (Deductive Reasoning):결과 → 원인

## [인공지능] 협업필터링(Collaborative Filtering)



**[정의]**

- 대규모의 기존 사용자 행동 정보를 분석하여 해당 사용자와 비슷한 성향의 사용자들이 기존에 좋아했던 항목을 추천하는 알고리즘  
- 유사도 기반

**[핵심/키워드]**

&lt;유형&gt;  
- 메모리 기반(Memory Based) 협업필터링  
  ㄴ사용자 기반(User Based) : 비슷한 사용자 구매 상품 추천  
  ㄴ아이템 기반(Item Based) : 구매 아이템 연관 상품 추천

- 모델 기반(Model Based) 협업필터링  
  ㄴ행렬 분해 방식(특이값 분해), 머신러닝 기반(KNN), 딥러닝 기반 방식(오토인코더)

&lt;유사도 알고리즘&gt;  
- 유클리디안 기반  
- 코사인 기반  
- 자카드 계수 기반  
- 피어슨 상관 계수  
- 맨해튼 거리

&lt;문제점&gt;  
- 필터버블, 콜드 스타트, 계산 효율 저하, 롱테일 문제

&lt; 해결방안 &gt;  
- 다양성/랜덤성 반영, 추천 제어 옵션 제공, 콘텐츠 기반 추천과 결합 (Hybrid 방식)  
- 차원 축소(Matrix Factorization, SVD), 근사 최근접 탐색(ANN)

## [인공지능] 콘텐츠 기반 추천 (Content-Based Filtering)



**[정의]**

사용자가 선호하는 콘텐츠의 특성을 분석하여 유사한 콘텐츠를 추천하는 알고리즘

**[핵심/키워드]**

&lt; 문제점 &gt;  
- 필터버블, 한정된 데이터 문제

&lt; 해결방안 &gt;  
- 메타데이터 확장 (텍스트, 이미지, 태그 활용)  
- NLP/딥러닝 기반 특징 추출  
- 협업 필터링과 결합 (Hybrid 추천)

## [인공지능] 행렬 분해 (Matrix Factorization)의 Latent Factor 모델



**[정의]**

- 사용자와 아이템의 숨겨진 특징을 벡터 공간으로 변환하여 추천하는 방식  
 - 행렬 분해(Matrix Factorization) 기법을 사용하여 사용자-아이템 행렬을 저차원 잠재 요인(Latent Factor)으로 표현

**[핵심/키워드]**

&lt;특징&gt;  
- 희소 행렬(Sparse Matrix) 처리 가능  
- 차원 축소(Dimensionality Reduction)  
- 사용자-아이템 관계를 수치적으로 표현  
- 잠재 요인(Latent Factor)해석 가능

&lt;예측 과정&gt;  
1. 사용자-아이템 행렬 준비  
2. 행렬 분해 초기화 : 사용자 행렬(P)과 아이템 행렬(Q)을 랜덤값으로 초기화  
3. 최적화 과정 수행 : SVD,ALS,또는 SGD를 이용해 행렬을 최적화  
4. 손실 함수 최소화  
5. 사용자-아이템 예측

&lt;구성요소&gt;  
- 사용자-아이템 행렬 (User-Item Matrix)  
- 사용자 잠재 요인 행렬 (User Latent Matrix, P 행렬)  
- 아이템 잠재 요인 행렬 (Item Latent Matrix, Q 행렬)  
- 내적 연산 (Inner Product)

## [인공지능] 숙고형 에이전트



**[정의]**

- 목표 달성을 위해 계획을 수립하고 실행하는 에이전트  
- 외부 환경에서 기인한 현상을 바탕으로 수행하고자 하는 목표를 달성하기 위해 취할 수 있는 행동의 리스트를 만들어, 행동 수행 여부를 결정하는 Agent

**[핵심/키워드]**

* 동작구조 : 환감상(예추)행  
환경→감지기→환경 상태 인식→행동에 따른 결과 예상→추론(목적)→행동

* 기능 : 내부 모델을 사용하여 계획하고 의사결정  
* 예제 : 자율주행차, AI 비서, 전략 게임 AI  
* 장점 : 장기적인 목표 달성 가능, 복잡한 문제 해결  
* 단점 : 연산량이 많아 처리 속도가 느릴 수 있음

## [인공지능] 메타휴리스틱스 (Metaheuristics)



**[정의]**

- 최적화 문제를 해결하기 위한 상위 개념의 탐색 기법  
- 완전 탐색(Exhaustive Search) 대신 근사 최적해(Approximate Solution)를 찾는 알고리즘

&lt;주요 활용 분야&gt; : 경로 최적화, 네트워크 설계, 머신러닝 하이퍼파라미터 최적화, 생산 스케줄링

**[핵심/키워드]**

&lt;종류&gt;  
단일 해 기반 기법 (Single Solution-Based)  
- 시뮬레이티드 어닐링 (Simulated Annealing, SA)  
- 타부 서치 (Tabu Search, TS)  
- 확률적 탐색 (Randomized Search)  
집단 기반 기법 (Population-Based)  
- 유전자 알고리즘(Genetic Algorithm, GA)  
- 개미 군집 최적화(Ant Colony Optimization, ACO)  
- 입자 군집 최적화 (Particle Swarm Optimization, PSO)  
하이브리드 기법 (Hybrid Methods)  
- GRASP (Greedy Randomized Adaptive Search Procedure)  
- MA (Memetic Algorithm)

## [인공지능] AI 윤리원칙 (2026)



**[정의]**

- AI의 개발·활용 전 생애 주기에서 인간의 존엄과 권리를 보호하고, 공정·안전·신뢰할 수 있는 AI를 구현하기 위한  
가치 및 실천기준

(2020년)  
- 인공지능 관련 이해관계자들이 준수해야 할 보편적 사회 규범 및 관련 기술

**[핵심/키워드]**

2026 기준  
3대 가치 : 인사지  
- 인간의 존엄성  
- 사회의 공공선  
- 인류의 지속 가능성

* 7대 원칙 인프공책안신투  
인간 중심성 , 프라이버시 보호, 공정성 포용성 , 책임성, 안전성, 신뢰성, 투명성

2020 기준  
* 3대 기본원칙: 인사기  
- 인간 존엄성 원칙  
- 사회 공공선 원칙  
- 기술 합목적성 원칙  
* 10대 핵심요건: 인프다침 공연데책안투  
인권보장, 프라이버시 보호, 다양성 존중, 침해금지, 공공성, 연대성, 데이터 관리, 책임성, 안전성, 투명성

## [인공지능] XAI(eXplainable AI)



**[정의]**

- 사용자가 인공지능 시스템의 동작과 최종 결과를 이해하고 올바르게 해석하여 결과물이 생성되는 과정을 설명 가능하도록 해주는 기술  
- 알고리즘의 조작 가능성, 의사결정의 편향성, 머신러닝 AI에 대한 신뢰성 입증 한계

**[핵심/키워드]**

&lt; 모델 내 설명 &gt;  
라모통  
- 신경 회로망 노드에 설명 라벨링: 신경 회로망의 특정 노드는 인간이 이해할 수 있는 방식으로 똑같은 일을 반복, 라벨링 역추적을 통해 이해  
- 의사결정트리를 이용한 설명 모델 만들기: AI가 의사결정트리 로직을 학습하여 신경회로망이 하는일을 의사결정트리에 빗대어 설명  
- 통계적 방법을 이용하여 설명 모델 유추: 블랙박스를 통계적 방법을 활용하여 모델을 유추하는 방법(군집, 분류)

&lt; 모엘 외 설명 &gt;  
모델 기반 기법  
 - 화이트박스 모델 (White-box Model)  
 - 해석 가능한 신경망 (Interpretable Neural Networks)  
 - Surrogate Model (대리 모델)  
사후 설명 기법  
 - LIME(Local Interpretable Model-agnostic Explanations)  
 - SHAP (SHapley Additive exPlanations)  
 - Counterfactual Explanations  
신경망 시각화  
 - Saliency Map (살리언시 맵)  
 - Grad-CAM (Gradient-weighted Class Activation Mapping)  
 - Feature Attribution (특징 속성 분석)  
규칙 학습 기반  
 - Rule Extraction (규칙 추출)  
 - Decision Trees Approximation(의사결정 트리 근사화)  
설명 가능성 강화 기법  
 - Attention Mechanism (어텐션 메커니즘)  
 - Concept Bottleneck Models  
대화형 AI 설명 기법  
 - Explainable Chatbots (설명 가능한 챗봇)  
 - Interactive Visualization (대화형 시각화)

## [인공지능] 적대적 공격(Adversarial Attack)



**[정의]**

- 딥러닝의 심층신경망을 이용한 모델에 적대적 교란을 적용하여 오분류를 유발하고 신뢰도 감소를 야기하는 머신러닝 공격기법

- AI/ML 모델의 입력 데이터에 사람이 인지하기 어려운 미세한 교란(Perturbation)을 의도적으로 추가하여 모델이 오 분류/오 판단하도록 유도하는 공격

**[핵심/키워드]**

* 공격유형: 포모도회  
- 포이즈닝 공격: 잘못된 학습데이터 주입  
- 모델 추출 공격: 반복적인 질의에 의한 답으로 인공지능의 동작을 모사  
- 도치 공격: 반복적 질의로 학습에 사용된 데이터 추출  
- 회피 공격: 분류 데이터 변조하여 오인식 유도

* 대응방안 : 예탐차은  
- 사용자 인증(행위, 생체신호 기반, 환경 기반)  
- CAPTCHA, DefenseGan  
- 이상 거래 탐지  
- 신용 예측(오버샘플링, 기존 데이터 합성)

## [인공지능] 인공지능 시스템의 취약점



**[정의]**

- 인공지능 모델과 데이터, 운영환경에서 발생할 수 있는 보안·신뢰성·윤리적 약점

**[핵심/키워드]**

데모운인신(데이터/모델/운영/인프라/신뢰성)

1) 데이터 취약점: 데이터 편향(Bias), 데이터 중독(Data Poisoning), 민감정보 노출  
2) 모델 취약점: 적대적 공격(Adversarial Attack), 과적합(Overfitting), 모델 추론 공격(Model Inference)  
3) 운영 취약점: 프롬프트 주입(Prompt Injection), API·인증 취약점, 가용성 위협(DoS)  
4) 인프라·연계 : 서플라이체인 공격. 하드웨어·엣지 기기 취약, 서드파티 의존 리스크  
5) 신뢰성·윤리 : 설명 불가성 (Opacity), 공정성 침해, 오남용·허위정보 생성, 규제·준수 리스크

&lt;대응방안&gt;  
- 데이터: 샘플링 보정·증강, 출처 검증, 익명화·탈식별화  
- 모델: 적대적 훈련, 교차검증, XAI 기법(SHAP, LIME) 도입  
- 운영: 입력 검증·정제, OAuth/mTLS 인증, DDoS 방어  
- 인프라: 공급자 검증, 서명된 아티팩트, SBOM 유지  
- 신뢰성: 공정성 지표 설정·모니터링, 개인정보 영향평가

## [인공지능] 연합학습



**[정의]**

- 중앙 서버에 데이터를 모으지 않고, 분산된 여러 장치(클라이언트)에서 개별적으로 모델을 학습한 후, 학습된 가중치만 서버에 공유하는 분산 학습 기법

- 데이터 프라이버시를 보호하면서 각 사용자 또는 장치의 로컬 데이터를 활용하여 AI모델을 학습하는 방식  
- 주로 모바일 디바이스,의료 데이터 분석,금융 서비스,IoT기기 등에서 활용

**[핵심/키워드]**

* 연합학습 주요 알고리즘  
1) FedSGD(연합통계학습)  
- 각 단말은 자신이 한번 학습한 하라미터 값을 중앙에 전달  
- 중앙 취합 값의 평균으로 글로벌 파라미터 업데이트  
- 결과를 다시 모든 단말로 전달  
- 파라미터의 수렴 조건이 만족할 때까지 과정 반복  
2) FedAVG(연합평균학습)  
- 각 단말이 일정 횟수 k만큼 반복 학습 수행 후 파라미터 값을 서버로 전달  
- 각 단말에서 batch size 크기로 나눠 학습하여 mini batch 효과를 주어 글로벌 파라미터가 수렴에 이르는 시간을 단축

3) FedProx (Federated Proximal)  
4) FedOpt (Federated Optimization)  
5) FedMA (Federated Matched Averaging)  
6) FedBN (Federated Batch Normalization)  
7) FedGKT (Federated Gradient Knowledge Transfer)  
8) FedReID (Federated Learning for Person Re-identification)

## [인공지능] 자기지도학습(Self-Supervised Learning)



**[정의]**

- 별도의 사람이 만든 Label 없이 데이터 자체에서 학습 신호를 생성하여 학습하는 방식  
- 라벨이 없는 데이터(Unlabeled Data) 에서 자신이 스스로 라벨을 만들어 학습하는 방식

**[핵심/키워드]**

&lt;핵심아이디어&gt;  
- 모델이 라벨 없이 스스로 학습 과제 생성,대조학습

&lt;라벨생성방식&gt;  
- 모델이 데이터 관계로부터 스스로 라벨 생성  
- 라벨 없이 표현(Representation) 학습하는 데 초점

&lt;절차&gt;  
1. 사전 과제 정의(Pretext Task)  
2. 자기 생성 라벨 구성(Synthetic Label)  
3. 모델 입력 및 학습  
4. 표현학습(Representation)  
5. 다운스트림 활용

&lt;대표알고리즘&gt;  
- Context Prediction : BERT,GPT계열  
- Contrastive Learning(대조 학습) : SimCLR, MoCo, BYOL, CLIP  
- Generative(생성 기반) : VAE, AE, MAE  
- Clustering/Prototype Learning : SwAV, DeepCluster  
- Predictive Coding(예측 부호화) : CPC  
- Transformation Prediction : RotNet

## [인공지능] 퓨샷러닝(Few Shot Learning )



**[정의]**

- 메타러닝 기반 머신러닝  
- 적은 양의 데이터로 모델을 학습하여 테스트 데이터에서 유의미한 성능을 얻고자 하는 작업  
- 배경: 높은 데이터 수집비용 및 라벨링 비용, 충분한 데이터 확보 어려움

**[핵심/키워드]**

* 구성요소  
- Support Set(학습데이터): 이미지와 레이블로 구성된 적은 양의 학습 데이터 셋  
- Query Set(평가데이터): Support Set으로만 모델을 학습한 후, 모델의 성능을 평가할 데이터 셋  
- way: 데이터 클래스의 갯수  
- shot: 데이터의 갯수  
- 메타러닝 (Meta Learning)

* 퓨샷러닝 동작과정  
[ 학습 ]  
- Train-test data split: 훈련/테스트 데이터 분리  
- Task Sampling: 메타훈련데이터를 각 task 데이터로 분리(task=episode)  
- Support Query data set split: task별 데이터를 다시 support set, query set으로 샘플링  
- Task Training : 각 task 진행하여 모델생성  
[ 검증 ]  
- Meta test 평가: 생성된 모델에 meta-test의 support set으로 새로운 클래스 학습시키고 최종적으로 meta-test query set을 분류

## [인공지능] 치명적 망각(Catastrophic Forgetting)



**[정의]**

- AI 모델이 새로운 데이터·Task를 학습하는 과정에서 기존에 학습한 지식이나 성능을 급격히 잃는 현상  
- 신경망이 새로운 Task·데이터를 학습하면서 기존에 학습한 지식의 파라미터가 크게 변경되어 이전 지식의 성능이 급격히 저하되는 현상

**[핵심/키워드]**

* 문제점  
① 기존 지식 훼손 : 신규 학습에 따른 기존 가중치 변경 및 지식 손실  
② 과거 작업 성능 저하 : 기존 표현과 결정겨례 변경으로 과거 Task 성능 급락  
③ 지식 간 간섭 발생 : 신규 · 기존 Task가 동일 파라미터 갱신하여 가중치 충돌  
④ 안정성(Stability)-가소성(Plasticity) 딜레마 : 기존 지식 보존과 신규 지식 습득 간 상충

* 해결방안  
- 재현 기반: 과거 데이터를 신규 데이터와 함께 재학습  
- 정규화 기반: 기존 지식에 중요한 파라미터의 변경 제한  
- 파라미터 분리: Task별 파라미터·마스크·Adapter를 분리  
- 동적 구조 확장: 신규 지식 수용을 위해 모델 구조를 점진적으로 확장  
- 지식 증류: 이전 모델의 출력과 표현을 신규 모델에 전달  
- 중첩학습: 다중 시간척도와 갱신 주기로 단기 적응과 장기 기억 분리

## [인공지능] 지속학습(Continual Learning)



**[정의]**

- 모델이 한번 학습된 후 멈추는 것이 아니라, 시간에 따라 변화하는 새로운 데이터나 작업을 순차적으로 학습하면서도 이전에 익힌 지식을 잃지 않고 유지하는 머신러닝 패러다임

- 목적: 치명적 망각의 최소화 , 신규 지식 습득과 기존지식 보존의 균형

**[핵심/키워드]**

* 핵심 원리  
- Stability(안정성)-Plasticity(가소성) Balance 확보  
- Stability: 기존 지식 안정적 유지  
- Plasticity: 신규 정보에 유연하게 적응

* 접근 방식  
- Regularization: 중요 파라미터 변화 제한(EWC,LwF 등)  
- Replay: 과거 데이터·특징 재학습  
- Architecture Expansion: 신규 Task에 맞춰 모델 구조 확장  
- Dynamic/Hybrid Approach: 여러 방식 결합

* 지속학습 절차  
: 초기 학습 → 신규 데이터·작업 유입 → 순차 학습 → 지식 유지 → 지식 적응 → 반복 학습

* 학습형태  
- Task-Incremental Learning(새로운 Task를 순차적으로 추가 학습)  
- Class-Incremental Learning(새로운 Class를 지속적으로 추가 학습)  
- Domain-Incremental Learning(동일 Task에서 새로운 환경

* 지속학습은 상위 목표·문제 영역

## [인공지능] 중첩학습(NL, Nested Learning)



**[정의]**

- 기존 딥러닝 모델의 치명적 망각 문제(Catastrophic Forgetting)를 극복하기 위해 계층적/연관 기억, CMS, HOPE 아키텍처 기반 지속 학습을 제공하는 인공지능 학습 패러다임  
- 모델을 서로 중첩된 다수의 소규모 최적화 문제 계층 구조로 설계하여 각 계층이 서로 다른 학습 속도로 지속 학습을  
수행하는 인공지능 패러다임 (지속학습의 하위 개념)

**[핵심/키워드]**

&lt;특징&gt;  
- 기존 학습 모델의 망각 문제 극복  
- 장/단기 기억별 다른 속도 처리  
- 장기 기억 데이터 처리 개선

* 메모리 구조  
- CMS(Continuum Memory System) : 서로 다른 업데이트 주기 가진 메모리 레벨 연속적 구성

* 실증 아키텍처  
- HOPE Architecture : Self-Modifying Learning Module + CMS 결합

* 핵심원리  
- Uniform and Reusable Structure : 공통 학습, 최적화 구조를 여러 레벨에서 반복 활용  
- Multi-time-scale Update : Learning Level별 Update Frequency 차등화

* 학습계층  
- Nested Learning Level(중첩 학습 레벨)  
: Fast(빠른 업데이트, 새로운 정보) → Intermediate(중간 업데이트, 반복 경험) → Slow(느린 업데이트, 핵심 지식) 형태의 계층적 학습

* 중첩학습 절차  
: Nested Learning Level 구성 → CMS 기억 계층 구성 → 다중 속도 학습 수행 → Nested Optimization 수행 → CMS기반 기억 통합

## [인공지능] K-Means



**[정의]**

- 데이터의 유사성을 기반으로 최적의 중심점을 찾아 K개의 그룹으로 분류하는 방법

- 데이터(Training Set)를 기준점(Code-vector)을 중심으로 유클리디안 거리가 최소가 되도록 K개의 묶음으로 구분하는 클러스터링 알고리즘

**[핵심/키워드]**

1) 군집 수 K를 정의하여 임의 위치 지정(initial Centroids)  
2) 모든 데이터들의 거리 계산 후 가장 가까운 중심점 기준으로 군집화  
3) 각 군집마다 계산하여 새로운 중심 계산  
4) step 2~3을 반복, 클러스터가 변경되지 않으면 학습 완료

## [인공지능] 가우시안 혼합 모델(Gaussian Mixture Model ,GMM)



**[정의]**

- 데이터가 여러 개의 정규분포(가우시안 분포)로 생성되었다고 가정하는 확률론적 생성 모델

**[핵심/키워드]**

&lt;특징&gt;  
- 분포 기반 군집화 알고리즘. EM알고리즘 사용. 군집화 및 밀도 추정에 사용  
- 각 데이터 포인트가 어느 정규분포(클러스터)에 속할 확률(소프트 클러스터링) 제공

&lt; 핵심요소 &gt;  
- 혼합 계수 (πₖ), 평균 벡터 (μₖ), 공분산 행렬 (Σₖ), 최적화 모수 집합 (θ)  
- 모수 최적화 과정: EM 알고리즘

 - 초기 데이터 분포 분석 -→ K개의 새로운 가우시안 분포로 군집화 -→  
EM 알고리즘을 이용해 최적의 분포(군집) -→ K개의 새로운 가우시안 분포로  
데이터 모델링

## [인공지능] 군집모델 평가지표



**[정의]**

군집화 결과의 군집 내 응집도, 군집 간 분리도 및 실제 정답과의 일치도를 측정하여 군집모델의 품질과 성능을 평가하는 지표

**[핵심/키워드]**

* 정답이 있는 군집 모델 평가지표(지도학습평가)  
- 일치행렬: C,T 두행렬의 모든 원소에 대해 값이 같으면 1, 다르면 0으로 계산한 행렬  
- 랜드지수(RI: Rand Index): 두개의 군집화 결과 간의 데이터 샘플 쌍이 일치하는 정도  
- 조정랜드지수(ARI): 기대값과 분산 재조정  
- 상호정보량(MI): 두 이산확률변수 T, C 간 상호 의존성 측정

* 정답이 없는 군집 모델 평가지표(비지도)  
- 던지수(DI): 군집간, 군집 내 데이터간 거리측정  
- 실루엣 계수(S): 군집내 응집도와 군집 간 분리도 이용한 지표  
- 팔꿈치 알고리즘(Elbow Method): Elbow 모습을 나타내는 부분을 K값으로 지정하는 방법

## [인공지능] 차원의 저주



**[정의]**

- 데이터 품귀현상  
- 기존 데이터를 포함하는 차원이 증가할수록 데이터의 부족으로 인해 overfitting등의 문제로 모델의 성능이 떨어지는 현상

**[핵심/키워드]**

* 차원의 저주 특징  
- 기하급수: N제곱수 기준으로 비례  
- Sparsing: 동일 개수의 데이터 밀도는 차원증가에 따라 희박해짐  
- 고차원 해당: 수십정도의 저차원에서는 발생하지 않음

&lt;발생원인&gt;  
- 차원이 증가하면 데이터가 희소(Sparse)해지고 거리 계산이 비효율적이 됨  
- 고차원 공간에서는 데이터 간의 유사성을 유지하기 어려움  
- 학습 데이터가 부족하면 과적합(Overfitting) 가능성이 증가

&lt;해결 방법&gt;  
차원 축소 (Dimensionality Reduction)  
 - 주성분 분석 (PCA)  
 - 선형판별분석 (LDA)  
 - 비선형 차원 축소 (t-SNE, UMAP)  
머신러닝 모델 최적화 (Feature Selection & Engineering)  
 - 특징 선택 (Feature Selection)  
 - 특징 추출 (Feature Extraction)  
데이터 처리 관점 (Sampling & Regularization)  
 - 더 많은 데이터 확보 (Increase Data Volume)  
 - 정규화 (Normalization) 및 스케일링 (Scaling)  
 - 규제항 (Regularization, Dropout, L1/L2)  
알고리즘 선택 관점 (Curse-Aware Models)  
 - 차원 증가에 덜 민감한 모델 선택  
 - 국소 근접 학습 (Locality-Based Learning)  
정보이론적 접근 (Entropy & Mutual Information)  
 - 정보 이론을 활용한 차원 축소  
 - 상호 정보량 (Mutual Information)  
비지도 학습 기반 사전 가중치 학습 (Pretraining)  
 - RBM (Restricted Boltzmann Machine)  
 - Autoencoder (AE)

## [인공지능] 차원 축소 알고리즘



**[정의]**

- 고차원 데이터를 저차원으로 변환하여 데이터의 중요한 정보를 유지하면서 연산 비용을 줄이는 기법

**[핵심/키워드]**

&lt; 목적 &gt;  
- 데이터 시각화, 노이즈 제거, 모델 성능 향상, 차원의 저주 해결

&lt;차원축소 알고리즘&gt;  
선형 차원 축소 (Linear Dimensionality Reduction)  
- PCA (Principal Component Analysis, 주성분 분석)  
- LDA (Linear Discriminant Analysis, 선형 판별 분석)  
- FA (Factor Analysis, 요인 분석)

비선형 차원 축소 (Non-Linear Dimensionality Reduction)  
- t-SNE (t-Distributed Stochastic Neighbor Embedding)  
- UMAP (Uniform Manifold Approximation and Projection)  
- Isomap (Isometric Mapping)  
- LLE (Locally Linear Embedding, 국소적 선형 임베딩)

신경망 기반 차원 축소 (Deep Learning-Based Dimensionality Reduction)  
 - Autoencoder  
 - Variational Autoencoder (VAE)  
 - RBM (Restricted Boltzmann Machine)

행렬 분해 기반 차원 축소 (Matrix Factorization)  
 - SVD (Singular Value Decomposition, 특이값 분해)  
 - NMF (Non-Negative Matrix Factorization, 비음수 행렬 분해)  
 - MDS (Multidimensional Scaling, 다차원 척도법)

## [인공지능] Auto Encoder(=Vanillar AutoEncoder)



**[정의]**

- 입력 데이터를 압축(Encoding)하고 다시 복원(Decoding)하는 신경망 구조로, 데이터의 중요한 특징을 학습하는 비지도 학습 모델

- 기울기 소멸문제(베니싱 그래디언트) 등의 문제를 해결하기 위해 입력층과 출력층의 노드수를 같이 하여 가중치를 최적화 시키는 기법

**[핵심/키워드]**

- 은닉층의 노드 수가 입력층보다 작음으로 입력층 정보가 손실되지 않게 정보 압축 가능

학습과정 : 인코딩 → 잠재 변수 → 디코딩 → 손실 계산 → 최적화

인코더(Encoder) : 입력 → 인코더 → 잠재 변수 변환  
 - 입력 x 를 잠재 표현 y 로 변환하는 과정

디코더(Decoder) : 잠재 변수 → 디코더 → 출력 재구성  
 - 잠재 표현 y를 다시 원본 차원 z로 복원하는 과정

&lt;네트워크 구조&gt;  
입력층 (Input Layer)  
인코더 (Encoder)  
잠재 공간(Latent Space, Bottleneck Layer)  
디코더 (Decoder)  
출력층 (Out Layer)

## [인공지능] 연관규칙



**[정의]**

- 특정 사건(상품 구매)들이 동시에 발생하는 빈도로 상호간의 연관성을 표현하는 규칙  
- 대량의 데이터에서 특정 항목이 발생했을 때, 다른 항목도 함께 발생할 가능성 및 항목 간의 관계를 발견하는 기법  
- 예 : 장바구니 분석→제품 구매 패턴 분석

&lt;특징&gt;  
- 연관성 측정 지표(지지도,신뢰도,향상도)를 통해 규칙 평가  
- 구매 데이터,웹 로그,의료 데이터 등 다양한 분야에서 사용  
- 빈발 항목 집합을 기반으로 연관 규칙 도출  
- 높은 계산 비용 → 최적화된 알고리즘 필요 (예:Apriori,FP-Growth,Eclat등)

* 연관규칙 발견 과정  
- 후보데이터군(최소한의 지지도, DB검색) → 대용량 데이터군(최소한의 신뢰성) → 연관규칙 (Apriori방법)

<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAgQAAAHKCAIAAADzasSYAAAQAElEQVR4AezdBYBV1dYA4HtmCMUAQRD12d2t6FMQscBCVAxs7O5uxQ7sfoKBLXZid/1Pn92FAQICIsrk/927Zw6He2eGCwwD4rlvuVl7nbX32WftvVcqr6Q6/aUSSCWQSiCVwD9eAiWZTOauu+467fTTz09/jSGB884778wzz9Q2xmTpHDNeAv369TvrrLNm/DrSFaQSmA4SOPnkk59//nlWAGSNwWOPPVZZXv6vBRfskP6mTQILLLDA7LPN9sTjj7dp3Xr+jh2nbbJ09IyXwEILLTRu3LghQ4a4HfPNN9+MX9DUrSAdlUqgLgksssgi33333SuvvMISgKwx6Nix4zbbbNO7d+8dtt8+hWmRQO8ddiDJVVddddttt93BL5Xn31wCO/buvflmm62x+urp7ZiWe5GOnTklsPNOO226ySZt2rRhCUDWGFRVVY0fP/6P9NcYEiDJ8vJybWNMls4x4yXw559/2tAZv450BakEGlsCot6//vpLrYQlAFlj4I8U/p4SSFedSiCVQCqBxpFAagwaR47pLKkEUgmkEvhbS2A6GoOSkpLmiV9paenUSapZs2ZRFBU5Nooi/EUyp2zFSMDGkWoxnIU8BtoObeGjlJJKICmBKTonThT+5PBZGW+qb5texsBuVVZWjh07VloKQMrKyhDzvku6yqbONumvZcuWDEnMKaulqhF3G0ZMiD/Jg2L6uev5zTHHHN6FJzkkxWMJEA68cOMQk0CArVq1IswkEY5uO7TwFFIJOAmzzz5769atC0WRd05atGiBs9Xss8egG06jsebBD0mhESUwXYyBPbPfgwYN6tylS5cNNwSdO3c+++yzKWWPkqvndY4cOfKLL7746uuvs/BV9vfjjz8yJBQQq/DTzz9v26vXa6+9FhQNIq0+z6Q/1XARiPOBB2evXr1+/vlnhym8yEtfeeWVSy+99PJJf1dcccWNN9741FNPqRBaRmBO26QEyPDXX3/daeedCbBVq1bJR3k4IT/22GN33X03Sdqj8BTxhx9+2Hbbbd98882Ghwf+tJ3lJeAYPPTQQyeccIILHqsC52To0KGueXxOnKIRI0b874MP/u+//62B99775JNPVPKdLtf85Vde6bXddsOGDXNEZ3mhNdkHThdjYC/FAautttrBBx20f+538CGHdNt4YyrbaaC148+bc845+19++YZdu24afptttvnmm2+8ySYPPPigLRc0iCreeecduw437V8TJhx//PE777LLbrvvnoXddtt1112PPuaYr7/+muXAg/Ptd95RdY+PGvqrr7567XXXJeGWAQPAEUceuUPv3u+//753xUtKkVgCc8011yuvvvrcc8/98ssv/LLkxsU8EPfTnWRcgS3QRQT26/dx4955993hw4ejo6QwqQT+cT2n6OFHHnH1nA3nBLinzoYL65qHc+IRpb/X3ntv1LXr1ttss9XWW2+9zTZbbLHFv9dff/DgwfN17DjX3HOPHj367bff/mP8eMP/cUKcbh/cyMbA7trak08+WTRw2umnP0uR5IBrOXDgwB122GHAwIG0M7bwRbzyXXbe+frrrrvqyiuvvOKKgQMG9O3bl0L/4/ff+QumomUwQ2giSKa6evSYMSNHjuQ4gFG//fbLsGHXXHONUxLMDE7nA4T5tTJUhx9++NtvvfXG66+/+cYb7/33v599+unjjz3WbaONPN1ll13WWGON8ePHw1OIJUDa7PR3330nokJ0e4UIKOi6eUDaLjO9v9RSS5F/zAPxCHOSqJvCP1MC7u+ECRPE/SuvvLKzJPdLFQA3nZHwNJwTLavw3nvv7bbbbk89+eTgBx546MEH773nHkNc87vvuuvOO+9kCXiWpSWNrL7+mfsSf3XjS5MKWG755ddbd91VV1lluWWXFR+ss/bac881lzTC40888fnnn9vF+PUCiBVXXFFiZ+utt95h++2FBW+9/fa8887LHeCNjhkzRmQQM1dUVDg3V1x++YODBz9w//3gkYcfvu7aa50nUWfMVojwNfj+bdu2bdeunXN2wQUXCEBuv+OO66677rZbb5VzKhzyT6a4lrJ8hH/AgQfar3POOefjjz/efY89Ro0a1bZtW8LME44N/fnnnwVnE/76y9i8p2k3lQAJUAvuoIP01ltvSR7y5Nzlo44+ukePHht167b/gQdiYAZwBoAvv/zynTp1Wjv3W2+99ebr0OG1118/8iiDjr7nnnucw+BqBP60nXYJNLIxsKMM/gH773/11VdfdfXV/Mode/cuKS394IMPll12We7/uf36YYjXTXdwFjjvykEU+tFHH/3CCy/ceMMNr736qjOw1tpr79qnjzmpmzAEzn6IIrUGOg0ffvghZIUVV2QqAk9e6wg6dkzLPffe23vHHddeZx3GgOYy1euvv37LLbd88OGHZrOSvIHT0v37juWjqcG8++673bt3f/bZZ/v37y/Ou/XWW8mqc5cu9957r1vKVJB8+EZiJOFnhgwR5A0ZMkTgJbkUHqVtKoFYAjw2R+X8Cy5wfn4YOvTY445zhJZeeunFl1himaWXXmjBBXFi0AZwH91rIXsMUgJ9+vT58osvPv/ss37nnEMJVFZVBea0bRQJNLIxsIU2W3rh8ccfP/bYY2nedTp1Ujr+8KOPRHmzzT67zKA4MWkPfAYFJB10xllnXXHllQ6Ec7POOuvQQWbYY889zclOYAuAwXAAQXn++efxr7H66g6HbhIMtJjbb799q6226rTuuvvuu+8333xzzNFHKyFQc4cddphQVL3h3//+9y59+kh0YE4O/wfivC1mW0Agyzf8119vu+22fffZZ/iwYT26dxew/+tf/1Kn2bBr10suuYTqx2wLWIJvv/1WbX799dfv2LHjkUcfzbQj/gOll35ynRJwSHhjLqkb/eCDDwrlr7nqqvvuu+9AvwMOuHXgwOuvv/60005zW5PXvHAq1/Onn356Kff7/Isv2JJi/33zwrlSSl0SaExjYHts2HHHH7/ueutt26vXHXfcsfjiiw+45RaGQaqBv3n66ad379Fj0803pz6cD6cEvywNt52W4bAfeeSRG2+8cY8ttpAW3H777elrvoBlU/3aPGBCPvvss4G33rrzTjstuuiivPs8ButhgRiA2Vu1OvPMM0UbygYqGSuttFKXzp379eunq4rgOO65xx4SINaTN8M/qktctuPsc8656667DjrooOefe267Xr1+//13wpcyWmWVVWTn/nPzzXO0akXm6PgpfU8PPewwO3jD9ddfffXVjL1Ur0KO3fmHy/MfdXga+Fh+HiXugl951VVcsR133HGPPfZw2e8YNGjNtdaSPWYD+BbJGZwcwH7MMeecc9f+HDY+3J577aW2LKB3Vp3A5Kgmx2e1FzaaMbB5kjlSBPTsGaef/sLzz3/4wQfs/6677SbhwCl4+qmn5BCeefrpyy69VKXREbGddMpll13GN0eXHbrowgup5gMOOODc885T1xUSChXrFLlzQN0YywYccsghzpMFJDkxSD29+eabW2y55WmnnuoVQgddOu6NN954+eWXn3v2WciIkSOXWWaZFVZYQZQgODAqOck/CidAzv4F55//zttvX3nFFYstthjhu5DMNiBhrWv8zDPP2NyFFlqIrIYOHbrzzjs/9dRTCjnsMUM+YMCAl15+WYZXatjtTX23f9QRqvNjW7Vq9cADD1D6ssR8MrfMrT/0kEMeeughHpj6AT3gdDl+Mr3iA5OgwG+97bajjjpKQkmG4Mijjvryyy933XXXt9zhN9446aSTXOc0TURWjQiNZgz44E888cQmm256/wMPvPjSSxdedJGdy/77optkfxDFYUVIGYa77757x512Ou644yiLJ5966sSTTjKKdt5ll12UKOWjr732Wir78MMPV0kuKytLnpLw5U6MOOPGm24aMHDgUUceqdAksRgexS1jo1a8c58+ckRCjW7dullAz2233WbbbTfeZBPEXttt17Nnzy169PCIFtuhd++vvv6agYln+EchRMrHd98gbubb77zzv//973O/L7746quvvvjyS+gnn3zC8dcOGz78iy++mDBhwjHHHvvU008PuuOOvffeW6nfJd9pxx2ffOKJDTfckKkwVXVOiC42PIemzT9OAk6FKP/FF17YfffdHS22wcV3qbfeaqtXXn6Zo19ZUcGTkMVdcskly8rKaPkOHTrst+++zZs1owcUq15/4w2lQbf1wAMOWHiRRRZdbDHX36Gqqg7n6x8n0un0wY1mDOxui5YtqXJaWIjAo5y7dWuWP/tv8LRrB5mnbdvs05YtcbIcAkA+wkZduz733HPXX3fdkkssQRlRGXZdWomi6dy5s2M0X4cO3EyHw94TgbEmb9eu3d333CMg2GabbfgI5vEoD8rKyoy6dcCAe+6++9FHHpHikP3Qyld6tN9++z3x+OPMUoB77rmHRltiscXywtW8OWfhrpiAQd1zr7026NxZVYDh3Lx7d9C9e/fNNt88a8u7Z7som262GfPJfr/yyivHHnOMsMAttQX2jgFgEtR7hHdrrrmm7VvoX/+68IILVl999b+XYGfhjW76T2MAeHU8Nlr+iiuu4PPtuae87B477LADf5GF2GnnnbmGC8w//yKLLoqHHrDIM844Y8iQISqCb7/5pnrVVVdccdCBB0o/ikpHjBjhXJlwthYtKATMKTSKBBrNGFAHXTfckEqVO5btueTiiwsB/dprrrnj9ttvu/XWk048kX6n1tV+aYqopERg0aNHj64bbdS7d28lB8haa68tksC8ySab0DI2frbZZnNcJJ2coS5dupiNDkIplIUjxSxRTBJEP/70E7xr165wSgrz0ksvrbDBzARAx9lqjjkcXE//geDDRUVKO7ZPiS+ACsHpp502cuTIHXv3tguBmG2vu0673HLLrb322v9ed10RWN999mEhNurWDRAs6NylC5Ag/uCDDziDtukfKNX0k0nA1rvp7ji8HFZRoQ0wgV9WXo5BzenMs85SwHNUsLnpcrx4uRc33HQTB6XLhhtut/32NIOioyv84osvDn7ggUUWWYTXiD+FRpFAoxkDO0opS/bxstWF6PF8WGstFF6nUACzzdZWVFRwSJ2Ap595ps+uuwoRZasff+yxIc88c/999+3ap49cEPpvv/1Gm9NWMjnqz3JQKpwMD4pDZp46ZeFIOSvGHnjggTfffLMuZkYLM9NSNmECPAbLYD/qm8qQWRsIR3DAnAvet6j9bb311iwoyds6pZda8hZbbqG35XzzzTd27Nhxf/xhYKdOnexst402CiDgg/To3l3gf9vtt7/77rus+KwtwPTrGpaAA+YyHn/ccffee6/AMQlCdvVkw91KbQzOzM3/+Y+bPv/88990881PPP64yiJmp/Siiy8+7fTTcbIW2hQaRQKNZgzCaqjUVVZZ5dRTTjn5pJPy4PQzzjji8MP5ia++9pptdjjCEPqXNqGs55577sceD4rRCgAAEABJREFUfXS33XZbddVVVXQ32GCDiy+55KabblLmVVGg9238mNGj52jVatAddwg7TEK5Gx7maaDFKf/ojZWVlXBZi44dOzJdDQz5Bz4iH6ZxrOROLdD1KERBzuP/+KOWXPNnRUUF4bOgEndC+HP79Tt70t/5559/9NFHG87/MzkkhX+yBJQK7rzzTk5D+DfO1+nUKQCNIYIkmfk6dozPiaPFeFx55ZXigIcefLDnNtusmPtt3K3bLQMGnHjiiRK8H3/8sXS0gSk0igQa2RjYPxkYRaFC2Kdv3z322INOz9jwgsqPvafrBRYeJj+sRfPmupJIWpZmpZVWeuThh7fccssxY8ZQMUahNwwmpLDUM2Zv1crRWWyxxV5+6aVtt93WKOYnQOF7PU2hSAmQMJtRYyISf2Rtyfjs3/NRzDYV+a6U7W8qAWfALRs0aNBXX321/3770QZ99947ALVwxBFHPHD//Z3WWcdBSn5glMk04yqW5v/t93w7bObUptBYEihprInCPLaHjqYFCoH6pigojsAZtyiVlZV9+/bl9W+51VaOy/vvv//pp5++8uqrJ5xwwl57771up04brL8+S2AItQ6cGKN0C8FTkHzqCLJAz7/wgoqFCgS4rH//Sy69FIg8Lva75BIHVMRQOFtKIUkbaoOmThSGGxhaSAr/ZAk4BhPKyxdccMHtt99eUZBDFqBXr17bbLPNCiuuOGbs2Fg+bjHX7dBDD33jzTcxPPzwwx9+9NEnn3wiybzffvuddfbZ6s+qVrzPeEiMpMjUSaCRjcFkF2HzCv/tYMp9k403ZgZ4AbafSdhk00232267AQMGKBQPHDiwdevWcVbHKanvLU6bBDfVz5kIPLSY4JQD4tG111038NZbwS233GLOW3M/XX9+9913BoYhaRtLgNCkgKTUyBAe04tHRHuYuQhcPEgK/1gJOD8OwyorryxRvNrqq6+zzjqd1l03CWuvvba8oiSw0xKkxP/bc889r73mmu++/55T2KNHj00322zHnXZ66sknjzvuuMv798fWgDbwNIUpkkDTGQMpZoXi2269tWfPnkKEvFWyB5ttttmjjz7K8isJDLjllocfeuill16y5e3atZOzjo9I3sBk1ySdO3dWf+Z9sDoeOYIQNahnnnrqpRdffOH55/PgxRdeQDGqcEmG/8NBTKB298jDD2/UrRvZTqk0/vrrr0UXWUQdaL311vsjly+a0hlS/llJAq7YUUce+egjj1xb1++G66/fc489/vzrL3c2fDXE5d19t92eHTJE6fi2224bOGCA200tnHH66dwU5zNwpm2jSKDpjAEbLmMjHlx6qaXq3MVx48Zx5JdaaqkuXbowDGuvtda8bdtKN2EuxhIQh+FqAGusvjo330lCARAzNGveXCKoPihyfrP9o4DobNmSSy4515xz2r4p/XbbIUpjaJlzrsCUDq+DPyX9nSXgPLieG3bp0qN79+6bb54HW2yxhYpg3jlxAsf+/rtAf4UVVtioa9dNN9109dVXF6fKOeNMr23jHoemMwbWbWtpfKq5vl2kcbiTeDgRfMmy8nKjigfTOnAGelFylC6601MfYEjyp3gsAZKxI6QXU4pHbIcNtZvEDi9+YMo5S0rAGXASfh83zu2uE5w0PIXf7vjJDThIRskdmaSQJ6VMuwSa1BhM+3LTGVIJpBJIJZBKYHpIYCYxBtPj09I5UwmkEkglkEqgOAlUVWWNgSq/NNyc6a8xJECSSlvaxpgsnWPGS0DZw4bO+HWkK0glMB0k4HiH1FzZ6N+yxkAO7/HHH7///vsfSH/TJgEyfOyxx776+uuHH3542mZKR88UErjvvvteeOGFL774ws7OFAv6Wy8iXfxMJoF777335VdemfDXhExVVcVvOWNQXlExbPjw77///qeff05hWiTww9Chvwwbpsb18y+/DB06dFqmSsfODBL47vvvfx0xQs3T7fjxp59mhiWla0glEEvAmWwIfp7Mif3m229Hjho1YeyYzJgxmepMNjJo167d8ccff9zxx5+Q/qZNAscff/xJJ53UqVOn0047LZXmtMlyphh93HHHHXjggZ07d05vx0yxH+kiJpXAiQ3/TjhxUvb8nuO95667tqiuzkyYkImirDGoqqqaiv+kqLiqxD+Oa9y4ceXl5f8wec7KuyzOKysrm5W/MP22v6MEqjPhL3mrrv1VVVVX1f7QivqmqqqxP/9sHszN2rTJGgNYCqkEUgmkEkgl8DeQQNYMSOpkIV5tTvt7kCOoCEeT//tfqkQDo3+r5uhgnnvuFm3bpsYgJ760SSWQSiCVwMwvgazWl9ah90Hdyy2h3Ot+MpFaVV5eNnx4NjuUyZS2miPTqlUmyqWJJrIUYCkhlUAqgVQCqQRmCglk9X9UuJKsgaillpRM3r+vrqws+3V45V9/ZTJR1KxZ6RxzZHK/yY/MsaVNKoFUAqkEUgnMMAnUhgNZgxAvghkAcbcoS1BVVf7rr1V/jM9alVatms3TJg4kUmMQSzJFUgn8MyWQfvXfQQIRMwAmLpV5CJ2AFGMJ1IrLR46s+P13A0tatsy0bl3SomVsTlJjkEl/qQRSCaQSmGklQNeDSerF1pq1C7l/ss+ke4rS5OW//VYxdozRUfPmLTq0hzAP2Tb3T1FT5DjTJpVAKoFUAqkEmlYCWYXvjTV/wAJU54xDzhBkSpSMs0mf8KTetnzM6PLfRmWqqqPSZs3bty+ZbfY81tQY5AlkluqmH5NKIJXA318CBZYgGIHch8kORdHkTYHUUPnIUdVV1ZnS0ubt2zWrLRrn5qhpUmNQI4j0jyCBX3755ZNPPgl4E7Qff/zxiBEjmuBF6StSCfz9JJD1/+u1BCxCLiaYvCWoHD++3C2rrIxKSlq0a9dsrrnrFEVqDOoUy6xJHJv7jRkzZvjw4dDCj7z33nv33Xff77//3qM///xz9OjR2LS6v//+O3zkyJFT8Z/jGgjMMz73f36p1R01atS4ceO+/vrrvffe+9FHH/WKFFIJpBIoUgIsQZT7ZTKTGVE14a+yEb9WV1Rkokyzedo0a926vgGpMahPMrMg/YknnlhhhRXWW2+9vn37dunSZc899/z555/j72QJzj333PPPP3+zzTZD/OKLL9ZZZ51lllnm9ttv17355psXWWSRPn36/J77VxFQioeHHnpoqaWW2nDDDb/55huj3n333aWXXrpTp04fffTRlltueeaZZ5566qmPP/64RymkEkglECRA3WcDg9DJtWKE+N/8YQiEBTlyQ00V32348OoJZZkoKm09T4t52jbAnRqDBoQzqz3aYIMNhg0btvbaa9PvV1xxxcCBA88666zwkVz+U0455bzzzmMtAmWllVbaZJNNZI26deuG8t1338lOXnLJJe3atdNNwn//+98DDzwQG+vy5JNPJh8FfPvtt2/VqpVzHCavqqqyjNNOO42xwbDaaquddNJJxx13nHBBN4VUAqkEWIJMrkQciyJLyf6TcY+KtATZ/7hsxIjKvyaYpHSuuSSIMlFkvG6dkBqDOsUyaxJlh8rLy3v06NG6dWuGgbf+wQcfhE8dPHhw8+bNQ0wQKFEU7bfffnBp/ddff53leOSRR4I2R4zhmWee6dy58xtvvLHGGmsMHTq0e/ful19+efw0ILPPPvsuu+zy3XffiSoqKioOPfTQk08+eddddw1Ptb169ZowYUKdhsTTfyykH/7PlAB1n2cJcnIQGGQ1eZT75SgNNlVV5SN+rfrjDyWF0jnnbNG+fVSSswQRQt0DU2NQt1xmSeo777xD46+11lq+juL+6quvaHA4eP7554UCUTTJQVl55ZUlc6Rx9tprLypefglnEtQVaPY111zTzBdeeOGQIUN0jz322G+//TbJBmdm1CrEECeccEL79u3jiMQjUFpautxyyz377LPwFFIJ/JMlkPP+JxEASs481FgCAfokj+vsVFeXZf/jsnGii9JWrVrMyxLkVP2kFzxvaI4jj5Z2Z1EJvPLKK5I8NLgEPe288MILH3300eFbP/30U+WBgCfbPfbYQ/Qgz7Pbbrsl6QFXA/jss89OPPFE2jxQ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d8cee6zEy7LLLhsYksoRhcbnMzEbpmrfvv0iiyyy+OKLU6xffPGFHfEUT8Ng76jRU045RXhBBRO7jD/lHm+9Xdh8882Vrx0Sj2xH29x/+8qSde/e/d5771UbgIe3KESreOsismQGrrrqqrfffrtLGhgablVJMYgGaADunVY3D5Zffnl1FHXjvfba66effpIcU0IXD4HXXntt1KhR6L4Fz2QtUN7M096t1fsTZ4oPeS5nU4SOra5SMa784w+WoEXbts3btJk4VxFY1hJUVQW5JVtDQxdSDBSx0GKmSXmaRAKSxeE9QTu4/7qIAYHHgOKI6AZOeDig8W1XP9xrr71oJV5hDJIVErKcOwOT8NBDD/H1TBITf/jhh2OOOSbkMWIihEY2SQyXXXaZdDY6ePnll88444wwCZUnGXLjjTcyD1rWiAGwQkXUp59+2uIlKL799lujkkCF0UTb5H6yBFTD888/HxjOP/98mivgea0vvfbaa/OITdDdfffdWVamiObixVNSlDtElyjYJ+osXoaiV9++fVUOON2dO3dmOOWLQhyAJ2wihLpnRWhbZgaIMG655RbusFKw+alCvvlknSRW6tBDD2WlGCdzqmNLW6kZUMe2AAXAASQPHDbBxFprrTXvvPPC46errLKKrfdREjgQGxovvgHj5HUgGIMwlcWjgNDVBtwbGUgikj+wAKslKB+OzmqyiCIk6Sw8QgSjmgaqs3agOvkuqwWBAiktLULBVldnLUHOr2IGpvSvHnKhQFD62YggM7FaEIiZon9FrLXouTBalhi28C8i92imBapHVO6azbQrjBemkOj0u3h0KCIdpyTOIZLG1U0C74mzifP6669Hp9/79Omz1FJL2R1doLjn5tBNFFYMNNfdd9/tpmFIAt30zDPPONwxsbS0FFtJSf75EXDQBQH4m1SDDEMYxenjyQbceiQE1AzvuOMOTj3/jg1wdp0fADG5VwTmuKVMZdKpsK5du26yySY8VqsNT6UvaLSAJ1s+7FdffUX5TvbfbEmOahScv0xH89l58Vrak9qC6HLqPYql4XUWzwwTMqsmbSIppH7G4QUyomoJeADFTRtSglIiG2+88YW53+GHH87o8s3ZD9VUaSWcdQKjIinEiDIGJ5xwQpLHo+T+uhTsvUth61lcS5Ks16oc4DSQJbBNkBjEAQ4na73iiisiKirIMpG8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q6666qKLLoJMFp5//vn999//r7/+SnIS1HfffffNN9+Ul5cn6TfccMPpp5+epMA//PDDww8/fL311lt77bXXWmutNddcs0+fPo8++qhHUwpP5n7evt9++9kdWhquZQnCVBUVFRJEiKGr9aKzzjrL9/bv3z/s4gUXXHD11Vf7fJTRo0fjieHrr7/GaYtxYgMQ4Bi8+uqrMRvEGwEkBl0QdxsF+ScYg0YRVDpJKoEpkwAd8eabbz7wwAMHH3wwnUvNPffcc7feeqvu4MGD//vf/2KIZ/zzzz/33ntvWuCZZ57JqaCa5umnnz7iiCPOPvvsmDMPmTBhwtixY//44w+KxoRlZWXjcr8xY8bgtACKDNCw2gMOOKBfv36//vqrR8AyXnjhBUid8NNPP3kv1aZNwjnnnLPLLrsceuih8ajvv/+esjvxxBNPPvnkk046CcP//vc/T2m66667DuItTzzxBCTAu+++e/vttzOH2gADBw6kxD39+OOP77jjDtKABxgyZAiFvuqqq66xxhorr7wywxTo2pdeeunhhx+GxMBKdenShZw322yzY4455oQTTthpp51++eWXrbfe+pRTTiGfmDOJvP766yzuZZddBmG9aO0rrrhi2LBhN998M8tN51pqsMfwMDDKRAHJaz/66CM7eNhhh1144YV2/Nlnn7XCQw45hN2i38N3CVbCSkj1yCOPtMU2+/HcD2K4sQ5DbBG9FOS9aHp0U2MwPaSazplKIOMC33TTTffee2+bNm0oGlrGtado5p577vvuu+/SSy/lY8ZicvPprDPOOIP6oDpjoFC22mqr4cOHx5x5yGeffbb++uuvtdZa3GFa5ocffujWrdvyyy/vjTgrKip+y/24+WzGjz/+SCfSOB6Bueaaq1WrVpA6YYUVVnj77bf/7//+752CH9Py5ZdfxqOuvfba4447DicL9957752d+3k6xxxzzDbbbBBvgUPA0KFDaWpqmgSYkADcYbrS0xYtWpAP0cEBs7HlllsuuOCCbCqnm6Kn3OEeAeuPp9WlYZmuRRdd9IMPPhAx7LHHHrvttpuFESlDxQH3amx5wGqybZx3WviWW27p3bs3e+NdjKvJZ599dvytW7e2MMjELYsy/testFlpSWm8WgzHH3/8yy+/vOKKK+6337523JwPPfhQu3btzjn7HCdh/vnnxxPDt99+u+2229pi2/1i7gex2pNPPtnb88Igo3ygLYYkAREkKVONp8ZgqkWXDkwlMHkJUFg0yJxzzhlY6Rdd+i5045ZCKS0txRxTYsQQT+NuHkJld+7c+ZNPPqEozdC2bVuqe8kllxR/4Pz3v/9NBwWQ3mGc6OU634I5D7yUKq8TfAILF/OLIbyd7st5t4/vuOOOI0eO9NQMAJIEtommEwq89dZblhqACdl3332TbAHnoVPunOuuXbvK/IgzaE8a/5tvvqFJzeOTA2cm94ev+/33370i16tpKFBWsHnuV0NK/MFGmufyyy+3+E022YTSf+SRR5jtZZZZhoVOME5ETZjVv1GGQchCJv/fHWrWrFn8fx9mry3SJmZqf6QXxAJJ0mufZ2yQR3E3RowCcTcgKCDg09imxmAaBZgOTyVQtwRkY+RA6F9eOWcTDmThqZ7rr7/+zjvvhCRH8gT57DQRz5diCoi8B4+7TtUQxlI0Qe9LQKMcdNBByy23nPxP+/btdfOA902Lrb766jHd8BgvHuFic5ZjfpOAuGu1cTfoqdAGBjhFyTrmlHNNg2JUYEi2jJygJ0nZYost3n///XXXXZcJJJzkMswsweIDl1122V133VUMxGzIjBGIUEwiqGPHjsmpAu69dLdWV2tBWngAcwYkbs1fYwxiUs4Y6E346y+SF17Imz3//AuSS+C6G64bMWLE4IcGyxCGXBPOGIQ+vsKOi0WUWCD2nVlViigtqVHO3gjCkHg9MSXQG6WteV+jzJVOkkrgHyUBRcUePXpwJ59IJMRjCSixUkC8ci4tLczJBXIIuoiS0UljwEPceeedPT366KOlULbZZhspDsixxx5L9ciNxNMWIpSdYilVIlkvw04fJVVkkp9NWmKJJRZaaKFApFnUF+RJtIFSZMsrX3rppZPMSd1UHx74w1MBR+g23Po0oUOSh670ap67LyV8fn3yKdmqOkhAca4l0JQupOnFHIyKNsmZhxMySlgbRQwPECgBDy2hMXVJg4EeKGXl5bcOvNUuW6GFQcDtt93eqVOnD/73wWWXXZZnDHr16qXYY4tttN3XhTgAYqa99tpr9kQGzzKAF8WQ10VHAZCphtQYTLXo0oFNI4GZ9C20DJecGaCV9tlnH3FA3kJVO9Vv6TKWwPWOQZc/SO9LgMRDOKQy75Ts57kfJahCC6U+KDWGIeasE7ESmZYLLrhA5LHUUkvVyUMzeip7Tp0FBhkMAco666yzww47jB8/PhAn27Ic3333XZ7DXucoGpl8ZHi4vbF9oka9S5pIodh6Bg0aNGDAgP/85z8sa+EkKrFfffWV1BBJKkhw8x966KEzzzyTbCnc+eabT1HEKOpb7V2lXdFYtcDyOnTowOxJl7F8auw33nijR0cddZScvpSRIcUA+bA6VLnYrkXLloYEbRsLUBegB4rvHfzgYOt87bXXfI6KC7DvdlyLznphjsGu+TpbbKN32Xln4Q4ESILZyjAnZgihaeExoMR4QDCAgE9dmxqDqZNbOuqfLoGysrJhw4YFKSjw8gQDrpW27tmzJyWitBtD9+7d6YK4K5uPYfPNN//www95u2IFKQIZA8ru/vvvF1WogtKhKACF3mR1ggPrFXkQkkIKszRv3qPQNfCQQw5RWJbQDxQte7bBBhuce+65tKREDUoAWQ5TWWFytfIziJIzvG8fTufCt99+e+pYnj0MzGslvhg836glrvB04YUX5gXLhCgai3iOPPJIRXXpHWoXQ546W2ONNZgTyl0Z2dsVV1kOo3ACbjW7AgEq52ra8lcWLzigT8kQ6H766adyaB5hAPVVAkySB9a8yCKLcNgJp6oy+/fTBdUf2OC+nWBDl5kRn6273rrkE+S28cYbK/7DY0lS90yvL33ppZdsqG21ucAB+PCjj6zw4YcfdgBQHAZHQpCXPFfeCMLr4raQEj+aUiQ1BlMqsZQ/lUBWAlxdjio9KEWw//770xpZau4fbj7Vv91229EjlC/lBWi0jz76CAIQqdHttttum222kSw6Mfc7+eST/SlRAOHzchiPO+64QNHSNZQm9Zp7wySNmWlzQ7ifebXTmE/swrmWtrbamMhlXnHFFS1SpitJl9Cneelf1gswA9b5+uuvKxTTbn369Ln66qv33ntvWn6jjTbionLMpd3jackkqEjGZtVVV7VyVQqKOzBwn0UDTCDfmdAkSbjM1Pdpp52GoVC1devWTdXE21999VVqfY899sAWwCJDzGTxKsBsJxMlwdK3b1/tnrkfBNggGRuqlv4VMYThofVGq5Wm06X0tQICLbD+lVZayS5Yc5B80lbBvVeLE1D0Aqztem23084721+7bJTaz9Zbb834odhxosYz77zzcvyJxUbbWeAVNk7qDNEBQNHCTz311F9++cXkMVhtjDc6MiON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6dttt9321WOHHXZ47733Qn799defcsopwXe8vfPOO63H5fbZZ5/PP/+8IwNvueWWCy644LrrrrvssssYGV166aW6F1544W233SZ8jklAJ3r99dfjkQ16LOnfhniyH3zwAU06Qfig6Gqjq8UH4TtC9cr1EvMQavNUL8mfxRfOgBEKKiwwUi3w1FNPnXbaaZttttmWW27Zv39/fN++fddff/1dd931rLPO+uijj/KrOfvss9dee+2TTz4ZGmqD+vXrB0bBOKTLK2c82FJ80Ko/YMgxuniMLpptttmWqztWWGGFL7/88rDDDqNJp1U6/vjjN998862GPLbZZpuNN954iSWWAPExyuXuuusudxfUv39/LsQpPqxnz54//PDDhx9+aCqXIwz67rvvvv76a+4hKCti3HHHHeecc07o1LdPPvnklVdeec0114B+LglA33zzzf/73/923nnnW2+91YTcXo2LrZ8kJNwz5R49ehx00EE8Ezr88MN1jznmGN46Mx3lX3/9dYsttuCxPLt4KNGeeuqp7HDggQfSqSdWdVPol19+ibMkDGW2mBzviffq1WujumODDTbwhvz8888xcIS3hTMY4SYtJiwsMNACbf0FRPiDJZdccrXVVnvssccef/zxRx55ZOaZZ4YsmPnmmy8/8NVXX5133nnh3T9zhyEQFox+//33eeWMhylmW2yxxZZffvlnnnmGfP/9919ooYX4jwhaSZzt2rXrJJNMMlnu0J1gggmglRnotEpgHaBbQw1BUksC8THKyt0giBRlI3gq5/jiiy8mnHBClzC/GsWkk06qpQ+4OZInnniCXH1DWQM4cjCsdMMNN0w99dQWRq2eXnrppRVXXJH3OvPMMw855BCOE5rjv/nmm4kmmsg8ZjNWWz+2XiKu5z/Y46STTvJokKkmnnhinuC8886Lpcaon376SWbAqk888UTuyaTsWmut9e6774ZaTSvFWWSRRRZffHEeyyn3uOeee3ou66677n//+18SLVO88cYbf2jtYDc6vxMVzuB3MmwxbWGBNi0AoRSOfdi+d5VchCH5v//7v3rMIiGnrHycEeWppppK29Y1XAIkwSkRaLdu3aipk0Bwfmi66abTRcJMqQmohXTC6owmnHDCo446yqrotEqwEjpbQJ6mrB7wF77HqE8//dSCwR+fYSXKLxYjIbA2FDpa6K9dYIEF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YHGTTTYRNa+yyipTTjnlVlttpRVH562gknP11VfzE6uvvjqQ7dKly2GHHcZnBIZCcyj88ccfi/pp9u3bd91119144403HXT07NlTTaZ79+7XXXed4fTzk8sSwHoeuPNn2+HDCeUVeJSaybOzk002mTu1YKWkTCgpue222/75z39yhJmwYEa5BQpnMMofQbGAcc4C0DALpRWC4PJ3333HCgGp4403Hh5JFNSChNL4jP70pz8Jt3XhOIV11llHlencc8+dfPLJp6gef64ef/nLX6AwATlP4BImz2Y2HN+5c2cuZLvttttyyMNewsEHH2xyavVktmeeeeb03PHRRx/xB/WaJJNMMsktt9zi0ksttZTi2LLLLovhz3hBXqqt3y1hYEEj3wKFM/g9bF7MWVhgeCwANKG2sruN388///z//u//ZpppJjWibC6w+8QTT/z9738nkRaoKZ188snqSErw8oyzzjoLuK+22mr2HiaddFJpQb9+/c455xwSOYfsgRf5+uuvDTScLznuuOMWWWQRWxTO5ol/0rUYavXEiyhD2aO+YNBhWrPVa4bEPoetgrvvvnuHHXZQGpIJHXTQQdyJ0fKG0Cna0cEChTMYHZ5CsYbCAqkF4K8Q+8ADD1RHgphENhUee+yxtddeG+IL/xdffHHFIrG8U3ILFZslllhi4YUXVn0iAfe9evWyT8BhAF+l+f32248ccRsKSgsssEBAMwlSfVLAufzyyyF7nlzLFrGV0KknSYxK1+OPP/6vQYdI//vvv6/RtHVhYd26dXNRy3Y711xzzf33328L3X7yLrvswqXNP//80gVZAvdTM7zojnwLFM5g5Nu8uGJhgcEW4AB0sk1jgG7T2KYr9CSH7HfccYddgb322uvoo49ebLHFHnroIZUipzgDEAya8UE2GC655JJbb71VZcYM559/vtg/dpsVptSLQP9ll13Gneyzzz4mbJ9sVks7Io2I+bM2W21I+KRg8q3L2QjZfvvt9957b/mH9fA921QP5Sm5wo477rjTTjtRWH/99dtJLPJzjl78WLeawhmMdY+0uKHR3gLi9AxAVV2UhoA1ZFecsfaZZ55ZrB3Bvu4KK6zAAbz44ov/+c9/YL3NAEI0yyyzyBumnnpqfBA1wbi6fHQVjrgNiYWuvWK1I65FkK769NJLL7366qsffvih+L36Y0etN2+//ba1GZ4nU9U4A/6MZ8rr4LkczgD4u51pppnGkGmnnba6nfFna4b+s846a+/evTkDmUFTU5MhBY1aCxTOYNTav7j6uGUBEbG92RtuuOGFF15QQ996662POeYY2wOqPUpDzz333B/+8IdwCZldFGSA+MYbb6w4wzHggxSLRN/5sjt4Vc3/5JNPYizngYfF0YXXMfOMM8542223SSB22203FaHb2jhuv/12OxBQO4ZnLe9lG0NWodSza/U35Dz55JN2lTOFPOPWZBgqUcpBxx133M7VQxVrttlmW3XVVTfffPO8csGPWgsUzmDU2r+4+mhogd9xSXZrn332WVDYs2fPzz77DDovvfTStnntE9hQnWeeeeqr51NMMYVwXsiP+Iwlq8cyyywzySSTQHNbzdlyBdrTTz895T59+qgp2a01+Zprrpkp5BlpAady11135YUd4ZV9Vl555bfeessMH3zwgT1t4b+9ilbHWrwylxrRfffd51p4Pubuu++2c2CSf//7362OKoSjxAKFMxglZi8uOo5aYLXVVhOSK+5fdNFF1157ra3UE044QelcScd+r7RA/F5jGvG+ctAhQx6ch9hckM6dZPpTTjmlHYJ11llH5A52FeVdy5yZQp5R7am/Vl6hLX6VVVbht1ziukHHWWedJfBvVd8WiKWuuOKKoF8q4PaRGVZaaSVe4W9/+1urowrhKLFA4QxGidmLixYWaMUCw4TOto5tPKjX5yfiD3gXlSX1KO7D5kT+bIX5n7kAABAASURBVA1vP0Apv0Y4YruyH7WmNdZY49RTTz0xd1gkv8UjjtjLFbP9FguMW87gt1iqGFtY4Pe2AGegjiSa7siFmpub7Tkb0hFlCQTnAf0z5YknnlihSXqx9tpri9bzJIRXXHoz90vxslFDZVwl/3+ryV3GH398OxmPPvqorYWMnnrqKbWjk0466csvvxzqnIXCyLFA4QxGjp2LqxQWGLoFAPQGG2yQ/bxQ+wOmmmoqtZf/+7//a18tzs4999zdu3fP/9BOly5dVHvWWmutWWaZZa4hjznnnHOOOeYA4jF2mFpeJF/8kanYIeeK7m/t4BKcGqb5C+XfzwKFM/j9bFvMXFhg2CzQuXPnyy+/3EZxR4Z169ZN2T37CdT2hwj/zznnnLwzoK92f9xxx6nYHD/kYf+ZvIMzmycjNavTTjtt0003zSSYXXbZ5eabb7bUGrKffOWVV04zzTR0RigVkw2nBQpnMJyGK4YVFhjlFgC+o3wNxQLGGgsUzmCseZTFjRQWKCxQWGD4LVA4g+G3XTFyJFuguFxhgcICv58FCmfw+9m2mLmwQGGBwgJjjAUKZzDGPKpioYUFCgsUFvj9LDB6OIPf7/6KmQsLFBYoLFBYoAMWKJxBB4xUqBQWKCxQWGBst0DhDMb2J1zcX2GB0cMCxSpGcwsUzmA0f0DF8goLFBYoLDAyLFA4g5Fh5eIahQUKCxQWGM0tUDiD0fwBjQnLK9ZYWKCwwJhvgcIZjPnPcMTdwRNPPPGf//xnxM3X0Zlc9+WXX+6odqFXWKCwwO9ggcIZ/A5GHc2mrFQqH3744UcfffT++++/8cYbmPoF/vLLLzvssEOfPn3iVyJ/++237733Hk1DKP/vf/8zwwcffPDxxx/rDgd9//33MaFJ4hKff/65+d99992vvvrqu+++22WXXY4//vjhmLkYUligsMAIsUD7zmCEXGKISVpaWl599dXnn3/+hRde0OIDGig9+OCDL730EqaGfvrpp08//TQvbG5uvu2228BTXljw7VigX79+f/vb31ZaaSWIv8oqq2CeeeaZvH6vXr0+++yzSy65JP7JKvnB4osvPv/88x911FHU3nrrLd155pnniiuu0B0Oeuedd5ZffnlrOPnkkzknM1x55ZXzzjvvsssu66GvuOKKF1xwwdVXX33EEUc4VVBhgcICI98CI9sZNDQ0bLvttuuss06PHj20sIkkbnv33Xc//fTTg8+3l19+Ofz64YcfMuE333zTs2fPu+++O5Ng+IZrrrkGplw45EFy8cUXf/LJJ3TGTUqSZM011+RQGfzWW289++yzn3zyyS222IKXDYMwkUINT5D9E4mLLrroqquuymirrbYanYkmmgiar7/++jvuuKNuDckqzj333E022WSDDTbo37//d999V6OgO9dcczlrDcstt1z861quJTk47rjjuBkK008/vQWccsopNV7KqYIKCxQWGAkWGHnOAGTAoMcee2ybbbY5+OCDDzjgAO1WW21F8vjjj3/99dcTTDBBq/9Kn+xBmWKCCSbIm6NTp04wLi/Zc889e/fufeKJJ6p15OmE6vH222/nlcc1XjXGLS+zzDLjjTfeQgsttMIKK7zyyitffPEFITr11FM33XTTGuPz2U5R0wJ6ycQZZ5xR/w+e/Pe//zXb1ltvzcLKPjvvvPMSSyyBN6qGuH8S6aCWm/ECHH744SEkQXPMMcff//73vn374gsaeRYorlRYoGqBkecMQM9mm20mPDz66KNPG3Qcc8wxJOjFF1+cfPLJn3vuucsuu+zmm29WTaouL21sLYL+LIFIRaWSrtAy+Ghfe+01tQ71jRoy3OSLLLJIqI2b7cMPPwzHZ5999rh9ED/FFFNMMskkukpAb7755tJLL43PU7du3eabb77rrruO8+aqr7rqKjbPKwSvsGPyO++8k0d/pHqw/x577JFV/0JNKzn485//fO+99+K5bTUi0QA+T0suueSjjz7awX/3MT+w4AsLFBb4jRYYec7gj3/8o+8cZKs7r7322nPPPbdKsboQCR+w2GKLSR0w6gbnnHMOPm5MIdteAkCHNSHRygmUGu64445LL73UWRLEYQh7MQXVWECNXk4255xzTjfddDDaPq0y/fbbbx//YuKzzz7L2rPMMkvNKF06Tz31lO2Zm266adJJJyWpIU5CTY6PlzfEKc9Rue/GG29UVgpJ1jY1NSk92SviXaQOvH52KmPsWHz88ceRx2TCgiksUFhgJFhg5DkDCC72FzYqQ4s3AZAC0XrrrXf77beTizohy5ZbbgksbrnllqxkIfB0VmVD1SIrRpsK9N91111wzVSZmaBexhdMqTTQBir1oPmDDz5Q9Bd6n3TSSftVjzgtY+NEM4OHMFoPBbP66qvPNttsmHpS9PdQbALnT9kV0HU5bQ3ZujDEFgUvLjWpOavL5XiIdPAFFRYoLDAyLTDynIG7UvwRbKoPiDdtCysvCCq32247gOKsXUrB/oEHHnjyyScLYEnkEOpJ/fr1UziSIqy88srxk47O2vw89thjeQ5naSKTSxcwBdVYYMCAAV999dWmm27K9e6///7//ve/Ved400wN/mZ8xvzzn/889NBDFXY4XXs2mTzP2DDQ7dKlizajQPlvv/02k2TM1FNPjbe7Y28AU0+xEs6+/lQhKSxQWOB3tcBIdQZAXNCnFCAUjbv629/+Bmggu644FGap7wOvH3/80b6vfcu9995bODnVVFPdf//9xs4zzzyvv/567BbUQIaix8UXX7xx9eBj1CKwG2200YYbbigiVqFyiXGTnnjiCTe++eabcwbSsj/96U+6GbEt+3sKmQTz3nvvrbHGGrvttpvtXEWbmh/cohDU3NyMqfHBNV0KGSkJ4m04a1slaQr5lFNOqS2osEBhgaFbYMRpjFRnIBoVFSpTKCtfc801hx122FZbbWXXNz5++QHUlgTYSPjkk084A7G/QlDcrO1HfsLYmWaaiRug/PPPP8epaI888kg+gEtQVlKMsvHAZ0xWPTp37mz7NNTGwda2rmi9a9eurd57t27d1IheffXV7CxPzG0suOCCe+211/LLL8+krdb36XsQ2gjnMUE13RBGyyVPMMEEdi+iW98+//zz0047rXSk/lQhKSxQWOB3tcBIdQbuRLBpyxFYn3LKKSJWFSGoTY5+/fXX7H8m+Mtf/mIzeZ999iFH3MAll1xy6qmnqgWpWogfd9llF1vQTmW0+OKLcxVnnXWWwtEWW2wx/fTTn3vuuWecccaZZ55JCNoyzXGKeeWVVxTfbN4yXas3ztSzzjrrfffdF2e5YamYOh5PTMLj8qnXX399fgOfPCgyAw8uutHGhWqETtlFUPfjP2wX6bZKDzzwwNJLL221rZ4dC4S27r3ArH3vvfdqv/zyy7gpBs/vfoVQy4xS4ey7IEG22bKfm9Adg0iZ91+tHU8++aS8P7sRd60CmZES8Y8//pid9Spee+21WbdVxkv48ssvCxkVG84777xvvvmmVbVWha4Foyy11bM1wg8//NAe2Pfff18j15VwC2680khB200RDgexg0sM9RbMD1d9sLEkVx/Wa41sZ2B96jb33HPPiSeeuO6664KeAw44IBwDrN91110pIHAQ1QzlC6nDwgsvLPC/8cYbPVddFWf1IkKarRLEQa2eGteEN9100xJLLDHffPO1VephEBmALZyvv/4aD6q82TaBvYK6sgplPQDd6nAJB81pppmGZkbysHqhs1deeaWp+GxPX7eeoIQIIHsH6hXGAsnVV18tHtqjesiSP/roo7gpxtENflCb/v3mm28uuuiizz77bNoZ9Oe4444TRQ3qpX+DPHhx9NFH2w2qoaOOOkpCliqN6j/vvPOOe1l99dU32mijDXKHekCPHj24xmyBdhPnn39+n/lC1WOBBRbwN6QLBXFhzQ8lv/3220JA+4uY0AGdq6666mOPPcbHqBjXI7s3zaehDoEwt912Wza/ITYy+aeYyjOigOhwzOQ33HADPmqe4lTzC3RCOVruxAplwMsuu6y9OiTD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w1SFMxgGYxWqhQUKCxQWGFstUDiDsfXJFvdVWKCwQGGBYbBA4QyGwViFamGBEWKB+HHGVqf66aef3n33XafsfN5xxx2YtiiTf/HFF7Yf2vkBm0wTY89WpX5Yf5rlv//974033pj9bh/zdJA6frmvvvrKTrLt9PqZnXKPNfK77747/neHGrkuZbvTw3qPb7/99jPPPPP000/bqy+Xy+bJqKabyccypnAGY9kDLW5ntLbAk08+uc022zzzzDNW+fnnn8PKN6sHAPr4448J//Wvf9mo/P7774HvjkP+Ho6ff/4Z6Nt+vPbaa/kMykEw0Z7qBx98EN2WlpaXX375idzhoj/++GOcNe1mm20WPy8fkqw9//zzd999932qx957773//vu7kNkovPjiiz169HjnnXfwrdJNN9201VZbde/e/fjjj8+7JVu4+cs999xz/fr1sx+e0dlnn21yc3J+66677muvvYavIVu1e+21V73wwgsvrBFG9+qrr15++eV/+eWX6A61deN/+9vf5p9//lVXXdV2/aKLLhrbvJmVvvnmm1133fWCCy4Y6lT/z96dgG81re8D/2c8GTI7xswlGSIyk8iceZYhU6YMmTWIlGQoSSF0SqWSQqRUkkYZIhkydKg0GCrH7Diu/0frWL9tv99vMhy9vdZ7rWtfa6/9rLXXevY59/0895Naog0SGSzRny9tfknywEMPPXTGGWccdNBBcEfouvPOO9euXbtu3bqQCwHAX4cBQHPnznVdZpllsn+aZf78+fXq1TvllFN69ep12mmnwSxm7LWlllpqueWWq1Chgr4Gf2vUqHHkkUdiCAgOYU8++eTp06d7pAVjncL24YcfvvXWW+BYw1CI58wzz/zoo49YhlkVKvz3FUayrVGjRl4nshZB46q9994b6MtvkIfpf/vb36Ix3O/SpQvwDQ28XnvttfUX/PNnyy67bPYUcYoObuMNnWzjnKWXXjo7EvsIzE4WMTNo2bKlY26//fa9e/ceO3bs+PHj+/fvf9hhh7Vo0eLEE0/0ISy76qqrNmzY0Oc799xz3ZZqS2RQql82nau4PCAbEHcDQbgJ2l599VVw6fbhBT8AdN1119kxCAOLFX76GQkNVQjwx4wZA08B1sSJE8Wq4ZErsHYNDXRWqlQp2DDTJAnxL+y0cNY4TAnXZs2aEabE+Jr9HHzwwWuuuWb8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ABGJOGYn//jHP6688kp9Eb3FHRwTKKJk7W+55RaHZabgHBszxo8//nhQzJQK2KCHRfwi2fWXoH4igyXoY6WtLvEeqFatmrJkzZo1f/EkYtUcbJU3hWohcFYqKM8gOy74FVAD/exgtq8wYHvCealAtu26665blvWfNcS5QuysfeybGP/CiWC8zjrreFrmK2wv2OSuovtzzjkHDShTqx8oReQM4i2yOemkk+rXr6+soh6jo0lZxPWq2SrD9hONdSQ0HlmTWWxuGftYDDRrogGVef0SbokMSvjjpqMVqQcWgsVFuuP/1bbSukXkgUQGRfQx0lb+sh747LPPCmun5XlDIZd9eU9Lfnz+/Plz5sz5tcc05YsvvliUWYoWCgzfLdq/jcOMsaLCoqzM5uuvv/5V9qb8aS2RwZ/m6vSi5IH/16RJE0qIwkCNGjV22GGHCRMmBKdQqI899md/gVoYBxzHH3/85MmTw224qr7SwUM/Xj/66KOpU6f+s+A3derU4mEOtW46PlnG8atUqcIPxJzu3bvn/txOPNQ777zz4osvzp07N47o3H777WQcnfLapEmTTjjhBOgfDYA12UftIY4ghvDfGL/102/KlCkGGZi43377jRgxQj807Js11lemRgOejh8/fp999vnggx//pVK35TUGTmrlUaNGKYMrQpRnuRjHExksRueX8qvT2XIeEG9+//33gOP8888nf4em6msQVIl2P/zww9wUtwYVQgNIuQ0NpsyePTv0w3XQoEGAlRq+W8FP0VVNOJj9gVcV4CG/8m9ynjdvXr169c4880wlYrK+ai1MX2655c4999xDDjkEmWW3p8a+1157ORHoVKtAopEwPv3001mzZmWNc/1XXnlFuRjxZMfRapZUlLv33nvvfX/6QX9Vbtv79ttviXjTp0/P+lx9fo899vjJdl/GCh4o2frsp02b5qqv6ShLoHkGGucrNhjHx0888QQOQCEzZszw0Q0WW0tkUGxfJO2nND3QoEEDsfCll17ao0ePhxb8HnjgAfhi8N5771199dVh0LRp0yAFvIguMLL88ssrEccRHQCa+8+7xKewMvwpHTCdbcOGDVNeNuvXtvIA64033gDlMLpZs2a/as2ePXs+9dRTQ4cO7d+//5VXXmlXjRs37r3gH5s02LFjx7gatjv44IO/+eYbmD5mzJgbb7zxlltuadq0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" alt="embedded_DR_25_Def_img_1.png" style="max-width: 100%; height: auto; margin: 4px 0 12px 0;" />

## [인공지능] 선험적 알고리즘(Apriori)



**[정의]**

- 데이터에서 자주 함께 나타나는 항목(빈발 항목 집합, Frequent Itemset)을 찾고, 연관 규칙(Association Rule)을 생성하는 알고리즘  
- 전체 항목(Item)에서 최소 N번의 트랜잭션(사건, 거래)이 일어난 항목 집합들을 발견하는 알고리즘

**[핵심/키워드]**

&lt;구성요소&gt;  
- 항목 집합(Itemset), 최소 지지도(Min Support), 빈발 항목 집합(Frequent Item Set=Superset)  
- 규칙 : 한 항목 집합이 빈발 항목이면, 모든 부분집합은 빈발 항목(비빈발항목 부분 -→ 비빈발)  
- 알고리즘 : 조인(Join), 가지치기(Pruning)

## [인공지능] 빈발패턴성장 알고리즘(FP-Growth, Frequent Pattern)



**[정의]**

- 분석해야 할 데이터가 증가하면서, 선험적 규칙(Apriori) 알고리즘의 연산 속도를 개선한, 트리(Tree) 구조 기반의 연관규칙 알고리즘(빈발 패턴 집합 탐색)  
- Apriori + 연산속도향상  
-→ 3,4단락에 쓰자

**[핵심/키워드]**

&lt;특징&gt;  
- Apriori보다 빠름, 데이터를 압축하여 저장 → FP-Tree를 사용, 대규모 데이터셋에 활용  
- 중복된 트랜잭션을 하나의 트리 경로로 결합

&lt;도출 과정&gt;  
최소 지지도 기반 품목 선택 → 빈도 수 기반 정렬 → FP-Tree생성 → 트리 시작 및 확장 → 빈발품목 집합 도출

## [인공지능] CART(Classification And Regression Tree)



**[정의]**

- 지니지수와 분산감소량을 사용하여 의사결정 트리를 분할하는 알고리즘  
- 분류트리(범주형)와 회귀트리(연속형) 모두 사용 가능

**[핵심/키워드]**

&lt; 특징 &gt;  
- 분류트리(범주형)와 회귀트리(연속형) 모두 사용 가능  
- 이진 분할, 지니 지수·분산감소량 기반 최적 분할, 비용복잡도 가지치기를 통한 과적합 방지

* 의사결정나무 형성 과정: 변성가타분  
1) 변수선택: 종속변수와 관계있는 독립변수 선택  
2) 의사결정나무 형성: 분석목적과 자료의 구조에 따라 적절한 분리기준과 정지규칙을 정하여 의사결정나무 구조 작성  
3) 가지치기: 부적절한 가지제거  
4) 타당성 평가: 이익, 위험, 비용 등을 고려하여 모델 평가  
5) 분류 및 예측: 분류 및 예측 수행

* 마디 분리 기준  
- 불순도: 다양한 범주들의 개체들이 얼마나 포함되어 있는가  
- 순수도: 목표변수의 특정 범주에 개체들이 포함되어 있는 정도

* 재귀적 분할 알고리즘  
ID3, CHAID, CART, C4.5/C5.0

## [인공지능] 지니지수



**[정의]**

­- 노드 내 서로 다른 클래스가 혼재되어 있는 정도,즉 불순도(Impurity) 측정

­- 지니지수가 0에 가까울수록 순수도가 높은 노드  
­- 지니지수가 클수록 클래스 간 이질성·불순도가 높은 상태  
­- 이진분류에서는 클래스 비율이 0.5:0.5일 때 Gini=0.5로 최대 불순도  
­- 분할 시 자식 노드의 가중평균 지니 불순도가 최소화되는 분할 선택

<img src="data:image/png;base64,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" alt="embedded_DR_29_Def_img_1.png" style="max-width: 100%; height: auto; margin: 4px 0 12px 0;" />

## [인공지능] 선형회귀분석



**[정의]**

하나 이상의 독립변수(X)와 종속변수(Y) 간의 관계를 직선 형태로 추정하여 설명하고 예측하는 통계 분석 기법

**[핵심/키워드]**

&lt;회귀식&gt;  
Y = β₀ + β₁X₁ + ε₁

Y  = 종속변수 (예측하고 싶은 값)  
β₀ = 절편 (X=0일 때 Y값, 직선이 Y축과 만나는 점)  
β₁ = 기울기 (X가 1 증가할 때 Y 변화량)  
X₁ = 독립변수 (입력값)  
ε₁ = 오차항 (실제값 - 예측값)

&lt;선형 회귀의 평가방법&gt;  
* 오차 평가  
1) MAE (Mean Absolute Error)  
- 수식: (1/n) Σ|yi - ŷi|  
- 실제값과 예측값 차이 절대값 합의 평균

2) MAPE (Mean Absolute Percentage Error)  
- 수식: (100%/n) Σ|yi - ŷi| / yi  
- MAE를 퍼센트로 변환한 값

3) MPE (Mean Percentage Error)  
- 수식: (100%/n) Σ(yi - ŷi) / yi  
- MAPE에서 절대값을 제외한 지표

4) MSE (Mean Square Error)  
- 수식: (1/n) Σ(yi - ŷi)²  
- 실제값과 예측값 차이의 제곱 합의 평균

5) RMSE (Root Mean Square Error)  
- 수식: √[(1/n) Σ(yi - ŷi)²]  
- MSE의 제곱근 값  
- 오차를 실제값 단위로 해석

* 적합도 평가  
1) R Square (결정계수)  
- 수식: 1 - SSE/SST = SSR/SST  
- 종속변수의 분산 중에서 독립변수로 설명되는 비율  
- 범위 0 ≤ R² ≤ 1  
2) Adjusted R Square (수정 결정계수)  
- 수식: 1 - [(1-R²) × (n-1) / (n-k-1)]  
- 변수 많아질 때 패널티 반영하여 평가  
- 결정계수의 단점 보완  
- 1에 가까워질수록 설명력 높은 모델

* 유의성 평가  
1) t-검정  
- 개별 회귀계수의 통계적 유의성 평가

## [인공지능] 로지스틱 회귀분석(Logistic Regression)



**[정의]**

- 독립변수 연속형/종속변수 범주형  
- 분석 대상들이 여러 집단으로 나누어진 경우, 독립변수의 선형 결합을 이용하여 개별 관측치가 어느 집단에 속하는지 확률을 계산하는 분류기법

- 종류 : 이항, 다항, 서수

- 최적화: 크로스 엔트로피

**[핵심/키워드]**

&lt;절차&gt;  
1) 확률의 선형 모델 표시  
2) 오즈 적용: 양의 값 무한대 변환  
3) 로짓 적용(연결함수): 음의 값 무한대 변환  
4) 판별함수: 판별함수 수식으로 선형함수 사용  
5) 시그모이드: 0~1사이의 값을 가지는 출력변수로 변환

&lt;로지스틱 회귀분석의 평가 및 검정&gt;  
– 목적 : 비연속형 종속변수의 범주 예측  
– 회귀계수 추정 : 최대가능도추정법(MLE)  
– 회귀계수 유의성 검정 : Wald 통계량  
– 모델 적합성 확인 : 로그우도함수(LL), -2로그우도함수(-2LL), 카이제곱 검정  
– 모델 설명력 확인 : McFadden 의사결정계수(Pseudo R²) 등

## [인공지능] SVM(Support Vector Machine)



**[정의]**

- 데이터 포인트를 고차원 공간에서 분리하는 최적의 결정경계(Decision Boundary)를 찾아주는 지도 학습(Supervised Learning) 알고리즘

**[핵심/키워드]**

- 분류(Classification: SVC) 및 회귀(Regression, SVR)에 사용  
- 최적의 결정 경계(Hyperplane)를 찾는 것이 목표

* 구성요소  
- Margin: 서포트 벡터 사이의 거리(최대화가 목표)  
- Support Vector: 집단 구분 결정직선에서 가장 근거리에 위치하는 벡터  
- Hyper-plane: n차원의 공간의 구분을 위해 결정되는 n-1 평면

* 분류방법  
- 하드마진 분류: 엄격한 분리, 모든 데이터가 마진 바깥쪽에 위치하도록 강제(오분류 허용안함)  
노이즈와 이상치에 매우 민감 <= 사용안하는 이유  
- 소프트마진 분류: 유연한 분리, 일부 데이터가 마진 안쪽에 위치할 수 있도록 허용(오분류 허용)

- 하드 마진과 소프트 마진은 SVM에서 "분류(Classification)"에 사용

&lt;하이퍼 파라미터&gt;  
- C(Regularization Parameter) : C ↑(좁은 마진, 하드 마진), C ↓(넓은 마진, 소프트 마진)  
- 허용 오차 (ξ) : 소프트 마진 허용  
- Epsilon (ε, SVR에서 사용) = 𝜀-Tube (Epsilon-Tube)  
- Kernel(커널 트릭)  
- Gamma (감마, RBF 커널사용)  
- Degree(다항 커널 사용)

## [인공지능] 모델 검증(Model Validation) 및 데이터 분할 기법



**[정의]**

일반화 성능을 높이기 위해, 모델의 성능을 신뢰할 수 있도록 평가하는 과정

**[핵심/키워드]**

* 비복원 추출방식  
- 예비법(Holdout Method): 전체 데이터를 서로 겹치지 않는 데이터 집합으로 비복원 추출  
- 교차검증(Cross Validation): 예비법에서 훈련용과 시험용의 역할을 교차로 함  
- 잭나이프 : 전체 N개 데이터에서 1개 또는 일부 데이터를 제외한 표본을 반복 생성하여 통계량을 재계산. 주로 Bias, Variance, Standard Error 추정에 활용

* 복원 추출방식  
- 부트스트랩(Bootstrap): 훈련용 데이터 복원추출, 겹치는 것은 하나로 간주

모형이 주어진 데이터에 대해서만 높은 성능을 보이는 과대적합 문제를 예방하여 2종 오류 채택 방지

## [인공지능] 잭나이프(Jacknife)  기법



**[정의]**

전체 표본에서 관측값을 하나씩 제외(Leave-One-Out)하여 통계량을 반복 계산함으로써 추정량의 편향(Bias)을 보정하고 분산(Variance)·표준오차를 추정하는 재표본추출 (Resampling) 기법

**[핵심/키워드]**

* 특징  
: Leave-One-Out, 반복 추정, 편향 보정

* 목적  
: 추정량의 편향 감소, 분산과 표준오차 추정

* 절차  
① 원본 추정 → ② 하나씩 제외(Leave-One-Out) → ③ 반복 추정(Resampling) → ④ 잭나이프 평균 → ⑤ 편향·오차 추정 → ⑥ 편향 보정

## [인공지능] 리브원아웃 교차검증(LOOCV)



**[정의]**

- K 값이 데이터 개수(N)와 동일한 상황으로, 각 반복마다 단 하나의 샘플을 검증 데이터로 사용하고, 나머지 N-1개를 훈련 데이터로 사용하는 방식

**[핵심/키워드]**

&lt;특징&gt;  
데이터 활용 극대화, 일반화 성능 평가가 가장 정확함, 연산량이 매우 큼, 과적합 증가

&lt; 동작절차 &gt;  
1. 데이터셋에서 한 개의 샘플을 제외하고 나머지로 모델을 훈련  
2. 제외된 샘플로 모델을 테스트  
3. 이 과정을 데이터셋의 모든 샘플에 대해 반복  
4. 각 반복에서 얻은 성능 지표의 평균을 최종 성능 평가로 사용

## [인공지능] 배깅(Bagging)



**[정의]**

- 여러 개의 동일한 모델(분류기)을 독립적으로 학습한 후, 그 예측 결과를 평균(회귀) 또는 다수결(분류) 방식으로 결합하여 최종 예측을 수행하는 앙상블 방법

**[핵심/키워드]**

&lt;특징&gt;  
- 모델의 분산(Variance)을 줄여 안정적 예측 가능, 병렬 학습 가능, 과적합 방지, 대표알고리즘 : 랜덤포레스트  
- 부트스트랩=복원추출(동일한 확률로 복원추출)  
- 같은 모델에 추출된 다른형태의 데이터 적용

## [인공지능] 랜덤포레스트(Random Forest)



**[정의]**

- 입력 특징 조작, Feature Randomize  
- 배깅처럼 데이터를 반복 복원추출을 진행할 뿐만 아니라, 거기에 더해 변수 또한 random하게 추출하여 다양한 모델을 만드는 것

- 부트스트랩을 이용한 데이터의 변화 및 나무모형 분할방법에 랜덤성을 가미하여 나무 모형에 다양성을 갖도록 유도하는 앙상블 기법

**[핵심/키워드]**

&lt; 특징 &gt;  
데이터 샘플링 (Bootstrap Sampling)/랜덤한 특성 선택 (Feature Randomness), 특성 중요도 제공

- 완전 다른 모형의 트리를 구성하도록 하는 방식  
- 배깅처럼 데이터를 반복 복원추출 할 뿐만 아니라, 변수 또한 랜덤하게 추출하여 다양한 모델을 만듬  
- 훈련집합을 만들기 위해 입력 특징들 중 일부분을 선택

## [인공지능] 스태킹(Stacking)



**[정의]**

- bagging과 boosting과는 달리 서로 다른 타입의 모델들을 결합하는 앙상블 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;  
- 서로 다른 타입의 모델들을 결합(취합이 아닌 학습)  
- 예측기가 예측들을 입력으로 받아 최종 예측 생성  
- voting 대신 Meta learner사용  
- 개별 학습시 K-Fold 교차검증 사용

&lt;구성요소&gt;  
- 기본 학습기 (Base Models) : 개별적으로 학습하는 여러 모델 (예: 랜덤 포레스트, SVM, 로지스틱 회귀 등)  
- 메타 모델(Meta Model): 기본 학습기의 예측 결과를 입력으로 받아 최종 예측 수행

## [인공지능] 혼동행렬(Confusion Matrix), 오분류표



**[정의]**

분류 모델의 성능을 평가하는 데 사용되는 중요한 도구

**[핵심/키워드]**

정확도(Accuracy): (TP + TN) / (TP + TN + FP + FN)  
정밀도(Precision): TP / (TP + FP)  
재현율(Recall): TP / (TP + FN)  
특이도(Specificity): TN / (TN + FP)

## [인공지능] PR 커브(Precision-Recall Curve, 정밀도-재현율 곡선)



**[정의]**

- 모델의 Precision(정밀도)과 Recall(재현율)의 관계를 나타내는 그래프

**[핵심/키워드]**

- 임계값(Threshold)을 변화시키면서 Precision과 Recall의 변화를 분석

- PR 커브는 양성(positive) 클래스 중심으로 평가  
- 가로 : Recall, 세로 : Precision  
- AUC (mAP, Mean Average Precision): PR 커브 아래 영역의 면적  
 ==> 1이면 좋은 모델

## [인공지능] ROC Curve



**[정의]**

이진 분류 모델의 성능을 평가하는 데 사용되는 그래프

**[핵심/키워드]**

TPR(민감도=정밀도): TP/전체 P  
FPR(1-특이도): 1- TN/전체 N  
AUC: ROC 커브 밑면적 값. 1에 가까울수록 성능이 좋음  
==> 곡선이 왼쪽 상단에 가까울수록 모델의 성능이 우수

## [인공지능] 회귀모델 평가



**[정의]**

예측값과 실제값의 차이를 다양한 오차 지표로 측정하여 모델의 설명력과 일반화 성능을 검증하는 과정

**[핵심/키워드]**

* 평가 항목  
AE : 평균오차  
MAE : 평균 절대 오차  
MAPE : 평균 절대 백분율 오차  
MPE : 평균 백분율 오차  
MSE : 평균 제곱 오차  
RMSE : 평균 제곱근 오차

## [인공지능] 강화학습



**[정의]**

- 데이터의 상태를 인식하고 이에 반응한 행위에 대하여 환경으로부터 받는 보상(Reward)을 학습하여 행위에 대한 보상을 최적화하는 정책을 찾는 기계학습  
- 반복적인 결정 및 착오와 경험에 기반하여 상태의 최적 행동을 조금씩 학습하는 알고리즘

**[핵심/키워드]**

* 강화학습 수행절차  
1) Agent와 환경과의 상호작용을 통해서 행동을 결정  
2) 반복적인 결정의 반복으로 최적의 행동으로 개선  
3) 최적 행동을 통한 Action 결정

&lt;구성요소&gt;  
- 에이전트 (Agent)  
- 환경 (Environment)  
- 상태 (State, s)  
- 행동 (Action, a)  
- 보상 (Reward, r)  
- 정책 (Policy, π)

&lt;유형&gt;  
1) Model Free  
- 정책 기반 방법 (Policy-based)- 직접 정책을 최적화하여 최적의 행동을 학습  
- 가치 기반 방법 (Value-based)- Q-러닝(Q-Learning)처럼 가치 함수를 학습하여 최적 행동 선택  
2) Mode Based  
- 모델 기반 방법 (Model-based)- 환경의 동적 모델을 학습하여 최적의 행동 결정  
3) Model-Free + Model-Based (혼합형)

<데이터를 학습하는 방식에 따른 분류 ‘On-Policy vs Off-Policy’>
- Model-Free RL(모델 없이 학습)에 적용  
- On-Policy : 현재 실행 중인 정책(Policy)을 사용하여 학습  
- Off-Policy : 과거 경험 데이터를  재사용하여 학습 (Replay Buffer 사용)

## [인공지능] 정책 그래디언트(Policy Gradient, PG)



**[정의]**

- 강화학습에서 정책(Policy)을 직접 최적화하는 기법  
- 에이전트가 상태(State)에서 행동(Action)을 선택하는 확률을 학습하여 최적의 정책을 찾아가는 방식

**[핵심/키워드]**

&lt;특징&gt;  
- 상태 S에서 행동 A를 선택하는 확률을 직접 학습  
- 확률적 정책(Stochastic Policy) : 행동 선택을 확률적으로 수행하여 탐색(결정적 정책도 사용가능)  
- 현재 실행 중인 정책(Policy)을 그대로 학습  
- Q-Learning과 달리 연속적인 행동(Continuous Action Space)에서도 사용  
 - 보상을 최대화하는 방향으로 정책을 업데이트

&lt;학습과정&gt;  
- 정책 파라미터화 → 샘플 수집 → 누적보상 계산 → 정책그레디언트 계산 → 정책파라미터 업데이트 → 수렴

&lt;정책 그래디언트 대표 알고리즘&gt;  
- REINFORCE(Monte Carlo Policy Gradient)  
- Actor-Critic  
- PPO(Proximal Policy Optimization)  
- DDPG(Deep Deterministic Policy Gradient)

## [인공지능] REINFORCE (Monte Carlo Policy Gradient)



**[정의]**

- Monte Carlo 방식을 사용하여 완전한 에피소드 후 기대값을 최대화하는 방향으로 정책을 업데이트하는 정책 그래디언트 기반의 강화 학습 알고리즘

**[핵심/키워드]**

&lt;특징&gt;  
 - 정책기반 학습(Value Function 없음), 확률적 정책(Stochastic Policy), On-Policy 방식, Variance(분산) 큼:수렴속도 느림  
 - 에피소드 단위 업데이트(Monte Carlo 방식): 전체 에피소드(시작 → 종료까지의 모든 단계) 를 완료한 후 보상

&lt;학습과정&gt;  
- 데이터 수집(Monte Carlo 방식) → 누적보상 계산 → 정책 그래디언트 계산 → 정책 업데이트 → 반복

## [인공지능] PPO(Proximal Policy Optimization, 근접 정책 최적화, PPO-Clip)



**[정의]**

- 신뢰 영역 정책 최적화(TRPO)의 단점을 보완하여, 신뢰 구간(Proximal Bound) 내에서 정책을 안정적으로 업데이트하는 강화학습 알고리즘

**[핵심/키워드]**

&lt;특징&gt;  
- 신뢰 구간(Proximal Bound)  
- 클리핑 기법(Clipping Objective) : 특정 값 이상으로 변화하는 요소를 제한하는 방법  
- 가치함수 업데이트 활용

&lt;학습과정&gt;  
1️⃣ 환경과 상호작용 데이터 수집  
2️⃣ 어드밴티지 계산  
3️⃣ 정책 업데이트(클리핑 적용)  
4️⃣ 가치 함수 업데이트  
5️⃣ 엔트로피 보상 추가  
6️⃣ 수렴(최적화 및 반복)

## [인공지능] 심층Q네트워크 - DQN(Deep Q-Network)



**[정의]**

- Q-러닝의 과대평가 한계를 극복한, 딥러닝으로 확장하여 뉴럴 네트워크를 사용해 Q-값을 근사하는 알고리즘

**[핵심/키워드]**

&lt;특징&gt;  
 - Replay Buffer(경험 재현)를 활용하여 학습 효율 향상  
 - Target Network(타겟 네트워크)를 사용하여 학습 안정성 증가  
 - Epsilon-Greedy 탐색 전략을 활용하여 최적의 정책 학습

* 핵심요소  
- Q-네트워크 (Q-Network) - 딥러닝 활용하여 Q-값 근사  
- Replay Buffer(재현 메모리) - 과거 경험 저장. 학습 안정성 향상  
- Target Network - 일정 간격마다 업데이트. 학습 안정성 증가  
- Epsilon-Greedy 탐색 - Q-Value기반 행동 선택. 탐색과 활용 균형 조절  
- CNN(Convolutional Neural Network) - 고차원 이미지 입력처리  
- 손실 함수 (Loss Function) - TD손실(Temporal Difference Loss)사용

&lt; 학습과정&gt;  
1️⃣ 초기화  
2️⃣ 경험 저장  
3️⃣ 환경과 상호작용  
4️⃣ Replay Buffer 저장  
5️⃣ Mini-batch 학습  
6️⃣ Q-값 업데이트  
7️⃣ Target Network 업데이트  
8️⃣ 반복 학습

## [인공지능] SARSA(State-Action-Reward-State-Action, "상태-행동-보상-상태-행동" 알고리즘)



**[정의]**

- 에이전트가 현재 상태에서 행동을 선택하고, 환경의 반응(보상)을 받은 후, 다음 상태에서 또 다른 행동을 선택하며 학습하는 방법

**[핵심/키워드]**

&lt;특징&gt;  
- Model-Free, Value-Based, On-Policy 강화학습

&lt; 학습과정&gt;  
1️⃣ 현재 상태(S)  
2️⃣ 행동 선택(A)  
3️⃣ 환경 반응 및 보상(R)  
4️⃣ 다음 상태(S')  
5️⃣ 다음 행동 선택(A')  
6️⃣ Q-값 업데이트  
7️⃣ 반복 학습

&lt;개선 알고리즘&gt;  
- Expected SARSA, Double SARSA

## [인공지능] 강화학습 평가 지표



**[정의]**

에이전트가 학습한 정책이 환경에서 얼마나 높은 장기 누적보상을 안정적·효율적·안전하게 달성하는지를 측정하는 기준

**[핵심/키워드]**

* 평가 지표  
보상 기반 평가  
- 총 누적 보상 (Total Reward, Return)  
- 평균 에피소드 보상(Average Episode Reward)  
- 할인된 총 보상 (Discounted Return)

정책 성능 평가  
- 성공률 (Success Rate)  
- 에피소드 길이 (Episode Length)

샘플 효율성  
- 학습 속도 (Learning Efficiency)  
- 샘플 효율성 (Sample Efficiency)

일반화 성능  
- 환경 적응성 (Generalization to New Environments)

안정성 평가  
- 정책의 일관성 (Policy Stability)  
- 분산 (Variance of Performance)  
계산 자원 효율성  
- 학습 시간 (Training Time)  
- 메모리 사용량 (Memory Usage)

## [인공지능] 파라미터 최적화



**[정의]**

- 계산된 실제값과 예측값의 차이인 오차(Error)를 학습 알고리즘(Learning Algorithm)을 이용하여 반복적으로 파라미터값을 조정하면서 모델을 최적화하는 과정

**[핵심/키워드]**

학습율 조정, 모델이 학습 통해 찾는 가중치  
최적화 기법: 확률적 경사하강법, 모멘텀, 아담, 아다그라드, RMSProp

## [인공지능] 아담(Adam)



**[정의]**

- 모멘텀(Momentum)과 RMSprop을 결합하여 만든 최적화 알고리즘  
- 학습률을 자동 조정하면서 빠르고 안정적으로 최적값을 찾는 경사 하강법

**[핵심/키워드]**

- Adam = 모멘텀 + RMSprop → 빠르고 안정적인 최적화 가능  
- 모멘텀(Momentum) → 속도를 고려하여 빠르게 이동  
- RMSprop → 학습률을 매개변수별로 자동 조정

## [인공지능] 하이퍼파라미터 최적화(Hyperparameter Optimization)



**[정의]**

머신러닝 모델의 성능을 극대화하기 위해 학습 전에 설정하는 하이퍼파라미터의 최적 조합을 탐색하는 기법

**[핵심/키워드]**

* 하이퍼파라미터 정의  
- 사람이 모델에 조정해주는 값  
- knn, k-means의 k값, 트리깊이, learningRate 등  
- 모든 기계학습 모델들은 저마다의 하이퍼파라미터를 갖고 있고, 그 값에 따라 성능 차이 발생

&lt; 최적화 기법 &gt;  
1) 블랙박스 최적화  
: 하이퍼 파라미터의 성능을 직접 평가하며 탐색하는 방식  
- Grid Search(격자 탐색), Random Search(랜덤 탐색), 베이지안 최적화, 시뮬레이티드 어닐링, 유전 알고리즘

2) 다중 충실도 최적화  
: 일부 데이터나 모델을 사용하여 성능을 예측하고 효율적으로 탐색하는 방식  
- Modeling Learning Curve(학습 곡선 모델링), Bandit Based(밴딧 기반 탐색), Successive Having(순차적 절반 선택), Hyper-Band(하이퍼밴드 알고리즘)

## [인공지능] 경사하강법(Gradient Descent Method)



**[정의]**

- 함수의 최소값의 위치를 찾기 위해 경사가 하강하는 방향을 관찰하고 그 쪽으로 조금씩 이동해가면서 검토를 반복하는 기법

**[핵심/키워드]**

&lt; 경사하강법 절차 &gt;  
1) 먼저 변수의 초기값을 선정  
2) 변수값에 해당하는 함수의 경사도 계산  
3) 변수를 검사방향으로 움직여 다음 숫자값으로 설정  
4) 1~3을 반복하여 함수의 최소값이 되는 변수값으로 근접해 나감

&lt; 경사하강법 종류 &gt;  
- 배치 경사하강법: 모든 데이터를 학습하고 오차를 이용하여 가중치 갱신 값을 계산한 다음, 가중치를 한번에 갱신  
- 확률적 경사하강법: 하나의 학습 데이터마다 오차를 계산해서 신경망의 가중치를 바로 조절  
- 미니배치 경사하강법: 훈련데이터에서 소량의 데이터를 적당히 선택해 학습 후 갱신 처리를 수행

&lt; 수식 구성요소 &gt;  
변수x: 각 연결의 weight  
함수f: 훈련데이터의 훈련 결과와 실제값의 차이를 제곱해서 더한 값 반복  
함수의 경사  
움직임의 정도(엡실론): 학습률

## [인공지능] 활성화 함수(Activation Function)



**[정의]**

- 시냅스의 전기 신호 전달을 모방하여, 세타에 따라 출력값을 조정 및 다음 노드로 전달하는 함수  
- 각 노드값의 출력을 제한하는 함수

**[핵심/키워드]**

항경계시  
- 항등함수: 입력값이 그대로 출력  
- 경사함수: 0보다 작은값은 0(ReLU)  
- 계단함수: -1, 0, 1 값으로만 출력  
- 시그모이드 함수: 0~1 사이값 출력

- tanh: -1~1 사이 값 출력  
- 시그모이드 함수: 0~1사이 출력  
- ReLU: 0보다 작은건 0  
- Parametric ReLU: 음수에 작은 경사값 설정  
- Leaky ReLU: Max(0.01x, x)  
- Swish β(x)=x⋅σ(βx)  
- SiLU(x)=x⋅σ(x)

- Swish : x⋅σ(βx)로 입력값과 Sigmoid 함수값을 곱한 매끄러운 비단조 활성화 함수  
- SiLU : x⋅σ(x)로 정의되는 Sigmoid Linear Unit. β = 1인 Swish. Mamba(맘바) 등 에서 사용

## [인공지능] CNN(Convolution Neural Network)



**[정의]**

- 시각인지 연구를 기초로 인공신경망에 필터링 기법을 적용한 것으로 이미지 같은 2차원 데이터를 분석하는 심층신경망  
알고리즘  
- 이미지 및 공간적 구조를 가진 데이터 처리에 특화된 신경망  
- 합성곱(Convolution)연산을 이용하여 이미지 특징을 추출하고,학습하는 방식

**[핵심/키워드]**

&lt; 특징 &gt;  
- 공간적 관계 학습, 파라미터 효율성(가중치 공유), 국소 수용 영역(작은 영역 특징 추출), 계층적 특징 추출

&lt; 구성요소 &gt;  
① 컨볼루션 레이어(Convolution Layer ): 이미지 특징 추출  
ㄴ 핵심요소 : 커널, 스트라이드, 패딩

② 풀링 레이어(Pooling Layer) : 특징 맵 크기 감소(차원 축소)  
ㄴ 핵심요소 : 윈도우 크기, 스트라이드(이동 간격)  
ㄴ 풀링 유형  
- 최대 풀링(Max Pooling):윈도우 내 최대값 선택 (가장 두드러진 특징 유지)  
- 평균 풀링(Average Pooling):윈도우 내 평균값 선택 (전체적인 정보 유지)  
- 확률 풀링 (Stochastic Pooling) : 값의 크기에 따라 확률적 선택(작은 특징도 반영 가능)

③ 완전 연결 레이어(Fully Connected Layer) :  특징 기반 최종 분류/예측 수행  
ㄴ 핵심요소 : Flatten Layer, Dense Layer, 활성화함수(ReLU, Softmax, Sigmoid)

&lt; CNN 개선 알고리즘 &gt;  
- ResNet, DenseNet, EfficientNet, Capsule Network, SENet

## [인공지능] RNN(Recurrent Neural Network)



**[정의]**

- 연속된 데이터 상에서 이전 순서의 히든 노드(Hidden Node)의 값을 저장한 후,다음 순서의 입력 데이터로 학습할 때 이전에 저장해 놓은 값을 이용하는 알고리즘  
- 시퀀스 데이터(Sequence Data)를 다룰 수 있도록 인공신경망을 구성하는 유닛 사이의 연결이 Directed Cycle을 구성하는 신경망

**[핵심/키워드]**

- 특징 : 시간 의존성 고려, 가변 길이 입력 처리 가능, 순차적 데이터 학습(이전 데이터 메모리 저장)

- BTPP(Backpropagation Through Time)을 이용하여 시간에 따라 역전파 수행 후 가중치 업데이트  
- RNN의 기울기의 사라짐 문제 발생 (장기 의존성 문제) → 정보 손실  
→ LSTM, GRU, Transfomer로 해결 가능

## [인공지능] LSTM(Long Short Term Memory)



**[정의]**

- RNN의 장기 의존성 문제(Long-Term Dependency)를 해결하기 위해 게이트(Gate)구조를 활용하여 정보 흐름을 조절하여 중요한 정보는 기억하고, 불필요한 정보는 제거할 수 있는 신경망

**[핵심/키워드]**

- 장기간의 시퀀스 학습하는 데 유리  
- 자연어 처리(NLP),음성 인식,시계열 예측 등에 활용  
- LSTM의 핵심 : 셀 상태(Cell State) 유지, 게이트(Gate) 메커니즘  통해 정보 흐름 조절

&lt; 구성요소 &gt;  
- Cell State: 장기 정보 저장 메모리  
- Forget Gate: 버릴지 유지할지 결정  
- Input Gate: 어떤값 갱신할지 결정  
- Output Gate : Cell State 갱신 후 출력 결정

## [인공지능] DBN(Deep Belief Network)



**[정의]**

- 심층 신뢰망  
- 입력층과 출력층으로만 구성되어 있는 RBM(제한된 볼츠만 머신)을 층층이 쌓아 학습하는 딥러닝 기법  
- 초기 가중치 정확성 향상, 선행학습에 활용

**[핵심/키워드]**

1) visible layer와 hidden layer1을 하나의 RBM으로 생각하고 RBM 학습  
2) 학습이 종료되면 hidden layer1의 값을 새로운 입력으로 하여 hidden layer1과 2를 RBM으로 학습함  
3) 단계적으로 마지막층까지 학습하여 결과 얻음

## [인공지능] Word2Vec



**[정의]**

- 의미기반 워드 임베딩 기법  
- 단어자체가 가지는 의미를 다차원 공간에서 벡터화하는 인공신경망 알고리즘

**[핵심/키워드]**

* 유형  
- CBOW: 주변 단어가 만드는 맥락을 이용해 타겟 단어를 예측(Continuous Bag of words)  
- Skip-gram: 한 단어를 기준으로 주변에 올 수 있는 단어를 예측

## [인공지능] VAE(Variational Auto Encoder)



**[정의]**

- 입력 데이터를 확률적 잠재 공간에서 학습하여 새로운 데이터를 생성하는 신경망 알고리즘

**[핵심/키워드]**

* 아키텍처  
입력층(Input Layer) : 원본 데이터 x가 입력됨  
인코더(Encoder) : 입력 데이터를 저차원 잠재공간으로 압축  
잠재변수(Latent Variables, z) : 평균 μ와 표준편차 σ로 표현되는 확률분포  
샘플링(Sampling) : 정규분포에서 ϵ을 샘플링하여 z=μ+σ⋅ϵ으로 변환  
디코더(Decoder) : 샘플링된 z를 원래 데이터 형태로 복원  
출력층(Output Layer) : 재구성된 데이터 x^가 출력됨  
손실 계산(Loss Calculation) : 재구성 손실(MSE, BCE)과 KL 발산 손실을 합쳐 최적화 수행  
모델 업데이트 : 역전파를 통해 인코더와 디코더의 가중치를 업데이트

* 기술요소  
잠재공간 : 데이터의 특징을 확률분포 형태로 변환하여 매핑  
변분추론 : 복잡한 사후분포를 단순한 분포로 근사하여 학습하는 확률적 방법  
재매개변수화 트릭(Reparameterization Trick) : 확률적 샘플링 과정을 미분 가능한 형태로 변환  
KL 발산(KL-Divergence) :  잠재변수 z의 분포가 표준정규분포를 따르도록 제약  
ELBO(Evidence Lower Bound): 데이터 로그 가능도의 하한으로, 재구성 성능과 잠재분포 정규화를 함께 최적화  
재구성 손실(Reconstruction Loss) : 원본 데이터 x와 복원 데이터 x^ 간의 차이를 최소화

## [인공지능] SNN(Spiking Neural Network)



**[정의]**

- 뇌의 뉴런이 시간에 따라 이산적인 전기적 스파이크(펄스)를 발생시키는 생물학적 신경 활동을 모사한 신경망 모델

**[핵심/키워드]**

&lt;특징&gt;  
- 3세대 신경망. 에너지 효율성 높음. 생물학적 학습 규칙 STDP(Spike-Timing-Dependent Platicity) 활용

&lt; 학습과정 &gt;  
1️⃣ 뉴런 활성화 : 전위(Potential) 누적. 임계값 초과 시 스파이크 발생  
2️⃣ 스파이크 전파 및 누적 : 입력 인코딩 층 → 스파이킹 뉴런 층  
3️⃣ 학습규칙 적용 : Winner-Take-All 메커니즘 적용. STDP 학습규칙  적용  
4️⃣ 출력 스파이크 패턴 분석 : Rate Coding, Temporal Coding

&lt; 구성요소 &gt;  
- Input 계층 : Input Spike, Synapse(스파이크 전송), Weight(가중치 조정)  
- Hidden 계층 : Neuron  
- Output 계층 : Output Spike

&lt; 활용분야 &gt;  
- 신경과학 연구, 저전력 AI 칩 → 뉴로모픽 컴퓨팅(IBM TrueNorth,Intel Loihi) 및 IoT  
- 로보틱스, 자율주행, 뇌-컴퓨터 인터페이스(BCI) → EEG 뇌파 분석

## [인공지능] GEO(Generative Engine Optimization)



**[정의]**

생성형 AI가 사용자 답변에 컨텐츠를 직접 인용 ·활용되도록 최적화하는 전략

**[핵심/키워드]**

&lt;기술요소&gt;  
- 콘텐츠 청킹  
- 임베딩 최적화  
- RAG 대응 : 검색+생성 결합 구조  
- 지식그래프 :브랜드, 제품, 서비스를 엔티티로 연결해 AI가 관계를 이해하도록 지원  
- E-E-A-T 충족 : 경험, 전문성, 권위, 신뢰를 증명하는 콘텐츠 작성  
- 멀티모달 : 텍스트 및 이미지, 영상, 오디오까지 AI가 인식 가능  
- Semantic Optimization : 문맥, 의미 중심으로 콘텐츠 작성

## [인공지능] Self-Attention



**[정의]**

- 입력 시퀀스 내 모든 단어가 서로의 관계를 학습할 수 있도록 하는 어텐션 메커니즘  
- 같은 문장 내 단어들이 서로를 참고하면서 관계를 학습  
- Transformer의 핵심기술

**[핵심/키워드]**

&lt;특징&gt;  
- Query-Key-Value(Q, K, V) 구조  
- 장기 의존성 문제 해결 : 멀리 떨어진 단어 간 관계도 학습 가능  
- 병렬 연산 가능(RNN은 불가)

&lt;핵심요소&gt;  
- Query(Q), Key(K), Value(V)  
- 어텐션 분포 (Attention Distribution) : Query와 Key의 유사도를 Softmax로 정규화한 확률 값  
- 어텐션 값 (AttentionValue) :  어텐션 분포를 이용해 Value벡터를 가중합한 최종 출력 값  
- Scaled Dot-Product Attention : Query와 Key간의 내적을 기반으로 가중치 계산하는 방식

&lt;알고리즘&gt;  
1️⃣ Query,Key,Value 생성 - 입력 문장의 각 단어를 Q,K,V벡터로 변환  
2️⃣ Query-Key유사도 계산  
3️⃣ Softmax 적용 (어텐션 분포 생성)  
4️⃣ Value가중합 (어텐션 값 생성)  
5️⃣ 최종 출력 반환

## [인공지능] Transformer



**[정의]**

- RNN을 제거하고 Self-Attention을 활용하여 문맥을 학습하는 신경망 기반의 자연어 처리(NLP)모델

**[핵심/키워드]**

&lt; 특징 &gt;  
- RNN없이 병렬 연산 가능, Self-Attention만 사용, Encoder-Decoder구조  
- GPT,BERT,T5등 최신 NLP모델의 기반이 되는 핵심 모델

* 레이어별 주요 기술요소  
[인코더/디코더]  
- Self-Attention  
- Multi-Head Attention  
- Positional Encoding:  
- Residual Connection & Layer Normalization

[디코더]  
- Encoder-Decoder Attention, Cross-Attention, Masked Self-Attention

## [인공지능] 인공지능 거버넌스(Governance)



**[정의]**

- AI 시스템의 개발과 활용에 있어 안전성, 신뢰성, 윤리성을 확보하기 위한 프레임워크

**[핵심/키워드]**

&lt;주요 구성요소&gt;  
- 정책 및 원칙 수립  
- 책임과 투명성  
- 위험 관리  
- 규제 준수  
- 지속적인 모니터링 및 평가

## [인공지능] AI  TRiSM



**[정의]**

- AI 모델에 대한 거버넌스, 신뢰성, 공정성, 효율성, 개인정보 보호, 데이터 보호 및 신뢰성을 지원하고 가능하게 하는 프레임워크  
- AI TRiSM은 AI 모델의 보안성 확보 위한 프레임워크 정의

**[핵심/키워드]**

* TriSM 의미  
인공지능 신뢰(AI Trust)  
인공지능 위험성(AI Risk)  
인공지능 보안(AI Security)

* 5가지 기본요소  
설명가능성(Explainability),모델옵스( ModekOps), 데이터 이상탐지(Data Anomaly Detection), 적대적 공격 복원력(Adversarial Attack Resistance), 데이터 보호(Data Protection)

* 관리 시스템  
: AI 시스템, Agent

## [인공지능] AI Risk



**[정의]**

- 인공지능의 개발·활용·관리 전 과정에서 발생할 수 있는 잠재적 손실이나 부정적 결과  
- AI 시스템의 개발·학습·배포·운영 과정에서 개인,조직,사회에 부정적 영향을 줄 수 있는 불확실성 또는 위험

**[핵심/키워드]**

&lt; AI 보안 리스크 &gt;  
* 정의 : 인공지능(AI) 시스템을 개발, 학습 및 운영하는 과정에서 발생하는 취약점을 악용한 공격이나 오작동으로 인해 데이터 유출, 시스템 무결성 훼손 등이 발생하는 위험  
* 유형 : 모델 탈취, 적대적 공격, 모델 포이즈닝 , 과적합 취약성 , 프롬프트 인젝션, 데이터 유출  
* 대응방안  
- Query rate limiting,출력값 최소화,워터마킹  
- Adversarial training,입력 정규화  
- 데이터 정제,이상치 탐지,무결성 검증  
- Regularization, Dropout, 교차 검증

&lt; AI 프라이버시 리스크 &gt;  
* 정의 : AI 시스템이 방대한 데이터를 수집, 학습, 활용하는 과정에서 개인의 프라이버시 권리를 침해하는 리스크  
* 유형 : 학습 데이터 출처 검증 미흡, 데이터 관리 체계 미흡, 불필요한 개인 정보 유입, 서비스 목적 외 개인 정보 과노출  
* 대응방안  
- 학습데이터 출처·이력관리 , 적법성 검증  
- 안전한 보관·파기 방안 마련 및 시행  
- 개인 정보 최소 수집, 비식별·가명 처리,전 처리 강화

&lt; AI 사회적 리스크 &gt;  
* 정의 : AI 기술이 인류의 민주주의, 고용 환경, 인간관계 등에 구조적인 부작용을 낳는 리스크  
* 유형 : 정보 자기 결정권 침해, 개인정보 삭제권 행사 불가, 알고리즘 편향, 디지털 격차 심화, 신규 일자리 창출 불균형  
* 대응 방안  
- 개인정보 보호 강화, 동의·통제권 보장  
- 삭제권 실질 보장, 데이터 관리 책임 강화  
- 알고리즘 편향성 평가 및 개선

## [인공지능] 인공지능 데이터 품질표준안



**[정의]**

- 데이터 댐 성공구축 지원  
- 데이터 댐의 핵심자원인 인공지능 데이터 관련 품질의 개념과 범위, 세부 요구사항 등을 정립한 표준안을 개발하는 과학정보통신부 주도의 정책

- 인공지능 데이터 품질: 인공지능 기술에 활용되는 데이터가 다양성, 정확성, 유효성 등을 확보하여 사용자에게 유용한 가치를 줄 수 있는 수준

**[핵심/키워드]**

* 주요 품질 요구사항  
[ 데이터 요구사항 ]  
- 원시 데이터 품질: 기준적합성, 기술적합성  
- 데이터 라벨링 품질: 라벨링 정확성  
- 인공지능 활용 품질: 유효성  
[ 구축절차 요구사항 ]  
- 획득: 법/제도 준수, 획득 환경/대상  
- 정제: 정제 기준, 비식별화, 중복방지  
- 가공(라벨링): 라벨링 포멧, 도구 및 작업 방식  
- 품질검수:  검수 기준 및 방법

## [인공지능] ISO/IEC TR 29119-11



**[정의]**

- AI기반 시스템 테스팅 가이드  
- AI 기반 시스템을 도입하고 테스트하는 방법에 대한 지침을 제공하는 ISO/IEC의 기술 보고서(Technical Report)

- 29119 소프트웨어 테스트 표준과 연계, 데이터 학습 과정, 모델의 의사결정 로직, 성능 평가 방법

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

## [인공지능] AI 기반시스템의 블랙박스 테스트



**[정의]**

- AI 모델의 내부 구조나 학습 과정(알고리즘, 코드)을 알지 못한 상태에서 입력과 출력을 기반으로 성능과 신뢰성을  
검증하는 테스트 방법

**[핵심/키워드]**

* 테스트 기법  
- 조합 테스트(Combinatorial Testing)  
· 다양한 입력 조합을 생성하여 AI 모델의 응답을 평가하는 기법  
· 테스트 케이스를 최소화하면서도 중요한 조합을 포함

- 백투백 테스트(Back-to-Back Testing)  
· 서로 다른 버전의 AI 모델 또는 기존 전통적 시스템과 비교하여 성능을 평가하는 방법  
· 새로운 AI 모델의 성능이 기존 모델보다 향상되었는지 검증 가능

- A/B 테스트(A/B Testing)  
· 두 가지 이상의 모델을 실제 사용자에게 제공하고, 피드백과 성과지표를 통해 어느 모델이 더 우수한지 평가

- 변성 테스트(Metamorphic Testing)  
· AI 모델이 일관된 논리적 변환을 유지하는지 검증하는 기법  
· 특정 입력을 변경했을 때 예상되는 입·출력 관계인 메타모픽 관계가 유지되는지 확인

## [인공지능] 변성 테스트 (Metamorphic Testing, 메타몰픽 테스트)



**[정의]**

-정답 자체 검증 대신, 입력을 일정한 규칙으로 변형했을 때 출력간에 성립해야 하는 관계 (Metamorphic Relation)를 검증하는 테스트 기법

-특정 입력을 변경했을 때 예상되는 결과가 유지되는 지 확인(입/출력관계)하는 테스트 기법

**[핵심/키워드]**

* 구성요소  
Source Test Case : 최초 실행하는 테스트 케이스  
Metamorphic Relation : 입력 변화에 따른 결과가 가져야할 기대 관계  
Follow-up Test Case : Source Test Case를 변환해 생성한 후속 케이스  
Result Verification : Source와 Follow-up 결과가 MR을 만족하는 지 비교·판정

* 메타몰픽 관계  
입력 변환 관계 , 출력 불변 관계 , 출력 등가 관계, 단조 관계, 비례 관계, 관계 위반

* 메타몰픽 테스트 절차  
1. 변성관계 구축  
2. 변성관계 리뷰  
3. 소스 테스트케이스 생성  
4. 후속 테스트케이스 생성  
5. 변성 테스트케이스 실행

## [인공지능] 신경망의 화이트 박스 테스트



**[정의]**

- AI 모델의 내부 구조, 신경망의 동작 방식, 코드 및 알고리즘을 직접 분석하여 성능과 신뢰성을 검증하는 테스트 방법

 - 뉴런 활성화, 임계값 변화, 가중치 업데이트 등의 내부 동작을 면밀히 분석하여 신뢰성을 평가

**[핵심/키워드]**

* 테스트 기법  
- 뉴런 커버리지  
· 신경망 내 개별 뉴런(노드)이 활성화되는 범위를 측정  
· 활성화된 뉴런 수를 신경망의 전체 뉴런 수로 나눈 비율

- 임계점 커버리지  
· 뉴런이 특정 임계값을 초과하여 활성화되는 빈도를 측정  
· 임계 활성값을 초과하는 뉴런 수를 신경망의 전체 뉴런 수로 나눈 비율

- 부호 변경 커버리지  
· 뉴런의 활성값이 음수에서 양수 또는 양수에서 음수로 변경되는 비율 측정  
· 활성값의 부호가 변경된 뉴런 수를 신경망의 전체 뉴런 수로 나눈 비율

- 값 변경 커버리지  
· 뉴런의 활성값이 얼마나 자주 변하는지를 평가  
· 정해진 범위보다 활성값이 크게 바뀐 뉴런 수를 신경망의 전체 뉴런 수로 나눈 비율

- 부호-부호 커버리지  
· 연속적인 뉴런 간의 부호 변경 패턴을 분석  
· 변경 조건·결정 커버리지(MC/DC)와 유사

- 레이어 커버리지  
· 신경망의 특정 레이어에서 활성화되는 뉴런의 범위를 측정  
· 신경망 전체 층에서 뉴런 세트에 대한 활성값이 어떻게 변경되는지 확인

## [인공지능] 데이터 어노테이션(Data Annotation)



**[정의]**

- 머신러닝/딥러닝 모델 학습을 위해 데이터에 의미 있는 정보를 부착하는 과정

**[핵심/키워드]**

- 텍스트, 이미지, 영상, 음성 등 다양한 데이터에 라벨(Label)을 추가하여 지도 학습(Supervised Learning) 가능하게 함  
- 라벨링(Labeling) : 어노테이션의 세부 작업으로, 특정 정답(클래스, 카테고리 등)을 부여하는 행위

* 주요 기법  
텍스트 - 토큰화 , 개채명 인식 , 감정분석 , 구문분석  
이미지 - 바운딩 박스, 폴리곤, 세그멘테이션 , 키포인트, 큐보이드  
비디오- 프레임 단위 바운딩박스 , 행동 어노테이션  
음성- 화자 분할 ,  음성- 텍스트 매칭 , 감정 어노테이션

## [인공지능] MLPerf(Machine Learning Performance Benchmark)



**[정의]**

- 다양한 하드웨어와 소프트웨어 플랫폼에서 머신러닝 워크로드의 성능을 객관적·공정하게 측정할 수 있는 벤치마크 표준  
- 2018년 하버드, 스탠포드, UC 버클리 등 주요 대학과 Google, NVIDIA, Intel 등 기업들이 공동으로 개발

**[핵심/키워드]**

ML워크로드 성능 벤치마크 표준(CLOSED/OPEN)

&lt;특징&gt;  
- 공개성과 투명성: 결과·코드·데이터셋 공개  
- 표준화: 모델·작업·평가 방식 통일, 공정한 비교  
- 포괄적 평가: Training + Inference 모두 포함

&lt;주요 벤치마크 카테고리&gt;  
- MLPerf Training: 모델 훈련 성능 측정  
ㄴ 측정지표: 학습속도, 학습시간, 처리량  
ㄴ 측정 방식 : CLOSED: 공정성·재현성 중심(표준 모델·데이터 고정)  
                     OPEN: 혁신성·자유도 중심(모델·데이터 선택 자유)  
- MLPerf Inference: 모델 추론 성능 측정  
ㄴ 측정지표 : 추론속도, 처리량, 정확도, 지연시간  
ㄴ Inference 시나리오 : 싱글 스트림(1개 쿼리 순차 실행) / 멀티 스트림(여러 개 쿼리를 일정간격 실행) / 서버(불규칙 쿼리 처리) / 오프라인(대량 쿼리 일괄 처리)  
- MLPerf Mobile: 모바일 기기에서의 추론 성능  
ㄴ 측정지표 : 배터리 효율성, 열관리 포함  
- MLPerf HPC: 슈퍼컴퓨터·GPU클러스터 기반 고성능 컴퓨팅(HPC) 환경에서 대규모 훈련 성능 평가  
- MLPerf Tiny: 소형·저전력 디바이스에서의 AI 모델 성능 평가

## [인공지능] AI 반도체 성능평가지표(K-Perf)



**[정의]**

- AI 학습·추론을 수행하는 반도체의 연산처리 능력, 메모리 처리 특성 및 전력 효율을 정량적으로 측정, 시스템 성능을 평가하기 위한 기준 체계  
- AI 반도체 수요/공급 기업의 성능 고도화를 위해 국산 신경망처리장치 공동 성능지표인 K-퍼프(K-Perf) 발표(과기정통부, 2025년 12월)

**[핵심/키워드]**

K-Perf=국산NPU벤치마크(TTFT/TPOT/TPS/TDP)

&lt;필요성&gt;  
①AI 성능 확보 검증 ②벤더 간 공정 비교 ③산업 차원의 성능 표준화

&lt;처리 단계별 측정 지표&gt;  
- TTFT(Time to First Token): 첫 토큰 출력 시각 - 요청 시작 시각 [Prefill 단계]  
- TPOT(Time per Output Token): 총 디코딩 시간 / 생성된 출력 토큰 수 [Decode 단계]  
- TPS per user(Tokens Per Second): 처리된 토큰 수 / 총 처리 시간 [공통]  
- TDP 평균 전력 소모: 전 구간 소비 전력 / 측정 구간 [공통]

* AI가속 측면의 AI반도체의 성능 평가 지표  
- FLOPS (Floating Point Operations PerSecond)  
- TOPS (Tera Operations PerSecond)  
- MemoryCapacity  
- MemoryBandwidth  
- Latency

## [인공지능] AI 기본법 개정사항 (2026년 7월 시행)



**[정의]**

- 2026년 1월 22일 시행, 세계 두번째 제정된 인공지능 기본법  
-→1월 22일 시행전, 국가 인공지능 전략위원회 기능 강화 일부 개정 됨

◎ AI기본법 추진 일정  
– 2026.01.20: 개정 법률 확정  
– 2026.01.22: 기본법 시행 및 일부 즉시 시행  
– 2026.05.21~06.19: 시행령 입법예고  
– 2026.07.21: 하위법령 포함 본격 시행  
→ 단계적 제도 정착 구조

- AI 산업 육성 기반 강화  
- 공공분야 AI 도입·활용 촉진  
- AI 연구소 설립·운영 근거 마련  
- AI 취약계층 접근성 보장 및 비용 지원  
- AI 창업·전문인력·학습용 데이터 활용 지원

**[핵심/키워드]**

&lt;시행령 개정안 주요 내용&gt;  
– AI기본법 제3조 제5호(AI 취약계층 범위: 장애인·고령자·기초수급자·차상위계층 등 포함),

– AI기본법 제3조 제5호(AI 취약계층 확대: 경력단절여성·구직자·비수도권 중소기업 재직자·농어업인 포함),

– AI기본법 제16조 제3항(공공조달 AI 제품·서비스 범위: 협회 확인 제품·서비스 대상화),

– AI기본법 제16조 제3항(공공조달 대상 확대: 과기정통부 고시 제품·서비스 추가 가능),

– AI기본법 제16조 제4항(공공 AI 면책 연계: 구매·사용 담당자 면책 대상 범위 구체화),

– AI기본법 제17조의2(AI 비용 지원 대상: AI 취약계층 및 비수도권 대학 인재·이공계 인력 포함),

– AI기본법 제18조 제3항(AI 창업 지원 절차: 한국벤처투자에 투자계획 수립 요청 가능),

– AI기본법 제22조의2(AI 연구소 설립·운영: 설립 절차·운영 요건·국가 지원 사항 구체화)

## [인공지능] 인공지능 영향평가 가이드라인



**[정의]**

&lt;인공지능 영향평가&gt;  
– 고영향 AI 제품·서비스 제공 전, 인간의 기본권에 미치는 영향을 사전 평가하는 절차

&lt;인공지능 영향평가 가이드라인&gt;  
– 사업자가 인공지능 제품·서비스가 인간의 존엄성과 기본권에 미치는 잠재적 영향을 사전에 식별·분석하고, 이를 존중·보호하는 방향으로 개선방안을 마련·이행하도록 유도하는 가이드라인

&lt;법적 근거&gt;  
– 인공지능 기본법 제35조(고영향 인공지능 영향평가): 영향평가 수행 노력 의무, 국가기관은 평가 수행 제품 우선 고려  
– 시행령 제28조(수행 방법 등)

**[핵심/키워드]**

&lt;평가 대상&gt;  
– 고영향 AI 제품·서비스 제공 사업자 중심  
– 사전 고영향 여부 판단 필요(필요 시 정부 확인 요청)  
– 법은 고영향 중심이나 모든 AI 서비스 자율 수행 권장

&lt;평가 시기&gt;  
– 신규 서비스 출시 전 수행,  기능/대상 변화 시 재평가 권장  
– 기존 서비스도 필요 시 자율 수행

&lt;평가 수행 주체&gt;  
– AI 사업자 직접 수행 또는 제3자 위탁 가능

&lt;영향 평가 절차&gt;  사 본 사  
① 사전 준비 단계: 평가 필요성 검토, 평가 대상 정의

② 본 평가 수행 단계: 피영향자 분석, 작동원리 분석, 기본권 영향 식별 및 분석

③ 사후 단계: 후속 조치, 문서 관리 및 공개

## [인공지능] AI 신뢰성 인증(CAT) 2.0



**[정의]**

- 민간 인증 전문기관인 한국정보통신기술협회(TTA,TelecommunicationsTechnologyAssociation)가 AI기술을 활용해 민간 제품과 서비스의 위험요인을 분석하고 신뢰성 확보를 위한 사업자의 요구사항 준수 여부를 평가하는 제도  
- 인공지능(AI,ArtificialIntelligence)이 인간을 대신해 학습,추론,자기 개발 등을 할 경우 발생할 수 있는 다양한 신뢰성(Trustworthiness),윤리(Ethic)이슈를 방지하기 위한 인증 제도

**[핵심/키워드]**

* 핵심속성  
- 안전성(Safety), 설명가능성(Explainability), 투명성(Transparency), 견고성(Robustness), 공평성(Fairness)

* 관련표준  
CAT1.0 : ISO/IEC TR 24028(신뢰성 개요), ISO/IEC 23894(위험관리), ISO/IEC 22989(용어)  
→ CAT2.0:위험관리(ISO/IEC 23894), AI경영시스템(42001), AI거버넌스(38507) 기반 설계 변경

- 제품·서비스 : ISO/IEC 23894 (AI 위험관리) - 위험관리 프레임워크 적용 여부 시험·심사  
- 조직 : ISO/IEC 42001 (AI 경영시스템) - 책임있는 AI 개발·운영 역량을 평가하기 위한 경영시스템 심사  
- 조직 : ISO/IEC 38507 (AI 거버넌스) - 의사결정(통제),AI활용 정책 거버넌스 체계를 심사

&lt; 심사내용 &gt; : 위경거  
- ISO/IEC 23894:AI제품의 위험관리 체계 +성능 시험 병행 평가  
- ISO/IEC 42001:AI개발·운영 조직의 PDCA기반 경영시스템 심사  
- ISO/IEC 38507:AI를 도입·활용하는 조직의 거버넌스 구조 검증

## [인공지능] AI RMF(Risk Management Framework)



**[정의]**

2023년 1월, NIST가 발표한 AI 시스템의 전 생애주기에서 발생하는 위험의 관리 및 신뢰가능한 AI 구현을 지원하는 관리체계  
(NIST AI RMF1.0, 2023년 발표)

**[핵심/키워드]**

Govern(거버넌스): 조직의 AI 관리체계 수립  
Map(맥락이해) : AI 사용 환경 및 위험 식별  
Measure(측정) : 위험평가 및 정량화  
Manage(관리) : 위험 대응 및 통제

&lt;신뢰 가능한 7가지 특성&gt;  
유효성 및 신뢰성(Valid&Reliable)  
안전성(Safe)  
보안 및 탄력성(Secure&Resilient)  
책임 및 투명성(Accountable&Transparent)  
설명 및 해석가능성(Explainable&Interpretable)  
개인정보 보호 강화(Privacy-Enhanced)개  
공정성 및 편향 관리(Fair-Harmful Bias Managed)

## [인공지능] 공공부문 초거대 AI 도입 원칙과 고려사항



**[정의]**

* 도입원칙  
원칙 1 : 민간 기술 적극 도입  
원칙 2 : 행정 혁신 병행  
원칙 3 : 부처 간 통합·협업  
원칙 4 : 보안과 권리 보호  
원칙 5 : AI 윤리기준 준수  
① 인권,② 프라이버시,③ 다양성,④ 침해 금지,  
⑤ 공공성,⑥ 연대성,⑦ 데이터 관리,⑧ 책임성,⑨ 안전성,⑩ 투명성

* 고려사항  
1. 적용 업무 및 성과 목표 정의  
2. 기술적 한계 인식  
3. 위험 인식 및 대응  
4. AI 거버넌스 체계 확립  
5. 조직 혁신 전략 및 로드맵

**[핵심/키워드]**

공공부문 초거대 AI 도입·활용 가이드라인 2.0('25년 4월 발행)

* LLM 서비스 레벨 목표(SLO) 예시  
- BLEU (Bilingual Evaluation Understudy)  
- 응답 시간 (Response Time)  
- 가용성 (Availability)  
- 데이터 보안 (Data Security)  
- 윤리강령 준수 (Ethics Compliance)  
- 모델 업데이트 주기 (Model Update Cycle)  
- 책임과 보상 체계 (Accountability & Compensation)  
- 사용자 수용능력 (User Capacity)  
- 기술 지원 (Technical Support)  
- 사용 데이터 보고 (Usage Data Report)  
- 해지 정책 (Termination Policy)  
- 법적 준수 사항 (Legal Compliance)

## [인공지능] 재현 데이터 (Synthetic Data, 합성데이터 )



**[정의]**

- 실제 데이터를 분석한 결과와 유사한 결과를 얻을 수 있도록 인공적으로 재현하여 생성한 가상데이터

- 원본과 통계적으로 유사하나 가상으로 다시 만들어진 합성 데이터

**[핵심/키워드]**

* 유형 : 완전, 부분, 하이브리드  
 * 생성기법 : 베이지안, 기계학습, 차등정보보호기반  
 * 절차 : 원본수집, 기법적용, 합성데이터확보, 유용성 평가, 익명성 평가, 활용

<유사성(Similarity) 평가>
– 상관관계/연관성  
– UM(Utility Metric)  
– CvM-거리  
– CAM(Clustering Analysis Metric)  
– pMSE  
– α-Precision  
– β-Recall  
<유용성(Utility) 평가>
– TSTR(Train Synthetic, Test Real)  
– MSE / RMSE  
– 신뢰구간 중첩  
– 타원체 중첩  
<위험성(Risk/Privacy) 평가>
– DUPI(Data Utility and Privacy Index)  
– CAP  
– CM(Confidentiality Metric)

## [인공지능] 이미지 캡셔닝 기술



**[정의]**

- 이미지에서 객체, 배경, 동작 등의 시각적 요소를 분석한 후, 이를 자연어 문장으로 설명하는 기술

생성형 AI 데이터 품질관리 가이드 v2.5 의 3장 '생성형AI 주요 기술' 항목에 기재

**[핵심/키워드]**

* 이미지 캡셔닝 방법  
오토 캡셔닝: 인공지능이 자동으로 분석 , 생성  
휴면 캡셔닝: 사람이 직접 이미지를 분석하여 이미지 캡션을 생성

*이미지 캡셔닝의 핵심 구성 요소  
이미지 특징 추출기  
언어 모델  
어텐션 메커니즘  
디코더  
데이터셋

*캡셔닝 방식  
맥락 기반 캡셔닝  
객체 레벨 캡셔닝  
질의 응답 캡셔닝  
스토리텔링 캡셔닝  
구조화된 캡셔닝  
밀집 캡셔닝  
희소 캡셔닝  
선호 기반 캡셔닝  
임베디드 캡셔닝  
관계형 캡셔닝  
지식 기반 캡셔닝  
비디오 캡셔닝  
공간, 시간 이해 캡셔닝

## [인공지능] 추론형 AI



**[정의]**

단순 패턴 인식·예측을 넘어 논리적 단계를 거쳐 복잡한 문제 해결 및 의사결정을 수행하는 AI

**[핵심/키워드]**

* 추론형AI 유형  
기술에 따른 분류:  기호적 추론 , 통계적 추론 , 뉴로-심볼릭 추론  
논리적 원리에 따른 분류: 논리적 추론 , 수리적 추론 , 비단조 추론, 퍼지 추론 , 상식 추론

* 주요 추론 아키텍처  
COT : 최종 답 도출 전 중간 추론 과정을 단계적으로 생성  
SC-CoT(자기 일관성 COT): 여러개의 독립적CoT를 생성 후 가장 일관된 답을 선택  
ToT(생각의 트리): 여러 추론 경로를 트리 구조로 탐색·평가  
GoT(생각의 그래프): 추론 단계를 노드(Node), 관계를 엣지(Edge)로 표현

## [인공지능] 추론형 AI 데이터 정의 및 품질 특성



**[정의]**

일반 데이터와 달리 논리적 연결성, 인과 관계, 다단계 추론 패턴을 포함하는 데이터

**[핵심/키워드]**

* 추론형 AI 데이터 구조  
질의(Query,Q)- 추론(Reasoning,R)- 답변(Answer,A)

*추론형 AI 데이터의 품질 특성  
정확성  
논리적 일관성  
정합성  
추론 완전성  
추론 경로 명료성  
일관성  
다양성  
신뢰성  
검증가능성  
윤리 투명성

## [인공지능] 고영향 인공지능 판단 가이드라인(고영향 인공지능 확인 가이드라인)



**[정의]**

&lt;정의&gt;  
- 사업자가 고영향 인공지능 해당 여부 및 책무 유무를 스스로 판단할 수 있도록 기준과 예시를 제공하는 가이드라인  
- 자율 판단 지원, 판단 기준·사례 제공, 예측 가능성 제고 및 혼란 방지

&lt;법적 근거&gt;  
– 인공지능기본법 제33조제3항(고영향 AI 기준·예시 가이드라인 )  
- 시행령 25조 “고영향 인공지능 확인 절차 등”

**[핵심/키워드]**

1단계. 영역 조건

- 중요 사회·공공 영역에 활용되는 AI  
- 에너지, 먹는물 관리, 보건의료·의료기기, 원자력  
- 범죄 수사·체포, 생체인식, 채용·대출 심사  
- 교통, 공공서비스, 교육

2단계. 위험 조건  
- 생명·신체·기본권에 중대한 영향 또는 위험 초래 가능성

최종 판단  : 고영향 인공지능 적용 기준  
- 1단계 영역 조건과 2단계 위험 조건을 모두 충족하는 경우 고영향 인공지능으로 판단

## [인공지능] 고영향AI 사업자 책무 가이드라인



**[정의]**

&lt;정의&gt;  
- 고영향 인공지능 사업자가 안전성·신뢰성 확보 의무를 효과적으로 이행할 수 있도록 구체적 기준과 절차를 제공하는 실행 가이드라인

&lt;법적 근거&gt;  
- 인공지능 기본법 제34조 (고영향 인공지능 관련 사업자의 책무)  
- 시행령 제27조 (고영향 인공지능과 관련한 사업자의 책무)

**[핵심/키워드]**

&lt;고영향 인공지능사업자 책무 조치사항&gt; : 위 설 보 고/감 문/보

① 위험관리방안의 수립·운영: 위험관리정책 수립 및 이행, 위험관리 조직체계 수립 및 운영

② 기술적으로 가능한 범위에서의 설명 방안 수립·시행: 인공지능이 도출한 최종결과 및 기준에 대한 근거 마련, 학습용데이터 정보의 관리, 설명 방안의 수립 및 시행

③ 이용자 보호방안 수립·운영: 인공지능 개발 단계, 인공지능 운영 단계

④ 고영향 인공지능에 대한 사람의 관리·감독: 인공지능 개발 단계, 인공지능 운영 단계

⑤ 안전성·신뢰성 확보 조치 확인 가능한 문서의 작성과 보관: 문서화 및 관리 방안

## [인공지능] 인공지능 투명성 확보 가이드라인



**[정의]**

&lt;정의&gt;  
- 이용자가 AI 기반 서비스 이용 사실과 결과물의 AI 생성 여부를 명확히 인식하도록 하여 혼동을 방지하고 사회적 신뢰를 확보하기 위해 정의된 가이드라인

&lt;법적 근거&gt;  
- 인공지능 기본법 제 31조 “인공지능 투명성 확보 의무”  
- 시행령 23조 , 인공지능 투명성 확보 의무 이행

- 적용 대상: 최종 서비스 제공 사업자, API 활용 서비스 사업자, 모델 개발자(직접 제공 시), 해외 사업자

- 제외 대상: 단순 이용자, 결과물 활용자, 콘텐츠 제작자 등

**[핵심/키워드]**

법 제31조 제1항  
- 사전 고지 의무: 고영향 AI 및 생성형 AI를 이용한 제품·서비스 제공 시 제품·서비스가 고영향 AI 또는 생성형 AI 기반으로 운영된다는 사실을 사전에 고지

법 제31조 제2항  
- 표시 의무: 생성형 AI 및 이를 이용한 제품·서비스 제공 시 결과물이 AI에 의해 생성되었다는 사실을 표시

법 제31조 제3항  
- 딥페이크 생성물 표시 의무: AI 시스템으로 실제와 구분하기 어려운 가상의 생성 결과물 제공 시 해당 생성 결과물이 AI로 생성되었다는 사실을 고지 또는 표시

## [인공지능] 인공지능 데이터센터 산업 진흥에 관한 특별법



**[정의]**

인공지능산업 발전의 기반이 되는 인공지능 데이터센터의 구축과 운영을 지원하고 관련 산업의 육성과 기반 조성 등에 필요한 사항을 규정함으로써 국가경쟁력 강화에 기여하기 위한 법

→ AI 데이터센터 법제화 추진  
(2026.05.07 국회 본회의 통과 )  
2027년 2월에 시행될 예정

**[핵심/키워드]**

안 제1조～제2조 :  목적 및 정의  
· AI 데이터센터의 구축·운영 지원 및 관련 산업 육성  
· AI, AI 데이터센터, AI 데이터센터 사업자의 개념 명확화

안 제5조～제11조 : 진흥체계 구축  
· 실태조사 및 통계 작성· 전담기관·협회 설립 근거 마련  
· AI 데이터센터 사업자의 과학기술정보통신부 장관 신고제 도입

안 제12조～제16조 : 행정·재정적 지원  
· 전력·통신 등 기반시설 우선 설치 및 부대시설 지원  
· 전문인력 양성, 금융지원 및 보조금 지급· 국제협력, 해외 진출 촉진 및 지역사회 협력

안 제18조 : 인허가 절차 간소화  
· 과학기술정보통신부를 통한 복합 인허가 사항 일괄처리(원스톱 창구)  
· 관계기관의 신속한 검토 및 통지 의무화  
· 타임아웃제 도입: 일정 기간이 지나면 인허가 처리 완료로 간주

안 제19조, 제21조～제23조 : 전력 및 건축 특례  
· 비수도권 AI 데이터센터의 전력계통영향평가 실시 면제  
· 승강기, 전기차 충전시설, 부설주차장 등의 설치 의무 완화  
· 산업입지법·산업집적법·항만법 관련 특례 부여

안 제17조, 제24조～제27조 : 특구 및 환경  
· AI 데이터센터 특구 제도 도입 및 규제개선 신청권 부여  
· 전자파 영향 측정 장비의 설치·운영에 관한 과학기술정보통신부 고시

## [인공지능] 보안 취약점 신고조치 공개 제도(CVD/VDP)



**[정의]**

기업·기관이 취약점 신고 정책(VDP)을 사전에 공개하고, 화이트해커가 취약점을 탐색·신고하면, 기관이 이를 접수·검증·조치한 후 외부에 공개(CVD)하는 협력 기반의 선제적 취약점 관리 체계

**[핵심/키워드]**

&lt;운영 흐름&gt;  
- 기업·기관 : VDP 정책 수립·공개  
- 화이트해커: 정책 준수 하 취약점 탐색·신고  
- 기업·기관: CVD 기반 접수·조치·공개(협의)

* 구성체계  
- VDP (Vulnerability Disclosure Policy) : 취약점 신고 정책  
- CVD (Coordinated Vulnerability Disclosure) : 취약점 공개 프로세스  
신고된 취약점에 대해 접수 → 검증 → 조치 → 공개(시기 조율)  
수행기업·기관과 화이트해커 간 협의 기반 책임 공개 프로세스

* 적용 로드맵  
1단계(~2026) : 시범사업  
- 민간(과기부)·공공(국정원) 주도 시범 운영  
- 제도 도입 가능성 및 효과 사전 검증  
2단계(~2027) : 참여 확대  
- 시범사업 기반 제도 설계 및 가이드라인 마련  
- 민간·공공 전반으로 참여 확산 유도  
3단계(이후) : 법제화  
- 관련 법령 개정 통해 제도 정식 도입  
- 정보통신망법, 개인정보보호법, 국가정보보안지침 등 법·제도 정비

## [인공지능] 소버린 AI



**[정의]**

국가 또는 특정 지역이 데이터/AI인프라 모델을 독립적으로 통제하고 운영할 수 있도록 하는 AI 주권 확보 전략

**[핵심/키워드]**

* 핵심 구성 요소  
- 자국 데이터 주권 확보  
- 국산 AI 모델 개발 역량 확보  
- 국가 차원의 AI 인프라 보유  
- 반도체 기반 기술 확보

* 정책/기술 요소  
- 국산 LLM 개발  
- 국산 AI 인프라 구축  
- AI 윤리 및 규제 체계 구축  
- Open-source 전략 병행

&lt;소버린 AI구현을 위한 기술 범주&gt;  
- 데이터 주권 : 소버린 클라우드, 로컬 데이터 허브  
- 모델 주권 : 자국어 LLM, 도메인 특화 모델  
- 컴퓨팅 자립 : 국산 AI 반도체, 국산 클라우드 인프라  
- AI 알고리즘 : 국산 프레임워크, 다국어 알고리즘  
- 보안/투명성 : XAI 기술, AI 감사 시스템  
- AI 운영 기술 : 모델 경량화, 저전력 추론  
- 오픈소스 전략 : 공개 모델 활용, 공동 개발 체계

