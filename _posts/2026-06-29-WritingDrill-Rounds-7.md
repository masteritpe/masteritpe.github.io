---
layout: post
title: "WritingDrill_Rounds_7"
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

### [인공지능] Drop Out(드랍아웃)

**[정의]**

심층 신경망의 과적합을 방지하기 위해 은닉층의 일부 노드를 무작위로 비활성화 시켜 정규화(성능 일반화) 하는 신경망 학습 기법

**[핵심/키워드]**

*효과 : 과적합 방지, 앙상블 효과, 학습성능 향상 
 * 드랍아웃 유형 
 - 표준 드랍아웃 (Standard Dropout) 
 - Spatial Dropout : CNN에 사용 
 - Variational Dropout : RNN에 사용 
 - Fast Dropout : 계산 비용 감소 
 - Ad-hoc Dropout : 가중치에 적용

### [인공지능] 지식증류

**[정의]**

대규모 모델(교사 모델, Teacher Model)이 학습한 지식을 소규모 모델(학생 모델, Student Model)로 전이하여, 성능은 최대한 유지하면서 모델의 크기와 계산 복잡도를 줄이는 기술

**[핵심/키워드]**

LLM성능향상, 모티모달(융합 모듈), 경량화 
- Teacher /  Student 모델  
- Soft Labels 학습(Temperature 조절 -→ 클래스 확률분포) 
- Soft Labels 모방 
 ① Distillation Loss(KL Divergence) : Teacher와 Student 모델 출력의 차이
 ② Student Loss(L1/L2 Norm) : 실제 레이블과 Student 모델 출력의 차이

### [인공지능] SLM (Small Language Model, 소형 언어 모델)

**[정의]**

특정 목적에 최적화되거나 엣지 디바이스 등 제한된 환경에서 효율적으로 동작하도록 설계 된, 상대적으로 작은 파라미터 수와 계산 자원을 사용하는 경량화된 언어 모델

**[핵심/키워드]**

- 연산 비용을 낮춘 경량형 언어 모델
- 수백만~수천만 개의 파라미터(LLM : 수십억 ~ 수조개)
- 모델 크기 : 작음 (MB~GB 단위) 
- 제한된 특정 도메인 데이터
- 로컬 AI, 모바일 AI, 엣지 컴퓨팅
- Gemma 2B, GPT-2, LLaMA-7B 

<모델 경량화 기술 : SLM 기술요소>
모델 경량화 (Model Compression)
지식 증류 (Knowledge Distillation)
양자화 (Quantization)
프루닝 (Pruning)
특화 데이터 파인튜닝
온디바이스 최적화 (Edge/On-Device AI)
효율적 트랜스포머 구조
멀티태스크 학습 및 적응

### [인공지능] 선형 판별분석(Linear Discriminant Analysis, LDA)

**[정의]**

클래스 간 분산(between-class scatter)과 클래스 내 분산(within-class scatter)의 비율을 최대화하여, 독립변수들의 측정값에 따라 데이터가 어느 집단에 속할 것인가에 대해 판별하는 분석 방법

**[핵심/키워드]**

분류분석, 차원축소, 클래스 간 분산(between-class scatter)과 클래스 내 분산(within-class scatter)의 비율을 최대화 
- 공통된(동일한) 공분산 행렬을 가지는 다변수 정규분포 가정 
&lt;절차&gt; 
- 클래스 평균 계산 -→ 클래스 내 분산 행렬 SW 계산 -→ 클래스 간 분산 행렬 SB 계산 -→ 판별 벡터 W계산 

- PCA :데이터의 분산을 최대화하는 축 기준 
- QDA : 클래스별로 서로 다른 공분산 행렬 사용

### [인공지능] Q-러닝(Q-Learning)

**[정의]**

환경과 상호작용하며 Q-값을 업데이트하여 최적 정책을 학습하는 모델 프리 강화학습

**[핵심/키워드]**

모델프리, Value-Based, Off-Policy  

Q-함수 (Q-Function, Q(s,a))
Q-테이블 (Q-Table)
벨만 방정식 (Bellman Equation)
할인율 (Discount Factor, γ)
학습률 (Learning Rate, α)
탐색 전략 (Exploration Strategy)
Epsilon-Greedy 탐색

Q-테이블 크기가 너무 커짐 -→ DQN, DDQN, SARSA

### [인공지능] XAI(eXplainable AI)

**[정의]**

사용자가 인공지능 시스템의 동작과 최종 결과를 이해하고 올바르게 해석하여 결과물이 생성되는 과정을 설명 가능하도록 해주는 기술

**[핵심/키워드]**

알고리즘의 조작 가능성, 의사결정의 편향성 , 머신러닝 AI에 대한 신뢰성 입증 한계 <= 해결 목표  
&lt;모델 내 설명 방법론&gt; 
신경 회로망 노드에 설명 라벨링
의사결정트리를 이용한 설명 모델 만들기
 통계적 방법을 이용하여 설명 모델 유추하기 
&lt;모델 외 설명 방법론&gt;  
화이트박스 모델 (White-box Model)
해석 가능한 신경망 (Interpretable Neural Networks)
Surrogate Model (대리 모델)
LIME(Local Interpretable Model-agnostic Explanations)
SHAP (SHapley Additive exPlanations)
Counterfactual Explanations
Saliency Map (살리언시 맵)
Grad-CAM (Gradient-weighted Class Activation Mapping)
Feature Attribution (특징 속성 분석)
Rule Extraction (규칙 추출)
Decision Trees Approximation(의사결정 트리 근사화)
Attention Mechanism (어텐션 메커니즘)
Concept Bottleneck Models
Explainable Chatbots (설명 가능한 챗봇)
Interactive Visualization (대화형 시각화)

### [인공지능] 빈발패턴성장 알고리즘(FP-Growth, Frequent Pattern)

**[정의]**

분석해야 할 데이터가 증가하면서, 선험적 규칙(Apriori) 알고리즘의 연산 속도를 개선한, 트리(Tree) 구조 기반의 연관규칙 알고리즘(빈발 패턴 집합 탐색, 즉 빈발품목 생성)

**[핵심/키워드]**

- 중복된 트랜잭션을 하나의 트리 경로로 결합 
- 데이터를 압축하여 저장 → FP-Tree를 사용 

최소 지지도 기반 선택 -→ 빈도 수 기반 정렬 -→ FP-Tree생성 -→ 트리 시작 및 확장 -→ 빈발품목 집합 도출

### [인공지능] SVM (Support Vector Machine)

**[정의]**

데이터 포인트를 고차원 공간에서 분리하는 최적의 결정경계(Decision Boundary)를 찾아주는 지도 학습(Supervised Learning) 알고리즘

**[핵심/키워드]**

* 구성요소
 - Margin
 - Support Vector
 - Hyper-plane  
 - 하이퍼 파라미터 : C(Regularization Parameter), 허용 오차 (ξ)
, Epsilon (ε, SVR에서 사용) = 𝜀-Tube (Epsilon-Tube)

* 학습 유형 : 분류, 회귀  
* 분류 설정  
 - 좁은 마진(큰 C값), 오분류 허용 X (하드 마진) 
 - 넓은 마진(작은 C값), 오분류 허용 O (소프트 마진) 

* 비선형 처리 -→ Kernel 함수(=커널트릭) 이용   
 - 선형, 다항, RBF, 시그모이드

### [인공지능] KNN(K-Nearest Neighbor)

**[정의]**

새로운 데이터 포인트(Test Data)가 주어졌을 때, 기존 학습 데이터(Training Data)와의 거리를 측정하여 가장 가까운 K개의 이웃을 찾고, 다수결 또는 평균을 이용하여 예측하는 비모수적(Non-Parametric) 지도 학습 알고리즘

**[핵심/키워드]**

- 분류 문제: 가장 많은 속성을 가진 클래스로 분류 (다수결 투표)
- 회귀 문제: K개의 이웃의 평균값을 사용하여 예측
- 비모수적 모델, 메모리기반학습(레이지 러닝: 학습 불필요)
&lt;절차&gt;
- 거리 계산 -→ 가장가까운 k개 데이터 선택 -→ 보팅(분류), 평균(회귀)
* 장점
 간단하고 효과적, 기본적인 분포가정 필요없음, 학습과정 빠름
 * 단점
 모든 데이터와 거리계산 필요, 새로운 인사이트를 얻는데 제한

### [인공지능] 앙상블 알고리즘

**[정의]**

여러 개의 모델을 결합하여 단일 모델보다 데이터의 변동성에 강하며, 더 높은 정확도와 일반화 성능을 얻을 수 있는 얻는 기법

**[핵심/키워드]**

- 성능 향상,  과적합 방지, 편향-분산 트레이드오프 최적화, 모델 안정성 향상 
&lt;유형&gt; 
배깅(Bagging)
 ㄴ 랜덤포레스트
부스팅(Boosting)

보팅(Voting)

블렌딩(Blending) : 검증데이터 에측값을 메타모델에 학습
스태킹(Stacking) : 각 모델의 예측 결과를 메타 모델에 입력으로 사용



&lt;앙상블 알고리즘 선택 예시&gt; 
- 속도가 중요하고 과적합을 방지해야 함 → 랜덤 포레스트 (배깅)
- 최고의 성능이 필요 → XGBoost, LightGBM (부스팅)
- 서로 다른 모델을 결합하고 싶음 → 스태킹(Stacking)

### [인공지능] 어텐션 메커니즘 (Attention Mechanism = Self Attention)

**[정의]**

seq2seq의 경사감소 소멸(Gradient Descent Vanishing) 등 RNN 모델의 문제 해결을 위해 출력 단어 예측 시점 마다 입력 시퀀스의 단어 가중치를 계산하여 정확도 감소를 보정하는 메커니즘 

Transformer의 기반 모델

**[핵심/키워드]**

&lt;학습 절차&gt; 
1️⃣ Query, Key, Value 생성
2️⃣ Query-Key 유사도 계산
3️⃣ Softmax 적용 (어텐션 분포 생성)
4️⃣ Value 가중합 (어텐션 값 생성)
5️⃣ 최종 출력 반환

&lt;핵심요소&gt; 
Query (Q)
Key (K)
Value (V)
어텐션 분포 (Attention Distribution)
어텐션 값 (Attention Value)
Scaled Dot-Product Attention

### [인공지능] MCP (Model Context Protocol)

**[정의]**

- 복잡한 AI 워크플로우 구축을 위해 생성형 AI 등 인공지능 모델에 문맥 정보를 제공하여 외부 데이터 소스 및 도구를 연결하는 개방형 프로토콜 

- AI 모델이 외부 애플리케이션, 도구, 데이터 소스 등과 안전하고 유연하게 상호작용할 수 있도록 설계된 개방형 통신

**[핵심/키워드]**

주요기능 : Context-Aware, Agent-Ready, 플러그인 기반 확장성, 실시간 연결 

MCP 핵심 구성 : MCP Host, MCP Client, MCP Server
AI 구성 요소 : AI 모델 (LLM), Context Provider
Context Provider : Local Filesystem, Database, Web APIs (인터넷 서비스)
연동·확장 구성 : MCP 브리지 (Bridge/Adapter), 플러그인·도구 (Plugins)

### [인공지능] 랜덤 포레스트 (Random Forest)

**[정의]**

- 배깅처럼 데이터를 반복 복원추출을 진행할 뿐만 아니라, 거기에 더해 변수 또한 랜덤하게 추출하여 다양한 모델을 만드는 앙상블 기법 

- 분류/회귀 분석 등에 사용하기 위해 다수 의사결정 트리를 결합하여 분류/회귀 모형을 생성하는 앙상블 기반 머신러닝 학습 기법

**[핵심/키워드]**

&lt;하이퍼 파라미터&gt; 
- n_estimators
- max_depth
- max_features
- min_samples_split
- min_samples_leaf
- bootstrap

&lt;알고리즘 요소&gt; 
 - 의사결정 트리, 부트스트랩, 보팅(하드/소프트)

### [인공지능] 주성분 분석 (PCA)

**[정의]**

- 데이터의 분산(Variance)을 최대한 보존하면서 고차원 데이터를 저차원으로 축소하는 선형 차원 축소 기법

 - 고차원 공간의 표본들을 선형 연관성이 없는 저차원 공간(주성분)의 표본으로 변환하여 분석하는 알고리즘

**[핵심/키워드]**

- 주성분간에는 독립성, 선형 변환, 차원 축소 

&lt; 절차&gt; 
1\. 데이터 정규화 (Standardization)
2\. 공분산 행렬 계산 (Covariance Matrix Computation)
3\. 고유값 분해 (Eigen Decomposition) 
  - 고유값, 고유벡터 
4\. 주성분 선택 (Select Principal Components)
5\. 데이터 변환 (Projection onto New Basis) 

&lt;주성분 선택 기준&gt; 
 - Eigen Value, Eigen Ratio, Scree Plot

### [인공지능] 파운데이션 모델 (Foundation Model)

**[정의]**

- 대규모 데이터와 강력한 연산 능력을 활용하여 사전 학습(Pretraining)된 범용 인공지능 모델로, 다양한 AI 태스크에 쉽게 적용(Fine-tuning)할 수 있는 기반이 되는 모델(기초 모델) 

- 범용적 모델, GPT-4등, 광범위한 학습데이터 활용

**[핵심/키워드]**

&lt;구성방법 및 특징&gt; 
사전 학습 (Pretraining) 기반
자기지도학습(Self-Supervised Learning) 기반
창발성 (Emergence)
균일화 (Homogenization)
다양한 태스크에 적용 가능
Fine-tuning 및 Prompting 지원
멀티모달 확장 가능
Zero-shot / Few-shot Learning 지원 

&lt;파운데이션 모델 최적화 기법&gt; 
지식 증류 (Knowledge Distillation)
가중치 가지치기 (Weight Pruning)
양자화 및 이진화 (Quantization & Binarization)
가중치 공유 (Weight Sharing)
파라미터 효율적 미세 조정 (PEFT, Parameter Efficient Fine-Tuning)
희소성 유도 (Sparsity Induction)
지연된 가중치 업데이트 (Delayed Updates)

### [인공지능] 생성적 적대 신경망 (Generative Adversarial Network, GAN)

**[정의]**

생성자(Generator)와 판별자(Discriminator) 두 개의 신경망이 경쟁(Adversarial)하며 학습하는 생성 모델 알고리즘. 

- 특징 : 경쟁학습, 생성 모델(Implict density : 학습 분포 모름), 준지도 학습, 비지도 학습 활용 가능(D는 학습없이도 판단 가능)

**[핵심/키워드]**

생성자 : 무작위 노이즈 z 를 입력받아 가짜 데이터를 생성 
 ㄴ 은닉층 : ReLU 또는 Leaky ReLU
 ㄴ 출력측 : Tanh 
 ㄴ 손실함수 : 1로 최대화 
판별자 : 판별  
 ㄴ 은닉층 : Leaky ReLU
 ㄴ 출력측 : Sigmoid 
 ㄴ 손실함수 : 크로스 엔트로피

### [인공지능] 연합학습 (Federated Learning)

**[정의]**

- 중앙 서버에 데이터를 모으지 않고, 분산된 여러 장치(클라이언트)에서 개별적으로 모델을 학습한 후, 학습된 가중치만 서버에 공유하는 분산 학습 기법
 
- 분산 저장된 데이터 이동 없이 각 장치의 학습 결과를 수집/종합하여 모델을 생성하는 분산형 머신러닝 기술 

- 프라이버시보호모델(PET), 온디바이스 AI 활용, 모델 지속적 업데이트

**[핵심/키워드]**

1️⃣ 초기 모델 배포(Global Model Initialization)
2️⃣ 로컬 학습 수행(Local Training at Clients)
3️⃣ 모델 업데이트 전송(Send Model Updates)
4️⃣ 연합 평균화 수행(Federated Averaging, FedAvg)
5️⃣ 모델 업데이트 및 재배포(Global Model Update & Redistribution) 

모델 결합 알고리즘 
-FedSGD (Federated Stochastic Gradient Descent)
- FedAvg (Federated Averaging)
- FedProx (Federated Proximal)
- FedOpt (Federated Optimization)
- FedMA (Federated Matched Averaging)
- FedBN (Federated Batch Normalization)
- FedGKT (Federated Gradient Knowledge Transfer)
- FedReID (Federated Learning for Person Re-identification)

### [인공지능] 규제화(Regularization)

**[정의]**

손실 함수에 추가 항을 적용하여 모델의 복잡도를 줄이고, 과적합을 방지하는 기법 

- 모델이 훈련 데이터에 과도하게 최적화되지 않도록 가중치나 구조를 조정하여 일반화 성능을 향상시키는 기법

- 과정합 방지, 손실함수에 규제 적용, 모델 복잡도 감소

**[핵심/키워드]**

L2(Ridge) : 가중치 축소, 모든 가중치를 0에 가깝게 유지

L1(Lasso) : 희소성 유도, 특정 가중치가 0이 되도록 유도

### [인공지능] GNN (Graph Neural Network = 그래프 신경망)

**[정의]**

- 노드(node)와 엣지(edge)로 구성된 그래프의 구조와 노드의 특성(feature)을 동시에 반영하여, 각 노드 또는 전체 그래프의 표현(embedding)을 학습할 수 있는 딥러닝 모델 
 
- 데이터의 특징 추출을 위해 이웃 노드 간 정보를 이용하여 특징 벡터를 찾아내는 그래프(Graph) 기반 신경망 모델

**[핵심/키워드]**

&lt;학습 매커니즘&gt; 
Data (입력 데이터)
Graph Construction (그래프 생성)
Graph Neural Network (그래프 신경망 학습)
Optimization(최적화)
&lt;GNN 방법론&gt; 
Spectral GNN : 주파수 도메인에서 변환
Spatial GNN : 직접 이웃 노도 정보 학습 

&lt;Spectral GNN&gt;  
 -GCN (Graph Convolutional Network)
- ChebNet (Chebyshev Graph Convolutional Network)
- Spectral CNN 
&lt;Spatial GNN&gt;
- GraphSAGE (Graph Sample and Aggregate)
- GAT (Graph Attention Network)
- MPNN (Message Passing Neural Network)
- GIN (Graph Isomorphism Network)

### [인공지능] DBSCAN Clustering (Density-based spatial clustering of applications with noise)

**[정의]**

- 데이터 포인트의 밀도를 이용해 군집을 형성하고, 이상치(Noise)를 효과적으로 식별하는 비지도학습 알고리즘

- 반달모양(Moon-Shaped) 비구형 데이터 셋 군집

**[핵심/키워드]**

&lt;하이퍼파라미터&gt; 
 - MinPoints, Epsilon 

&lt;탐색 기준&gt; 
 - 코어, 노이즈, 보더 

&lt;단점 및 해결 알고리즘&gt; 
 - 하이퍼파라미터 설정에 민감, 밀도 다른 경우 군집 어려움  -→ OPSTIC 알고리즘(유동적 Epsilon 사용)

### [보안] 다자간 계산(MPC, Multi-Party Computation)

**[정의]**

서로 신뢰하지 않는 다수의 참여자가 개별 입력을 노출하지 않고, 공동의 연산 결과만을 계산할 수 있도록 하는 암호 기반 분산 계산 기법

**[핵심/키워드]**

프라이버시 보장, 분산 신뢰 모델
 주요기술 : Yao의 개릿 서킷, 시크릿 셰어링, 동형암호, 소수정밀연산, 블라인드 평가, 하이브리드 MPC

### [보안] 산업제어시스템 보안

**[정의]**

발전소, 제조설비, 교통, 수도 등 물리적 인프라를 제어하는 시스템(PLC, SCADA 등)을 사이버 위협으로부터 보호하는 기술 및 정책 체계

**[핵심/키워드]**

&lt;취약점&gt; 
 - 보안 설계 결여, 에어갭 신화, 공격 면 확대, 노후화된 시스템 사용, 패치 미흡, 비보안 장비 다수 존재, 취약한 임베디드 SW 사용, 공급망 불안정, 권한 관리 미비, 네트워크 분리 미흡, 보안 인력 부족 
 &lt;대응방안&gt; 
 - 산업제어시스템 위험 평가, 자산 식별 및 가시성 확보, 탐지 장비 도입, 화이트리스트 기반 제어, 네트워크 세그멘테이션, 단방향 통신 구성, 로그 수집 및 모니터링, 외부 인력 통제, IT/OT 사고 대응계획, 보안 전문가 육성, 정보보호 교육 확대

### [보안] CC(Common Criteria)

**[정의]**

- 서로 다른 국가 간에도 보안 평가 결과를 상호 인정받기위해, IT 보안 제품 및 시스템의 보안성 평가를 위한 국제 표준 (ISO/IEC 15408)

**[핵심/키워드]**

기능 요구사항(SFR), 보증 요구사항(SAR),
 PP, ST, TOE, CCRA, CEM, EAL

### [보안] 제로트러스트 가이드라인 2.0

**[정의]**

아무도 신뢰하지 않는다(Trust No One)”는 원칙 하에, 모든 사용자·기기·서비스에 대해 지속적으로 검증하고 최소 권한만 부여하는 보안 모델을 구현하기 위한 국가 차원의 적용 지침

**[핵심/키워드]**

성숙도 모델 : 기존 환경, 초기, 고급, 최적 
 핵심 영역 : 식별자·신원, 기기 및 엔드포인트, 네트워크, 시스템, 애플리케이션 및 워크로드, 데이터 
 핵심 구성요소 : 
 - 정책결정지점 (PDP) 
 ① 정책 엔진(PE)
 ② 정책 관리자(PA)
 - 정책시행지점 (PEP)

### [보안] 소프트웨어 공급망 공격(SW Supply Chain Attack)

**[정의]**

소프트웨어 공급망을 구성하는 요소 중 하나 이상이 공격자에 의해 손상되거나 변경되어, 최종적으로 배포되는 소프트웨어가 악성 코드 또는 취약한 상태로 조작되는 공격 방식

**[핵심/키워드]**

&lt;취약점&gt; 
 - 공개 SW 보안취약점, 타사 의존성, 공용 리포지토리, 변환 시스템, 업데이트 가로채기, 내부 리포지토리, 공급사 및 협력사 
 &lt;대응방안&gt; 
 - 취약점 점검 및 패치, SBOM 관리, 외부 라이브러리 검증, 코드 서명·무결성 검증, 리포지토리 모니터링, 의심 파일 탐지, 빌드 서버 점검, CI/CD 보안, 안전한 OTA 구축, 업데이트 암호화, 접근통제 강화, 내부 감사, 공급망 보안 계약, 보안 점검 수행

### [보안] OWASP(Open Web Application Security Project) TOP 10 2021

**[정의]**

- 웹 애플리케이션의 보안 취약점 중 가장 위험한 10가지를 선정하여 공개하는 프로젝트 
 2021년 : 보안이 설계·운영 단계까지 확장, 복합적 보안 이슈 반영

**[핵심/키워드]**

취약한 접근 제어, 암호화 실패, 인젝션, 불안전한 설계, 잘못된 보안 구성, 취약하고 오래된 컴포넌트, 식별 및 인증 실패, 소프트웨어 및 데이터 무결성 실패, 로깅 및 모니터링 실패, 서버 측 요청 위조

### [보안] Lattice모델

**[정의]**

보안 등급 간의 위계 관계(격자 구조)를 기반으로 주체(사용자)와 객체(데이터) 간 접근 권한을 수학적으로 모델링한 접근 제어 모델

**[핵심/키워드]**

구성요소
 - 주체, 객체, 보안 등급(SL), 격자 구조, 허용 규칙
 - MAC, RBAC 
 - biba, bell labpdula

### [보안] DAC (Discretionary Access Control)

**[정의]**

자원 소유자(Owner)가 해당 자원에 대해 누가 어떤 접근 권한을 가질지 자율적으로 결정할 수 있는 접근통제 방식

**[핵심/키워드]**

소유자 중심 통제(소유자가 권한 설정), 유연성(자율적 운영 가능), 보안 취약 가능성(권한 확산 위험), 
  
 ACL/CL기반(객체 중심 구현), 일반 시스템 적용(운영체제, DB 등), Clark-Wilson

### [보안] CSO (정보보호 최고책임자)

**[정의]**

조직 내 정보보호 및 보안 전반을 총괄하는 최고 책임자로, 정보보호 정책 수립, 위험관리, 보안 사고 대응, 보호대책 운영 등을 담당하는 임원급 역할

**[핵심/키워드]**

정보통신망법, 제45조의3(정보보호 최고책임자의 지정 등) 
 
 - 정보보호 계획 수립 및 개선
 - 정보보호 실태 감사 및 개선
 - 위험 식별 및 대책 마련
 - 정보보호 교육·훈련 계획 수립 및 시행
 - 정보보호 공시 업무 (정보보호산업법)
 - 기반보호법상 정보보호책임자 업무
 - 전자금융거래법상 CSO 업무
 - 개인정보보호법상 개인정보 보호책임자(CPO) 업무
 - 기타 정보보호 관련 법령상 업무

### [보안] ISMS-P(Information Security Management System – Privacy)

**[정의]**

조직의 정보자산 보호뿐 아니라 개인정보의 수집·이용·보관·파기 등 흐름 전반에 대한 보호체계를 포함한 통합 인증 제도 
 1\. 관리체계 수립 및 운영(16)
 1.1 관리체계 기반 마련 (6)
 1.2 위험관리 (4)
 1.3 관리체계 운영 (3)
 1.4 관리체계 점검 및 개선 (3)
 2\. 보호대책 요구사항(64)
 2.1 정책, 조직, 자산 관리 (3)
 2.2 인적보안 (6)
 2.3 외부자 보안 (4)
 2.4 물리보안 (7)
 2.5 인증 및 권한 관리 (6)
 2.6 접근통제 (7)
 2.7 암호화 적용 (2)
 2.8 정보시스템 도입 및 개발 보안 (6)
 2.9 시스템 및 서비스 운영관리 (7)
 2.10 시스템 및 서비스 보안관리 (9)
 2.11 사고 예방 및 대응 (5)
 2.12 재해복구 (2)
 3\. 개인정보 처리단계별 요구사항(21)
 3.1 개인정보 수집 시 보호조치 (7)
 3.2 개인정보 보유 및 이용 시 보호조치 (5)
 3.3 개인정보 제공 시 보호조치 (4)
 3.4 개인정보 파기 시 보호조치 (2)
 3.5 정보주체 권리보호 (3)

**[핵심/키워드]**

정통망법 제47조, 개인정보보호법 제32조의2
 (개인정보 보호 인증) 
 ISMS, ISMS-P, ISMS 예비인증

### [보안] ISO/IEC 27001

**[정의]**

정보보호 관리체계(ISMS)의 구축, 구현, 유지 및 지속적인 개선을 위한 요구사항을 규정한 국제 표준

**[핵심/키워드]**

요구사항 : 표준의 범위, 참조 표준, 용어와 정의, 조직의 상황, 리더십, 기획, 지원, 운영, 성과 평가, 개선 
 
 도메인/카테고리 : 정보보호 정책, 정보보호 조직, 인적 보안, 자산 관리, 접근 통제, 암호화, 물리적 및 환경 보안, 운영 보안, 통신 보안, 시스템 획득·개발·유지보수, 공급자 관계, 사고 관리, 사업 연속성 관리, 준수

### [보안] ISO/IEC 27014

**[정의]**

정보보안 거버넌스를 효과적으로 수립·유지·모니터링하기 위한 원칙과 모델을 제공하는 국제 표준

**[핵심/키워드]**

책임, 전략, 확보, 성과, 준수 
 평가, 지시(방향 설정), 모니터링, 소통, 정책 일치, 보증

### [보안] CSPM(Cloud Security Posture Management, 보안 형상관리)

**[정의]**

클라우드 환경에서 설정 오류, 정책 미준수, 보안 취약점을 자동으로 점검·분석하고 수정하여, 보안 상태(Posture)를 지속적으로 관리하는 솔루션 또는 기능 체계

**[핵심/키워드]**

컴플라이언스 모니터링, DevOps 통합, 설정 모니터링, 자산 인벤토리 관리, 위험도 평가, 사고 대응

### [보안] 망분리

**[정의]**

외부의 악성코드 침입을 막고 내부 정보의 유출을 막기 위해 내외부 인터넷 사용 공간을 다른 네트워크로 분리한 환경

**[핵심/키워드]**

- 정보통신망법 시행령 : 제15조의2 (정보통신서비스 제공자의 기술적·관리적 보호조치
 - 전자금융감독규정 (금융위) : 제15조의2 및 제18조 
 
 물리적 망분리 : 2pc, kvm스위치
 논리적 망분리 : SBC, CBC, 터미널 기반
 
 다중계층보안, 국가망 보안 체계

### [보안] 정보보호공시제도

**[정의]**

- 기업이나 기관이 자율적으로 수행한 정보보호 수준과 정보보호 투자 현황 등을 외부에 공개하는 제도
- 정보보호산업법 제13조

**[핵심/키워드]**

&lt;공시대상&gt; 
- 자율 공시 :  정보통신망 기반 정보제공자
- 의무 공시 대통령령 기준 충족 기준, ISP·IDC·상급종합병원·클라우드 제공자(사업분야), 매출 3,000억 이상 상장법인(매출 기준), 일일 이용자 수 100만명 이상(이용자 수 기준) 

&lt;공시항목&gt; 
- 정보보호 투자 현황, 정보보호 인력 현황, 인증·평가·점검 사항, 정보보호 활동 현황

### [보안] IAM(Identity Access Management)

**[정의]**

사용자의 신원(Identity)을 확인하고, 해당 사용자에게 적절한 자원 접근 권한을 부여 및 관리하는 보안 프레임워크

**[핵심/키워드]**

IAM = EAM + 감사 + 정책 + Provisioning (사용자 계정과 권한의 생성·배포·회수·삭제 자동화)

### [보안] FIDO2(Fast Identity Online2)

**[정의]**

FIDO 1.0의 모바일 앱 중심에서, PC 운용체계(OS)나 웹 브라우저에서 FIDO 인증 장치를 인식해 서비스하는 인증체계

**[핵심/키워드]**

WebAuthn, ASM/CTAP, Relying Party, Authenticator, Client, UAF/U2F

### [보안] OpenID Connect (OIDC)

**[정의]**

OAuth 2.0 기반으로 사용자 신원(ID) 확인 및 ID토큰을 활용하여 프로필 정보 제공 할 수 있는 사용자 인증(Authentication) 프로토콜

**[핵심/키워드]**

- OAuth 확장: 인증 정보를 포함한 ID Token 사용
  - 사용자 정보 포함: 로그인한 사용자 정보 확인 가능
  - JWT 기반: 경량 구조로 모바일/웹 모두 적합

### [보안] 전자봉투 (Digital Envelope)

**[정의]**

데이터를 비밀키(대칭키, 세션키)로 암호화하고, 해당 비밀키를 수신자의 공개키로 암호화하여 안전하게 전달하는 하이브리드 암호화 방식

**[핵심/키워드]**

전자서명, 비대칭키(RSA), 비밀키, 수신자 공개키, 수신자 개인키

### [보안] HMAC(Hash-based Message Authentication Code

**[정의]**

해시 함수(SHA-1, SHA-256 등)를 이용해서 비밀키와 메시지를 섞어 MAC을 생성하는 단방향 암호화 방식

**[핵심/키워드]**

- 비밀키 기반 : 해시값 생성 시 비밀키 사용 → MAC과 달리 키 없이는 위조 불가
 - 중첩 구조(2번 해시) : 내부해시, 외부해시 
 
 메시지(M), 비밀키(K), 해시 함수(H), ipad, opad, 내부 해시 결과, 최종 HMAC 결과

### [인공지능] 인공지능 신뢰성 인증(CAT, Certification of Artificial Intelligence)

**[정의]**

민간 인증 전문기관인 한국정보통신기술협회(TTA, Telecommunications Technology Association)가 AI기술을 활용해 민간 제품과 서비스의 위험요인을 분석하고 신뢰성 확보를 위한 사업자의 요구사항 준수 여부를 평가하는 제도 

CAT 2.0 : 국제표준 ISO/IEC 23894, ISO/IEC 42001, ISO/IEC 38507 

23894(제품/서비스): AI 제품의 위험관리 체계 + 성능 시험 병행 평가
42001(조직): AI 개발·운영 조직의 PDCA 기반 경영시스템 심사
38507(조직): AI를 도입·활용하는 조직의 거버넌스 구조 검증

&lt;인증대상&gt;  
‘제품·서비스’, ‘조직’ 두 가지로 구성

**[핵심/키워드]**

&lt;핵심속성&gt; 
안전성(Safety)
설명가능성(Explainability)
투명성(Transparency)
견고성(Robustness)
공평성(Fairness) 

&lt;인증대상&gt;  
‘제품·서비스’, ‘조직’ 두 가지로 구성

&lt;23894 인증항목&gt;  
- AI 위험관리 프레임워크 평가 : 설계 ~ 개선
- AI 위험관리 프로세스 평가 : 위험 평가/처리, 대응, 문서화

&lt;42001 인증항목&gt; 
- 조직 맥락
- 리더십
- 계획
- 운영
- 성과 평가
- 개선 등

&lt;38507 인증항목&gt;   
- 거버넌스 유지
- 책임 분배
- 정책 수립
- 의사결정·데이터 관리
- 문화·가치·법 준수·위험관리

### [보안] 클라우드 보안 인증제도(Cloud Security Assurance Program, CSAP)

**[정의]**

클라우드컴퓨팅 서비스의 정보보호 수준을 정부가 인증하는 제도로, 공공기관이 안전한 클라우드 서비스를 이용하도록 보장하기 위한 제도

**[핵심/키워드]**

최초(5년)-사후(5년동안 매년)-갱신(5년연장) 
인증등급제 : 상(물리)/중(물리)/하(논리/물리) 
인증기준 : 
 - 기존 인증제도 : IaaS, SaaS (표준등급), SaaS (간편등급), DaaS
 - 등급제 시행 이후 : 하등급(공통), 하등급 SaaS 

통제 항목 :  
 - 정보보호 정책, 정보보호 조직, 내부인력 보안, 외부인력 보안, 정보보호 교육, 자산 식별 및 분류, 자산 변경관리, 위험관리, 공급망 관리정책, 공급망 변경관리, 침해사고 대응 절차 및 체계, 침해사고 대응, 사후관리, 장애대응, 서비스 가용성, 법 및 정책 준수, 보안 감사, 물리적 보호구역, 정보처리 시설 및 장비보호, 가상화 인프라, 가상 환경, 접근통제 정책, 접근권한 관리, 사용자 식별 및 인증, 네트워크 보안, 데이터 보호, 매체 보안, 암호화, 시스템 분석 및 설계, 구현 및 시험, 외주 개발 보안, 시스템 도입 보안, 관리적 보호조치, 물리적 보호조치, 기술적 보호조치

### [인공지능] 데이터 산업진흥 및 이용촉진에 관한 기본법 (약칭: 데이터산업법)

**[정의]**

데이터의 생산·거래·활용을 촉진하여 경제적 가치를 창출하고 데이터산업 발전의 기반을 마련하는 법

**[핵심/키워드]**

제1장 총칙 (제1조 목적, 제2조 정의, 제3조 국가 등의 책무, 제4조 기본계획, 제5조 시행계획, 제6조 국가데이터정책위원회, 제7조 시행계획, 제8조 지원의 원칙)

제2장 데이터 생산·활용 및 보호 (제9조 데이터의 생산 활성화, 제10조 데이터 결합 촉진, 제11조 데이터 품질관리 등, 제12조 데이터산업의 보호, 제13조 데이터산업 활용 정보분석 지원)

제3장 데이터 이용 활성화 (제14조 가치평가 등, 제15조 데이터 이동성 촉진, 제16조 데이터사업자 신고, 제17조 공정한 유통질서 조성 등)

제4장 데이터 유통·거래 촉진 (제18조 유통 및 거래 체계 구축, 제19조 플랫폼에 대한 지원, 제20조 품질관리 등, 제21조 표준지원, 제22조 자료 제공 요청, 제23조 인재양성 지원)

제5장 데이터산업 기반 조성 (제24조 산업 육성 지원, 제25조 전문인력 양성, 제26조 기술개발·촉진 및 실증사업 지원, 제27조 투자활성화, 제28조 국제협력, 제29조 지역진흥, 제30조 세계지표 등, 제31조 진흥전략·계획, 제32조 전문기관 지정·운영, 제33조 협의체 설립)

### [보안] 양자과학기술 및 양자산업 육성에 관한 법(약칭.양자기술산업법)

**[정의]**

양자과학기술(통신·센서·컴퓨터 등)의 연구기반 조성과 양자 산업의 체계적 육성을 위한 종합체계를 구축하기 위한 법('24.11.1.시행)

**[핵심/키워드]**

제1장 총칙 - 제1조(목적), 제2조(정의), 제3조(국가 등의 책무), 제4조(다른 법률과의 관계)

제2장 양자과학기술 및 양자산업 육성을 위한 추진체계 - 제5조(양자종합계획의 수립), 제6조(시행계획의 수립·시행), 제7조(양자전략위원회 설치), 제8조(실태조사 등), 제9조(정보체계 구축·운영), 제10조(영향분석 및 대응)

제3장 양자과학기술 및 양자산업에 대한 지원 및 기반조성 - 제11조(연구개발의 추진), 제12조(연구개발 특례), 제13조(전용실시권의 설정), 제14조(상용화 촉진), 제15조(표준화 추진), 제16조(창업 및 기업육성), 제17조(양자팹 지원), 제18조(연구센터 지정), 제19조(문화 확산 장려), 제20조(지자체의 지원)

제4장 양자과학기술 및 양자산업 분야의 인력 양성 - 제21조(인력 양성사업의 지원), 제22조(전문교육기관 지원), 제23조(해외 인력 유치·활용), 제24조(기본계획 수립)

제5장 양자클러스터 지정 등 - 제25조(개발계획 수립 및 지정), 제26조(계획 변경 및 해제), 제27조(성과점검), 제28조(행정·재정 지원), 제29조(국제협력 지원)

제6장 협력 강화 - 제30조(해외 연구센터 유치), 제31조(산학연 협력 촉진)

### [인공지능] ROUGE (Recall-Oriented Understudy for Gisting Evaluation)

**[정의]**

- 자동 문서 요약 및 기계 번역의 성능을 평가하는 대표적인 지표로, 요약된 텍스트가 원본 문서와 얼마나 유사한지를 재현율(Recall)을 중심으로 측정하는 기법 

BLEU (Bilingual Evaluation Understudy)는 정밀도 중심  

텍스트 요약(Summarization) 평, N그램 기반 혹은 문장레벨 평가 까지 버전 존재

**[핵심/키워드]**

&lt;유형&gt; 
ROUGE-N
ROUGE-L
ROUGE-W
ROUGE-S
ROUGE-SU 

&lt;절차&gt; 
참조 문장 &생성 문장 준비
n-그램 추출
n-그램 비교 및 매칭 개수 계산
ROUGE N 점수 계산
 =  참조 문장에서 등장한 n-그램 중, 생성 문장에서 일치한 n-그램 개수 / 참조 문장 전체에 포함된 n-그램 개수

### [보안] 서비스 거부 공격 - DDoS(Distributed Denial of Service)

**[정의]**

다수의 공격자(좀비 PC, 봇넷 등)를 이용해 동시에 특정 서버나 네트워크에 과도한 트래픽을 발생시켜 정상적인 서비스를 방해하는 공격
(가용성 저해) 

&lt;유형&gt; 
 - DRDoS, Ransom DDos, Multi-Vector DDos

**[핵심/키워드]**

&lt;절차&gt; 
1\. 악성코드 은닉
2\. 악성코드 감염(좀비 PC, Agent 감염)
3\. 감염 사실 은폐 및 명령 대기
4\. DDoS 공격 수행 (공격자의 C&C 서버에 의한 제어)

&lt;대응방안&gt; 
-ACL 적용, 공격 IP 차단, SYN Proxy 사용, 보안 패치/장비 교체, 서버 설정 변경, 웹서버 증설, 불필요한 서비스 차단, 공격자 IP 차단, DNS 서버 다중화, DNS 전용회선 준비, IP 필터링, 지리적 차단, 의심 트래픽 필터링, 트래픽 이상 감지, AI 기반 분석 도입, Blackhole/Sinkhole 라우팅

### [인공지능] ISO/IEC TR 29119-11

**[정의]**

- AI 기반 시스템을 도입하고 테스트하는 방법에 대한 지침을 제공하는 ISO/IEC의 기술 보고서(Technical Report) 
- 29119 소프트웨어 테스트 표준과 연계, 데이터 학습 과정, 모델의 의사결정 로직, 성능 평가 방법

**[핵심/키워드]**

&lt;구성&gt; 
1\. Scope(적용 범위)
2\. Normative references(규범적 참조 문헌)
3\. Terms, definitions and abbreviated terms(용어, 정의 및 약어)
4\. Introduction to AI and testing(AI 및 테스트 소개)
5\. AI system characteristics(AI 시스템 특성)
6\. Introduction to the testing of AI-based systems(AI 기반 시스템 테스트 소개)
7\. Testing and QA of ML systems(머신러닝(ML) 시스템 테스트 및 품질 보증)
8\. Black-box testing of AI-based systems(AI 기반 시스템의 블랙박스 테스트)
9\. White-box testing of neural networks(신경망의 화이트박스 테스트)
10\. Test environments for AI-based systems(AI 기반 시스템의 테스트 환경)

11\. 블랙박스테스트 : 조합, 백투백, A/B테스트, 변성 테스트 

12\. 화이트박스테스트 : 뉴런 커버리지, 임계점 커버리지, 부호 변경 커버리지, 값 변경 커버리지, 부호-부호 커버리지, 레이어 커버리지

### [보안] 스니핑(Sniffing)

**[정의]**

- 네트워크 상에서 송수신되는 데이터를 몰래 엿보는 행위
- 주로 패킷 분석 도구를 이용해 사용자의 ID, 비밀번호, 민감정보 등을 비인가 수집하는 패시브(비활성) 공격

**[핵심/키워드]**

&lt;스니핑종류&gt; 
- 패스워드 스니핑, 세션 하이재킹 기반 스니핑, 이메일 스니핑, FTP 스니핑, DNS 스니핑, VoIP 스니핑, Telnet/SSH 스니핑, ARP 스푸핑 기반 스니핑, 브로드캐스트 스니핑 

&lt;대응방안&gt; 
- 탐지 도구 사용: Promiscuous 모드 탐지를 위해 sniffchk, AntiSniff 등 도구 활용
- ARP 모니터링: 비정상 MAC 변경 및 ARP 조작 감지를 위해 ARP 알림 시스템 적용
- NIC 모니터링: NIC 수신 범위 이상 여부를 OS 명령어로 점검
- 포트 미러링 감지: 스위치 포트 미러링 설정을 정책 기반 시스템으로 감시
- 이상 트래픽 분석: 갑작스러운 트래픽 증가를 IDS/IPS, NetFlow로 분석
- 강제 인증/암호화: 평문 통신 방지를 위해 HTTPS, TLS 등 암호화 적용
- 스위치 기반 전환: 허브를 스위치로 교체해 트래픽 노출 차단
- MAC 접근 제어: 불법 장비 차단을 위해 Port Security, 802.1X 인증 활용
- VPN 도입: 무선/공용망 환경에서 종단 간 암호화를 위한 VPN 도입
- 패킷 감시 정책 강화: 내부 사용자 감청 방지를 위해 DLP, UEBA 등 적용

### [인공지능] ModelOps(Model Operations)

**[정의]**

- AI 및 머신러닝 모델의 운영, 거버넌스, 리스크 관리, 성능 최적화를 담당하는 프로세스
- 모델의 규제 준수, 신뢰성, 성능 모니터링, 지속적인 개선이 목표

- MLOps + DataOps + 거버넌스 및 규제 준수

**[핵심/키워드]**

&lt;역할 및 주요 기능&gt; 
모델 거버넌스(Model Governance)
성능 최적화(Performance Optimization)
AI 윤리 및 공정성(AI Ethics & Fairness)
운영 모니터링(Operational Monitoring)
모델 재현 가능성 (Reproducibility & Versioning)
리스크 관리 및 규제 준수(Risk & Compliance Management)
AI 모델 배포(Model Deployment & CI/CD)
자동화된 A/B 테스트 (Automated A/B Testing)

### [보안] 스푸핑(Spoofing)

**[정의]**

- 공격자가 허위 정보를 조작하거나 위조하여 자신을 다른 사용자나 시스템으로 가장하는 공격 기법

**[핵심/키워드]**

&lt;유형&gt; 
- IP 스푸핑, ARP 스푸핑, DNS 스푸핑, ICMP Redirect 공격, 이메일 스푸핑, 웹사이트 스푸핑, MAC 스푸핑 

&lt;대응방안&gt; 
- IP 스푸핑: Ingress 필터링으로 위조된 IP 패킷 차단
- ARP 스푸핑: 정적 ARP 설정 및 DAI(Dynamic ARP Inspection) 적용
- DNS 스푸핑: DNSSEC(DNS Security Extensions) 적용으로 응답 위조 방지
- ICMP Redirect 공격: ICMP Redirect 메시지 수신 차단
- DDoS 공격: 트래픽 필터링, 속도 제한(Rate Limiting), DDoS 전용 방어 장비 도입

### [인공지능] 검색 통합 생성(Retrieval-Integrated Generation, RIG)

**[정의]**

- LLM의 성능을 향상시키기 위해, 모델이 응답 생성 과정 중에 실시간으로 데이터베이스와 상호작용 하는 방식  (필요한 정보를 검색하여 생성 과정 중 필요시, 업데이트)
- LLM이 자체 파라미터에만 의존하지 않고, 실시간 검색 결과를 반영해 더 정확하고 최신성 있는 응답을 생성

**[핵심/키워드]**

&lt;응답 생성 절차&gt; 
① 사용자 질문 입력 → ② 프롬프트 생성 → ③ 정보 검색 및 추출 → ④ 부분 응답 생성(LLM)→ ⑤ 최종 응답 생성 → ⑥ 사용자에게 응답 전달 


RAG는 고정된 검색 결과를 생성에 활용하는 선형적 방식,
RIG는 생성 도중에도 검색을 반복하는 상호작용적 방식으로 정확성과 맥락 이해에 더 강함

### [보안] WPA3

**[정의]**

- WPA2의 취약점을 보완하고, 최신 Wi-Fi 환경에서 더욱 강력한 보안성과 개인정보 보호를 제공하기 위해 2018년 Wi-Fi Alliance가 발표한 차세대 무선랜 보안 표준

**[핵심/키워드]**

&lt;동작과정&gt; 
 - SAE로 사용자 인증 수행 (WPA2의 PSK 대체)
 - 인증 결과로 PMK 생성
 - 4-Way Handshake 수행 → PTK, GTK 생성 및 교환
 - 데이터 전송 시 GCMP를 통해 암호화 및 무결성 검증 수행
 - 관리 프레임은 PMF를 통해 별도로 암호화 보호 

&lt;구성요소&gt; 
- SAE(ECC), AES-GCMP(AES + HMAC), PMK, PTK, GTK, 4-Way Handshake, PMF

### [인공지능] 전문가 혼합 모델(Mixture of Experts, MoE)

**[정의]**

- 여러 개의 전문가 네트워크(Expert Network)를 두고, Gating Network가 특정 입력에 적합한 전문가를 선택하여 최적의 결과를 도출하는 모델
- 여러 전문가 모델(Experts) 중 일부만 선택적으로 활성화하여 입력을 처리하는 딥러닝 아키텍처

**[핵심/키워드]**

입력(Query) → 게이트 네트워크(Gate Network) → 전문가 네트워크(Experts) 선택 → 로드 밸런싱(Load Balancing) → 추론 레이어(MoE Layer) → 출력(Output) 

&lt;MoE 딥러닝 모델&gt;
Google Switch Transformer
- MoE 구조를 대규모 트랜스포머에 적용한 최초 사례 중 하나 - 최대 1조 파라미터 모델에서도 소수 전문가만 활성화하여 효율 유지
GShard (Google)- 기계번역 등 대용량 작업을 위해 다중 전문가를 선택적으로 활성화하는 시스템

### [보안] SSRF(Server-Side Request Forgery)

**[정의]**

- 공격자가 서버 측에서 실행되는 요청 기능(예: URL 호출)을 조작하여, 서버가 내부 또는 외부 자원에 요청을 보내도록 유도하는 공격 
- 서버가 공격자의 프록시처럼 동작하게 만들어 내부 시스템 스캔, 민감 정보 접근 등을 시도함

- OWASP TOP 10, CSRF, XSS

**[핵심/키워드]**

&lt;공격절차&gt; 
1\. 조작된 요청 생성 (Attacker)
2\. 방화벽 우회 (Firewall)
3\. 취약한 웹사이트가 요청 실행 (Vulnerable Website)
4\. 내부 서버 접근 (Internal Server)
5\. 정보 유출 (Data Leak) 

&lt;대응방안&gt; 
- Whitelist Filtering, Blacklist Filtering, ACL 설정, 망분리, 공격징후 탐지, 로그/모니터링 강화, 최소권한 사용

### [인공지능] LWM (Large World Model, 대규모 세계 모델)

**[정의]**

- 물리적 환경을 이해하고 시뮬레이션하는 AI 모델(로봇, 자율주행, AI 기반 시뮬레이션 등에 활용) 

LWM은 물리 AI의 한 형태 또는 하위 범주로 간주될 수 있음
→ "물리 세계를 학습 기반으로 모델링하는 물리 AI"

물리 AI는 물리 법칙을 더 명시적으로 사용하는 반면, LWM은 경험 데이터를 통해 법칙을 암묵적으로 학습

두 방식은 상호 보완적이며, 실제 로봇이나 자율주행 AI 시스템에서는 함께 적용되기도 함

**[핵심/키워드]**

- 환경 시뮬레이션, 로봇 학습, 예측 모델링
- 센서 데이터, 영상, 3D 공간 정보
- 자율주행, 로봇, AI 시뮬레이션
- 현실 환경을 정확히 모델링하고 예측하는 문제
- 센서 데이터, 물리 엔진 시뮬레이션 데이터
- 환경 예측, 3D 공간 시뮬레이션
- 현실 환경과의 일치도, 예측 정확도
- Tesla FSD, Google DeepMind’s Simulated AI

### [보안] IAST (Interactive Application Security Testing)

**[정의]**

- 애플리케이션 실행 중 내부 코드 흐름과 외부 요청/응답을 동시에 분석하여 정적 + 동적 분석을 결합한 보안 테스트 기법 
- 정적 + 동적 보안취약점 분석 테스트 
- 런타임 시 애플리케이션 내부에 센서(Agent)를 삽입해 코드 수준 추적 + 요청 이벤트 분석을 병행 
- DevSecOps, DevOps

**[핵심/키워드]**

&lt;주요 매커니즘&gt; 
- 코드 실행 여부(실행함), 테스트 위치(내부 흐름 + 외부 요청 동시 분석), 정확도(높음), 적용 시점(개발~테스트 연속 가능), 통합 가능성(DevSecOps 최적화), 대표 도구(Contrast, Seeker, Veracode IAST)

### [인공지능] 에이전틱 AI (Agentic AI)

**[정의]**

- 사용자의 명확한 지시나 명령 없이도 스스로 작업을 수행하는 자율적인 소프트웨어(가트너2025)
- &lt;특징&gt; : 자율성, 목표지향성, 계획 수립 능력, 지속적 상호작용 및 피드백, 학습 및 적응력

**[핵심/키워드]**

User (사용자)
AI Agent
LLM (대형 언어 모델)
Database (DB)
Vector DB
(벡터 데이터베이스)
Action (행동 수행 모듈)
Model Customization (모델 맞춤화)
Data Flywheel (데이터 플라이휠) 

인식 (Perceive)
- 데이터 수집, 특징 추출, 멀티모달 데이터 처리, 실시간 데이터 스트리밍
추론 (Reason)
- LLM 기반 추론, RAG, 지식 그래프, 강화학습, 상황 인식 AI
행동 (Act)
- 목표 설정, API 연동, 클라우드 서비스 실행, 로봇 및 IoT 제어, 작업 자동화
학습 (Learn)
- 피드백 루프, 데이터 큐레이팅, 모델 재훈련, 지속 학습, SaaS 기반 학습
성능 관리 (Self-Governance)
- IoT 연동, 자율 의사결정, Explainable AI, AI 보안 및 신뢰성, 데이터 거버넌스

### [보안] 서비스형 랜섬웨어(Ransomware as a Service, RaaS)

**[정의]**

- 전문 해커가 개발한 랜섬웨어 도구를 다른 범죄자에게 서비스 형태로 제공하고, 감염 수익을 공유하는 사이버 범죄 비즈니스 모델 
- RaaS 운영자는 툴을 제공하고, 사용자(affiliate)는 공격을 실행

**[핵심/키워드]**

&lt;유형&gt; 
- 구독형(Rental)
- 수익 공유형(Affiliate)
- 혼합형 

&lt;사례&gt; 
- 갠드크랩 (GandCrab)
- REvil (Sodinokibi)
- LockBit 

&lt;대응방안&gt; 
- 보안 정책 및 백업 체계 수립
- 버그바운티 프로그램 운영
- 랜섬웨어 대응 시나리오 및 대응계획 수립
- 주기적인 백업 복구 테스트 및 모의훈련 수행
- 사용자 권한 최소화 및 외부기기 제한
- 보안 인식 교육 정기적 시행
- 업무용 PC·노트북 보안 점검 및 통제
- 방화벽, IDS/IPS, 보안관제체계 운영
- 행위 기반 탐지 (EDR, SandBox 등)
- WAF 및 웹 보안관제 적용 (웹서비스 대응)
- SIEM(보안정보 이벤트 통합관리) 구축
- 보안 개발 생명주기(Secure SDLC) 적용
- 애플리케이션 화이트리스트 적용 (실행 통제)
- 백신(Anti-Virus) 및 최신 보안 패치 적용
- 주기적 백업 및 백업 데이터 무결성 검증

### [인공지능] 물리 AI (Physical AI,  피지컬AI)

**[정의]**

- 인공지능(AI)이 물리적 환경에서 직접 동작하며, 감각, 학습, 행동을 수행하는 시스템
- 가상공간(디지털트윈, 메타버스)과 실제 물리환경에서 학습한 지능을 기반으로 현실 세계에서 인식, 판단, 행동을 수행하는 인공지능 기술

**[핵심/키워드]**

센싱 시스템: 카메라, Lidar, IoT 센서
컴퓨터 비전: 온디바이스 비전 AI, 모델 경량화
강화학습:  강화학습(RLHF, PPO 등)
자연어 처리: 소형 LLM(sLLM)
엣지 AI : 온디바이스 AI, AI 전용 칩셋
액추에이션 시스템 : 액추에이터 제어 기술
통신 기술 : 5G/6G 통신, 초저지연 IoT 네트워크
피지컬 AI 개발 F/W : LWM, Tokenizer, 디지털트윈, 메타버스, AI 가속기
데이터베이스: 벡터DB
서비스: 자율주행차, 휴머노이드 로봇

### [보안] APT(Advanced Persistent Threat)

**[정의]**

- 특수목적을 가진 공격자가 피해 대상을 표적으로 삼고 다양한 IT기술과 방식들을 이용해 지속적으로 정보를 수집하고 취약점을 파악하여 이를 바탕으로 피해를 끼치는 공격 

&lt;특징&gt; 
지능성 (Advanced)
지속성 (Persistent)
목표지향성 (Targeted)
조직성 (Organized)

**[핵심/키워드]**

&lt;공격절차&gt; 
침입(Incursion): 사회공학, 제로데이 취약점, 수동 공격, 탐색
탐색(Discovery): 관찰, 탐색, 다중 벡터, 은밀한 활동, 연구 및 분석
수집(Capture): 수집, 은닉, 권한 상승
유출 및 제어(Exfiltration & Control): 유출/제어, 유출, 중단 

&lt;대응방안&gt; 
관리적 대응: 보안관리 및 운영, 보안교육 강화, 위협 인텔리전스 활용, 침해사고 대응 체계 수립
기술적 대응: 엔드포인트 보안, EDR/XDR 도입, DLP 및 중요정보 암호화, 계층형 방어
접근 및 권한 관리: 접근권한관리, 다단계 인증(MFA), 네트워크 접근 제어(NAC)

