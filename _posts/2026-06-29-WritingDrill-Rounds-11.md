---
layout: post
title: "WritingDrill_Rounds_11"
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

### [인공지능] 가디언 에이전트(Guardian Agent)

**[정의]**

AI시스템의 안전성,신뢰성,윤리성 확보를 위해 AI를 감시·감독·제어하는 보조 AI 또는 시스템

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

### [인공지능] 검색 증강 생성 기술 RAG&lt;div&gt;(Retrieval-Augmented Generation)&lt;/div&gt;

**[정의]**

- 언어모델관점 정의: 대규모 언어 모델에서 질문에 대한 답변이나 텍스트를 만들기 전에 광범위한 문서 집합에서 관련 정보를 질의하고, 이를 이용하여 응답을 생성하는 방법
- 환각 해소관점의 정의: 기존 텍스트 생성 모델의 사실적 오류, 문맥 부족, 정보 누락 등의 문제점을 개선하기 위해, 검색 결과를 통해 이러한 문제점을 보완하고 보다 정확하고 풍부한 텍스트를 생성하는 매커니즘

**[핵심/키워드]**

* RAG 모델 3가지 메커니즘(기고모)
- 기본(Native) RAG: 검색 모델을 사용 데이터 수집하고 청크로 분할하여 임베딩 후 Vector DB에 저장
- 고급(Advanced) RAG: 기본RAG의 부족한 점을 개선하기 위해 3단계로 수행하는 매커니즘
- 모듈형(Modular) RAG: 다양한 모듈과 기능 통합하여 패턴화하고, 시나리오, 요구사항에 맞게 조정 가능한 메커니즘

### [인공지능] 국가 AI역량 강화 방안

**[정의]**

4대 AI 플래그십 프로젝트(인공지능 3대 강국(AI G3) 도약) --&gt; 국가 AI역량 강화 방안  
&lt;정의&gt; 
- 국가 차원의 인공지능(AI) 경쟁력 확보를 위한 종합 전략으로, AI 인프라·기술·인재·산업 생태계를 전방위적으로 강화하기 위한 정부 주도 정책 방안

**[핵심/키워드]**

① AI컴퓨팅 인프라 확충&lt;/font&gt;
-단기(즉시~단기): 중앙·지자체·민간 협력 기반 3단계 AI 마스터플랜 이행
-중기(2026년): 최첨단 GPU 1만개 규모의 국가 AI컴퓨팅센터 구축
-장기(2030년): 국산 AI반도체 50% 이상 도입 목표
-재정 구조 혁신: 민간 투자 활성화 및 정부 R&amp;D(30~50%), 투자펀드(15~35%) 조성
② 차세대 AI모델 개발&lt;/font&gt;
-독자 AI모델 개발·고도화를 위한 생성형 AI 연구개발 집중 지원
-초거대 AI 모델 및 AI 반도체 최적화 기술 개발 추진
-글로벌 경쟁력 확보형 AI 모델 개발 생태계 구축
③ AI전환 가속화&lt;/font&gt;
-공공·산업 전반 AI 서비스 확산: 교육·의료·행정·산업 분야에 AI 접목
-AI전환 지원 플랫폼 구축: 중소기업·지자체 대상 AI 활용 지원
-AI 신뢰성·윤리성 확보: 데이터 품질, 보안, 신뢰성 인증체계 강화

### [인공지능] 근사 최근접 이웃탐색(Approximate Nearest Neighbor, ANN)

**[정의]**

고차원 벡터에서 입력한 벡터와 유사한 이웃을 빠르게 찾는 근사 검색 기법

**[핵심/키워드]**

&lt;알고리즘&gt; 
- HNSW&lt;/font&gt;: 계층형 그래프 기반 탐색으로 정확도 매우 높고 실시간 검색에 적합
- IVF&lt;/font&gt;: 벡터를 K-means 클러스터링하여 검색 범위를 줄이는 방식
- PQ&lt;/font&gt;: 벡터를 압축·양자화해 연산량 감소, IVF와 자주 병행
- ScaNN&lt;/font&gt;: IVF + PQ + Rerank(재정렬) 방식의 구글 고성능 벡터 검색 알고리즘
- ANNOY&lt;/font&gt;: 랜덤 트리 기반 디스크 검색, 속도 빠르나 정확도는 중간

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

### [인공지능] TurboQuant

**[정의]**

- 긴 문맥 추론: KV Cache가 메모리 병목을 해결 하기위해, LLM 추론 시 KV Cache 압축에 적합하도록 설계된 경량·온라인 적용형 알고리즘

**[핵심/키워드]**

1단계: PolarQuant &lt;/font&gt;기반 데이터 분포 단순화 수행 
2단계: QJL&lt;/font&gt;(Quantized Johnson-Lindenstrauss) 기반 압축 과정 오차 보정 

상세 절차 
- 입력 벡터 수집 → 랜덤 회전 전처리 → 극좌표 변환 → 스칼라 양자화 1차 압축 → 잔차 오차 계산 → JL 기반 1비트 보정 압축 → 최종 압축 표현 생성

### [인공지능] LiteLLM

**[정의]**

- 다양한 LLM을 하나의 API로 호출할 수 있는 오픈소스 Python 라이브러리 및 프록시 서버 
 - 여러 인공지능 모델(OpenAI, Anthropic, Gemini 등) 연동 복잡성 제거

**[핵심/키워드]**

구조: Python SDK 기반 단일 코드 호출 지원, Proxy Server/AI Gateway 기반 중앙 관리 및 라우팅 제공
핵심 기능: API 표준화 지원, 요청 라우팅 및 모델 전환 지원, 자동 fallback 기반 장애 시 대체 모델 호출 지원
운영 기능: 비용 추적 지원, Rate Limit·Budget 관리 지원, 로깅 및 모니터링 기반 운영 현황·장애 추적 지원
기술 특징: LLM 연동 지원, OpenAI 호환 API 제공, Load Balancing 및 Failover 지원
활용 방식: 멀티 모델 실험 및 비교 활용, 기업 내부 인공지능 Gateway 구축 활용, Agent/워크플로우 통합 활용
장점: 벤더 종속성 감소, 모델 교체 용이, 비용 최적화 가능

### [인공지능] 로지스틱 회귀분석(Logistic Regression Analysis)

**[정의]**

분석 대상들이 여러 집단으로 나누어진 경우, 독립변수의 선형 결합을 이용하여 개별 관측치가 어느 집단에 속하는지 확률을 계산하는 분류기법

**[핵심/키워드]**

1) 확률의 선형 모델 표시
2) 오즈(odds)적용: 양의값 무한대
3) 로짓(Logit)적용: 음의값 무한대
4) 판별 함수: 선형함수 사용
5) 시그모이드: 로짓함수의 역함수

### [인공지능] 마르코프 모델

**[정의]**

- 시간의 경과와 상태변화를 표현하고 외부 입력이나 이벤트가 발생할 때 유한 패턴 안에서 상태를 변화시키는 모델 
- 현재 상태가 미래 상태를 결정하고, 과거 이력은 현재 상태에 모두 반영되었다고 가정하는 확률 기반 상태 전이 모델

**[핵심/키워드]**

*마르코프 체인(성질): n+1회의 상태가 오로지 n회 상태에만 영향을 받음
*이상 시간 확률 과정: 시간흐름에 변화 

구성 요소:
– 상태(State): 시스템이 가질 수 있는 상황
– 전이확률(Transition Probability): 한 상태에서 다른 상태로 이동할 확률
– 초기확률(Initial Probability): 시작 상태의 확률 분포
– 관측값(Observation): 상태에 따라 나타나는 출력값(은닉모델일 때)

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
  ㄴ Vision-LanguageModel(VLM)기반 생성 
  ㄴ DiffusionModels(이미지/영상 생성) 
  ㄴ 다양한 출력 형식 지원

### [인공지능] 메타휴리스틱스 (Metaheuristics)

**[정의]**

- 최적화 문제를 해결하기 위한 상위 개념의 탐색 기법 이며, 완전 탐색(Exhaustive Search) 대신 근사 최적해(Approximate Solution)를 찾는 알고리즘 
- 다양한 문제 도메인에 적용 가능한 일반화된 최적화 기법

**[핵심/키워드]**

&lt;주요 기법&gt; 
- 단일 해 기반 기법: 시뮬레이티드 어닐링(SA), 탭 서치(TS), 확률적 탐색(Randomized Search)
- 집단 기반 기법: 유전자 알고리즘(GA), 개미 군집 최적화(ACO), 입자 군집 최적화(PSO)
- 하이브리드 기법: GRASP(Greedy Randomized Adaptive Search Procedure), MA(Memetic Algorithm)

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
- 잠재 공간 (LatentSpace)  
- 변분 추론 (VariationalInference)  
- 재매개변수화 트릭(ReparameterizationTrick) 
- KL-발산 (KL-Divergence) 
- ELBO(EvidenceLowerBound)  
- 재구성 손실 (ReconstructionLoss)

### [인공지능] 생성형 인공지능(AI)개발/활용을 위한 개인정보 처리 안내서

**[정의]**

생성형 AI 서비스 개발‧운영 과정에서 개인정보 보호 리스크를 최소화 하고, 개인정보보호법 준수 기반으로 투명하고 안전한 AI 생태계 마련한 안내서

**[핵심/키워드]**

&lt;적용 범위&gt; 
- 모델 개발자, 모델 이용자  
&lt;단계&gt; 
- 목적 설정
- 전략 수립
- AI 학습 및 개발
- 시스템 적용 및관리
- AI 프라이버시거버넌스 구축

### [인공지능] 생성형 AI데이터품질관리가이드 v2.0&nbsp;&lt;div&gt;&nbsp;1) 데이터구축과정 2) 품질지표&lt;/div&gt;

**[정의]**

- 생성형 AI 데이터 품질관리 가이드라인은 생성형 인공지능(Generative AI) 학습에 활용되는 데이터의 정확성, 다양성, 대표성, 안전성, 법적 준수성을 확보하기 위한 표준 지침서 
- 1.0(초거대AI데이터) --&gt; 2.0(-LLM, LMM, 합성데이터의 특성 및 품질관리 지표 추가)
&lt;생성형AI의 주요 모델&gt; 
  - 거대 언어 모델(LLM), 거대 멀티 모달 모델(LMM), 
  - 소형 거대 언어 모델(sLLM), 온디바이스AI 모델, 버티컬AI(Vertical AI)
&lt;주요 학습 방식&gt;
  - 지도학습, 비지도학습, 강화학습, 적응 학습(파인튜닝, 특징추출, 전이학습)   
&lt;생성형 AI 데이터&gt; : 대규모 학습 데이터, 멀티모달 데이터, 파인튜닝 및 강화 학습, 데이터셋 관리

**[핵심/키워드]**

1) 데이터구축과정  
- 구축계획 수립, 데이터 획득/수집, 데이터 정제, 데이터 가공, 데이터 학습, 데이터 구축 및 학습 반복
2) 품질지표 
- 구축 공정 적정성 : 준비성, 완전성, 유용성, 기준 적합성, 
- 데이터 적합성 : 다양성, 유사성(중복성), 편향성(유해성), 합성데이터 유용성, 합성데이터 안전성, 
- 가공 데이터 정합성 : 구문 정확성, 의미 정확성(전달성), 
- 학습모델 적합성 : 알고리즘 적정성, 유효성

### [인공지능] 선형 판별분석(Linear Discriminant Analysis, LDA)

**[정의]**

클래스 간 분산(between-class scatter)과 클래스 내 분산(within-class scatter)의 비율을 최대화하여, 독립변수들의 측정값에 따라 데이터가 어느 집단에 속할 것인가에 대해 판별하는 분석 방법

**[핵심/키워드]**

분류분석, 차원축소, 클래스 간 분산(between-class scatter)과 클래스 내 분산(within-class scatter)의 비율을 최대화 
 - 공통된(동일한) 공분산 행렬을 가지는 다변수 정규분포 가정 
 &lt;절차&gt; 
 - 클래스 평균 계산 -→ 클래스 내 분산 행렬 SW 계산 -→ 클래스 간 분산 행렬 SB 계산 -→ 판별 벡터 W계산 
 
 - PCA :데이터의 분산을 최대화하는 축 기준 
 - QDA : 클래스별로 서로 다른 공분산 행렬 사용

### [인공지능] 소버린 AI(SovereignAI)

**[정의]**

&lt;소버린AI 정의&gt; 
- 국가 또는 특정 지역이 데이터/AI 인프라 모델을 독립적으로 통제하고 운영할 수 있도록 하는 AI 주권 확보 전략 
- 국가 AI 역량 강화 방안 (2025.2)

**[핵심/키워드]**

- 데이터 주권: 소버린 클라우드, 로컬 데이터 허브
- 모델 주권: 자국어 LLM, 도메인 특화 모델
- 컴퓨팅 자립: 국산 AI 반도체, 국산 클라우드 인프라
- AI 알고리즘: 국산 프레임워크, 다국어 알고리즘
- 보안/투명성: XAI 기술, AI 감사 시스템
- AI 운영 기술: 모델 경량화, 저전력 추론
- 오픈소스 전략: 공개 모델 활용, 공동 개발 체계

### [인공지능] 앙상블 알고리즘 (Ensemble Algorithms)

**[정의]**

일련의 분류 기준을 구성한 후 예측 가중치 투표를 통해 새로운 데이터를 분류하는 방식

**[핵심/키워드]**

&lt;특징&gt;
- 성능 향상, 과적합 방지, 편향-분산 트레이드오프 최적화, 모델 안정성 향상
&lt;유형&gt; 
- 동일모델(데이터 다양성 부여): 보팅, 배깅(랜던포레스트), 부스팅
- 여러개 모델 결합(알고리즘 다양성 부여): 보팅, 스태킹, 블랜딩

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

### [인공지능] 엣지 AI(Edge AI)

**[정의]**

데이터가 생성되는 디바이스 또는 인근 네트워크 엣지에서 AI 모델을 직접 실행하여 분석·처리하고, NPU·TPU·FPGA 등 전용 AI 가속기와 모델 경량화·최적화 기술을 활용하는 기술

**[핵심/키워드]**

&lt;엣지AI 기술요소&gt; 
- 하드웨어 기술 : 전용 AI 칩셋(NVIDIA Jetson, Google Edge TPU, 
Qualcomm AI Engine)
- AI 모델 경량화·최적화 : TensorFlow Lite, ONNX, PyTorch Mobile
- MEC 아키텍처: MEC 참조 아키텍처(ETSI)
- 실시간 데이터 처리·추론 최적화 : NVIDIA TensorRT, &nbsp;Intel OpenVINO, 
Qualcomm SNPE
- 네트워크 융합 기술 : 5G·IoT·MEC 결합 
&lt;엣지 컴퓨팅 기반 생성형 AI 이점 &gt; 
- 실시간/저지연성
- 데이터 프라이버시·보안 강화
- 맞춤형 개인화
- 네트워크 비용 절감
- 에너지 효율성

### [인공지능] 지능형 엣지 컴퓨팅(IntelligentEdgeComputing)

**[정의]**

- 엣지 AI+네트워크 제어 +데이터 분석/처리 기능을 통합한 차세대 분산 컴퓨팅 구조 
- 엣지 AI에서 한 단계 발전 →엣지 노드 자체가 지능화되어 AI추론·분석,네트워크 제어,자원 관리까지 수행

**[핵심/키워드]**

– MEC, 경량 AI 추론엔진, 모델 경량화, 스트리밍 분석, SDN/NFV, 5G, 연합학습, Edge MLOps, Zero Trust 중심 기술로 구성됩니다.

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
 5️⃣ 모델 업데이트 및 재배포(Global Model Update &amp; Redistribution) 
 
 모델 결합 알고리즘 
 -FedSGD (Federated Stochastic Gradient Descent)
 - FedAvg (Federated Averaging)
 - FedProx (Federated Proximal)
 - FedOpt (Federated Optimization)
 - FedMA (Federated Matched Averaging)
 - FedBN (Federated Batch Normalization)
 - FedGKT (Federated Gradient Knowledge Transfer)
 - FedReID (Federated Learning for Person Re-identification)

### [인공지능] 오토마타 이론 (AutomataTheory)

**[정의]**

- 형식 언어(Formal Language)와 입력을 받아 상태를 변경하는 수학적 모델을 연구하는 학문
- 컴퓨터 과학에서 알고리즘, 언어 인식, 계산 가능성을 분석하는 이론

**[핵심/키워드]**

&lt;구성요소&gt; 
- 오토마톤, 상태(State), 형식 언어(Formal Language), 전이 함수(Transition Function), 입력(Input)과 출력(Output)

결정적 유한 오토마타 (DFA) , 비결정적 유한 오토마타 (NFA) 

오토마톤 → 오토마타 → 유한 오토마톤 → 스택 오토마톤 → 튜링머신

### [인공지능] 의사결정나무(Decision Tree)

**[정의]**

분류함수를 의사결정규칙으로 표현할 때 타원, 직선, 사각형을 이용하여 나무형태로 그려서 분석하는 도구 
- 분류나무트리 -&gt; 범주형 
- 회귀나무트리 -&gt; 연속형

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

### [인공지능] 이미지 캡셔닝(ImageCaptioning)

**[정의]**

- 이미지에서 객체, 배경, 동작 등의 시각적 요소를 분석한 후, 이를 자연어 문장으로 설명하는 기술

**[핵심/키워드]**

&lt;구성요소&gt; 
- 이미지 특징 추출기, 언어 모델, 어텐션 메커니즘, 디코더(캡션 생성기), 데이터셋 
&lt;유형&gt; 
- 오토 캡셔닝, 휴먼 캡셔닝, 맥락 기반 캡셔닝, 객체 레벨 캡셔닝, 질의 응답 캡셔닝, 스토리텔링 캡셔닝, 구조화된 캡셔닝, Dense 캡셔닝, Sparse 캡셔닝

### [인공지능] 자기조직화 지도(Self-Organizing Map,&nbsp;&lt;div&gt;= 코헤넨 맵, Kohonen map)&lt;/div&gt;

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

### [인공지능] Mamba

**[정의]**

– 상태공간모델(SSM) 기반 시퀀스 모델로, Transformer의 Self-Attention 병목을 줄이기 위해 설계된 선형 복잡도 중심 아키텍처

**[핵심/키워드]**

동작 관점:
– 입력 시퀀스를 모두 서로 비교하는 대신, 현재 입력과 이전 상태를 이용해 정보를 갱신
– 중요한 정보만 선택적으로 반영하는 Selective State Space 구조 사용
– 긴 문맥에서도 KV Cache 부담 없이 시퀀스 처리 가능
주요 특징: 
– Self-Attention 미사용 또는 최소화 
핵심 기술요소:
– SSM(State Space Model)
– Selective Scan
– State Update
– Gating
– Linear-time Sequence Modeling
– Convolution + Recurrence 결합 구조
– Hardware-aware Parallel Algorithm 
Transformer 대비 포인트:
– Transformer: 전체 토큰 간 관계 계산, O(n²) 복잡도, KV Cache 부담 큼
– Mamba: 상태 기반 순차 갱신, O(n) 복잡도, 긴 시퀀스에 유리

### [인공지능] 전문가 혼합 모델(Mixture of Experts, MoE)

**[정의]**

여러 개의 전문가 네트워크(ExpertNetwork)를 두고,GatingNetwork가 특정 입력에 적합한 전문가를 선택하여 최적의 결과를 도출하는 모델

**[핵심/키워드]**

- Input Layer: 외부 입력을 벡터로 임베딩하거나 전처리)
- Gating Network: 입력을 분석해 적합한 Expert 후보를 Softmax 또는 Top-k 방식으로 선택
- Load Balancing Loss: 특정 Expert에 쏠림 방지를 위해 활용도를 균등하게 유지
- Top-k Routing: Gating 점수 상위 k개의 Expert만 선택해 활성화, 연산 효율성 확보
- Expert Layer: 선택된 Expert들이 독립적으로 연산 수행, MLP 또는 Transformer 블록 구성
- Inference Layer: 활성화된 Expert들의 출력값을 Gating 가중치로 통합
- Out Layer: 분류·생성 등 목적에 맞춘 최종 출력 생성&lt;/moe&gt;

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

### [인공지능] 지식증류(Knowledge Distillation)

**[정의]**

대규모 모델(교사 모델, Teacher Model)이 학습한 지식을 소규모 모델(학생 모델, Student Model)로 전이하여, 성능은 최대한 유지하면서 모델의 크기와 계산 복잡도를 줄이는 기술

**[핵심/키워드]**

LLM성능향상, 모티모달(융합 모듈), 경량화 
 - Teacher / Student 모델 
 - Soft Labels 학습(Temperature 조절 --&gt; 클래스 확률분포) 
 - Soft Labels 모방 
  ① Distillation Loss(KL Divergence)&lt;/font&gt; : Teacher와 Student 모델 출력의 차이
  ② Student Loss(L1/L2 Norm)&lt;/font&gt; : 실제 레이블과 Student 모델 출력의 차이

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
  ㄴ ResidualConnection&amp;LayerNormalization 
  ㄴ PositionalEncoding
- 디코더 
  ㄴ Encoder-DecoderAttention 
  ㄴ MaskedSelf-Attention 
  ㄴ Softmax &amp;LinearTransformation

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
 양자화 및 이진화 (Quantization &amp; Binarization)
 가중치 공유 (Weight Sharing)
 파라미터 효율적 미세 조정 (PEFT, Parameter Efficient Fine-Tuning)
 희소성 유도 (Sparsity Induction)
 지연된 가중치 업데이트 (Delayed Updates)

### [인공지능] 퓨샷러닝 (Few-Shot Learning)

**[정의]**

적은 양의 데이터로 모델을 학습하여 테스트 데이터에서 유의미한 성능을 얻고자 하는 딥러닝 알고리즘

**[핵심/키워드]**

* 적은 양 데이터
* 데이터셋 : support, query
* 기술 : 전이학습, 메터학습, 거리학습, 액티브러닝, 생성모델
* 동작 : train-test 분리, 샘플링, support, query 분리, 학습, 평가

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

### [인공지능] 혼동 행렬(Confusion matrix = 오분류표)

**[정의]**

분류 모델의 성능을 평가하는 데 사용되는 중요한 도구

**[핵심/키워드]**

&lt;구성요소&gt;
- 정확도(Accuracy): (TP + TN) / (TP + TN + FP + FN)
- 정밀도(Precision): TP / (TP + FP)
- 재현율(Recall): TP / (TP + FN)
- 특이도(Specificity): TN / (TN + FP)

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

### [인공지능] Agent2Agent(A2A)

**[정의]**

- JSON-RPC 2.0 기반 메시징을 활용하여  서로 다른 AI Agent 간의 통신 및 협업을 위한 표준 프로토콜

**[핵심/키워드]**

&lt;설계원칙&gt; 
- 에이전트 능력 수용, 기존 표준 기반 개발, 기본 보안 보장, 장기 실행 작업 지원, 모달리티 독립적 설계 
&lt;동작 과정&gt; 
- 발견 → 요청 → 처리 → 상호작용 → 완료/알림 단계로 동작하며 
&lt;핵심요소&gt; 
- 에이전트 메타 정보: Agent Card, Agent Discovery
- 통신 주체: A2A 서버, A2A 클라이언트
- 작업 단위: Task(작업), Task Lifecycle
- 메시지 구조: Message, Part, Artifact
- 통신 및 확장 기능: 통신 프로토콜, Streaming, Push Notifications, 고급 기능

### [인공지능] AgenticRAG

**[정의]**

- 에이전트(agent)가 주도적으로 목표를 설정하고, 검색→생성→피드백→행동을 반복하는 능동적 RAG 프레임워크 
- 기존 RAG 모델에 에이전트(Agent) 자율성을 부여하여 정보 검색, 추론, 행동 결정을 스스로 수행하도록 확장한 구조

**[핵심/키워드]**

&lt;절차&gt; 
입력(Query)이 들어오면 → Router Agent가 요청을 분석 → 각 Retrieval Agent(X, Y, Z)가 적합한 Data Source (Vector DB, Web, Mail, Chat 등)에서 검색 수행 → 결과를 LLM Core로 전달 → 응답(Response) 생성 
&lt;구성 레이어&gt; 
Agent Layer: 질의 분석과 검색 오케스트레이션 담당
RAG Core Layer: 검색·생성의 중심 처리
Evaluator Layer: 품질 검증과 피드백 루프 관리
 
Agent Layer: Retrieval Router Agent, Retrieval Agent X/Y/Z, Action / Tool Agent
RAG Core Layer: Retriever, Re-ranker, Generator(LLM), Vector DB
Evaluator / Feedback Layer: Self-Evaluator, External Evaluator, Memory Module

### [인공지능] AI 네이티브 개발 플랫폼&lt;div&gt;(AI-Native Development Platforms)&lt;/div&gt;

**[정의]**

&lt;개념&gt; 
- 생성형 AI(Generative AI)를 사용하여, 소프트웨어를 이전보다 빠르고 쉽게 개발 할 수 있도록 바이브코딩 및 AI 에이전트를 지원하는 소프트웨어 개발 플랫폼 (가트너 기술전략 2026) 
&lt;부각배경&gt; 
– 복잡한 SW 개발, 생산성 한계
– 생성형 AI·Agent 기반 개발 확산
– DevOps → AI 기반 자동화 진화

**[핵심/키워드]**

&lt;구성 요소&gt;
– 요구/프롬프트 입력 → LLM 코드 생성 → 테스트·검증 → CI/CD 배포 → 피드백 학습 기반 End-to-End 자동화 구조
&lt;핵심 기술&gt;
– LLM(Code LLM) + Prompt/Context Engineering + AI Agent(MAS) + MLOps/AIOps + RAG/Vector DB 통합 기술 스택
&lt;아키텍처&gt;
– Input → AI 모델(생성/추론) → Tool/Agent 실행 → CI/CD 배포 → Feedback Loop 기반 Closed Loop 구조

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

### [인공지능] AI기본법

**[정의]**

- 인공지능 기술의 발전과 활용에 따라 발생하는 다양한  사회적, 윤리적, 법적 문제를 해결하기 위해 제정된 법률 
- 2024년 12월 26일 국회 본회의를 통과하였으며, 2025년 1월 21일에 공포(2026년 1월 시행)

**[핵심/키워드]**

제2조(정의)
- 인공지능, 고영향 AI, 생성형 AI 등 11개 용어 정의
- 고영향 인공지능: 생명·신체·기본권에 중대한 영향, 12개 활용 영역 명시 
제6조(인공지능 기본계획 수립)
- 3년마다 기본계획 수립
- 전략, 윤리, 재원 등 포함
제12조(인공지능안전연구소)
- 위험 대응 위한 안전연구소 설치·운영
제13조(기술 개발 및 안전한 이용 지원)
- 기술개발·실용화 및 안전한 이용 지원 
제14조(기술의 표준화)
- 인공지능 기술 표준 제정·보급
제15조(학습용데이터 시책 수립)
- 학습데이터 정책 수립 및 시스템 구축
제27조(인공지능 윤리원칙 등)
- 윤리원칙 제정 및 실천방안 마련
- 생명 보호, 접근성, 공헌 등
제30조(안전성·신뢰성 검증 지원)
- 자율 검증·인증 활동 지원
제31조(투명성 확보 의무)
- 생성형 AI 결과물 표시 등 고지 의무
제32조(안전성 확보 의무)
- 고성능 AI 안전 확보 및 위험 관리
제33조(고영향 AI 확인 절차)
- 고영향 여부 사전 검토 및 확인 요청 가능

### [인공지능] AI기본법(인공지능 발전과 신뢰 기반 조성 등에 관한 기본법) 시행령

**[정의]**

- 인공지능의 건전한 발전을 지원하고 인공지능사회의 신뢰 기반 조성에 필요한 기본적인 사항을 규정 한 시행령

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

### [인공지능] DBSCAN Clustering(Density-based spatial clustering of applications with noise)

**[정의]**

- 데이터 포인트의 밀도를 이용해 군집을 형성하고, 이상치(Noise)를 효과적으로 식별하는 비지도학습 알고리즘
 - 반달모양(Moon-Shaped) 비구형 데이터 셋 군집

**[핵심/키워드]**

&lt;하이퍼파라미터&gt; 
  - MinPoints, Epsilon 
&lt;탐색 기준&gt; 
  - 코어, 노이즈, 보더 
&lt;단점 및 해결 알고리즘&gt; 
  - 하이퍼파라미터 설정에 민감, 밀도 다른 경우 군집 어려움 --&gt; OPTICS 알고리즘(유동적 Epsilon 사용) 
OPTICS (Ordering Points To Identify the Clustering Structure)

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
  
 Spectral GNN : 주파수 도메인에서 변환
 Spatial GNN : 직접 이웃 노도 정보 학습 
   
  -GCN (Graph Convolutional Network)
 - ChebNet (Chebyshev Graph Convolutional Network)
 - Spectral CNN 
 
 - GraphSAGE (Graph Sample and Aggregate)
 - GAT (Graph Attention Network)
 - MPNN (Message Passing Neural Network)
 - GIN (Graph Isomorphism Network)&lt;/spatial&gt;&lt;/spectral&gt;&lt;/gnn&gt;

### [인공지능] K-평균 군집(K-Means Clustering)

**[정의]**

데이터의 유사성을 기반으로 최적의 중심점을 찾아 K개의 그룹으로 분류하는 방법

**[핵심/키워드]**

&lt;절차&gt;
1) 군집 수 K를 정의하여 임의 위치 지정(initial Centroids)
2) 모든 데이터들의 거리 계산 후 가장 가까운 중심점 기준으로 군집화 
3) 각 군집마다 계산하여 새로운 중심 계산 
4) step 2~3을 반복, 클러스터가 변경되지 않으면 학습 완료

### [인공지능] KNN(K-Nearest Neighbor)

**[정의]**

새로운 데이터 포인트(Test Data)가 주어졌을 때, 기존 학습 데이터(Training Data)와의 거리를 측정하여 가장 가까운 K개의 이웃을 찾고, 다수결 또는 평균을 이용하여 예측하는 비모수적(Non-Parametric) 지도 학습 알고리즘 
- Lazy Learning, 비모수적 모델

**[핵심/키워드]**

- 분류 문제: 가장 많은 속성을 가진 클래스로 분류 (다수결 투표)
- 회귀 문제: K개의 이웃의 평균값을 사용하여 예측
 - 비모수적 모델, 메모리기반학습(레이지 러닝: 학습 불필요)
 &lt;절차&gt;
 - 거리 계산 --&gt; 가장가까운 k개 데이터 선택 --&gt; 보팅(분류), 평균(회귀)
 * 장점
  간단하고 효과적, 기본적인 분포가정 필요없음, 학습과정 빠름
  * 단점
  모든 데이터와 거리계산 필요, 새로운 인사이트를 얻는데 제한

### [인공지능] MLPerf (MachineLearningPerformanceBenchmark)

**[정의]**

- 다양한 하드웨어와 소프트웨어 플랫폼에서 머신러닝 워크로드의 성능을 객관적이고 공정하게 측정할 수 있는 벤치마크 표준
- 2018년 하버드, 스탠포드, UC 버클리 등 주요 대학과 Google, NVIDIA, Intel 등 기업들이 공동으로 개발

**[핵심/키워드]**

MLPerf Training
MLPerf Inference
MLPerf Mobile
MLPerfHPC 
MLPerfTiny

### [인공지능] Physical AI

**[정의]**

- 인공지능(AI)이 물리적 환경에서 직접 동작하며, 감각, 학습, 행동을 수행하는 시스템
- 가상공간(디지털트윈, 메타버스)과 실제 물리환경에서 학습한 지능을 기반으로 현실 세계에서 인식, 판단, 행동을 수행하는 인공지능 기술

**[핵심/키워드]**

- 센싱 시스템: 카메라, Lidar, IoT 센서
- 컴퓨터 비전: 온디바이스 비전 AI, 모델 경량화
- 강화학습: 강화학습(RLHF, PPO 등)
- 자연어 처리: 소형 LLM(sLLM)
- 엣지 AI: 온디바이스 AI, AI 전용 칩셋
- 액추에이션 시스템: 액추에이터 제어 기술
- 통신 기술: 5G/6G 통신, 초저지연 IoT 네트워크
- 피지컬 AI 개발 F/W: LWM, Tokenizer, 디지털트윈, 메타버스, AI 가속기, SimToReal
- 데이터베이스: 벡터DB
- 서비스: 자율주행차, 휴머노이드 로봇

### [인공지능] SVM  (Support Vector Machine)

**[정의]**

데이터 포인트를 고차원 공간에서 분리하는 최적의 결정경계(Decision Boundary)를 찾아주는 지도 학습(Supervised Learning) 알고리즘

**[핵심/키워드]**

* 구성요소
  - Margin
  - Support Vector
  - Hyper-plane 
  - 하이퍼 파라미터 : C(Regularization Parameter), 허용 오차 (ξ), Epsilon (ε, SVR에서 사용) = 𝜀-Tube (Epsilon-Tube)
 * 학습 유형 : 분류, 회귀 
 * 분류 설정 
  - 좁은 마진(큰 C값), 오분류 허용 X (하드 마진) 
  - 넓은 마진(작은 C값), 오분류 허용 O (소프트 마진) 
 * 비선형 처리 --&gt; Kernel 함수(=커널트릭) 이용 
  - 선형, 다항, RBF, 시그모이드

### [인공지능] XAI(eXplainable AI)

**[정의]**

사용자가 인공지능 시스템의 동작과 최종 결과를 이해하고 올바르게 해석하여 결과물이 생성되는 과정을 설명 가능하도록 해주는 기술

**[핵심/키워드]**

알고리즘의 조작 가능성, 의사결정의 편향성 , 머신러닝 AI에 대한 신뢰성 입증 한계 &lt;= 해결 목표 
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

### [인공지능] 옴니모달 AI

**[정의]**

&lt;정의&gt; 
– 텍스트, 이미지, 음성, 영상, 행동 등 모든 모달 데이터를 단일 모델에서 통합 학습·처리하는 AI 구조 
– 모달별 분리 처리 후 결합하는 멀티모달과 달리 → 공유 잠재 공간(Shared Latent Space) 기반으로 입력부터 출력까지 통합 처리
– 멀티모달 : “여러 모달을 연결(Fusion)하는 구조”
– 옴니모달 : “모든 모달을 하나의 모델 안에서 통합 처리하는 구조” 
&lt;특징&gt; 
– 단일 Transformer 기반 통합 구조
– 공통 토큰화(Tokenization) 방식 적용
– Sequence-to-Sequence 통합 학습
– Interleaved 데이터 흐름(모달 혼합 시퀀스 처리)
– 입력·이해·생성의 일체형 구조

**[핵심/키워드]**

&lt;기술요소&gt; 
– 입력·토큰화 계층 : 공통 토큰화, 멀티모달 인코딩
– 공유 잠재 공간 : 모달 정렬, 공통 임베딩, 의미 통합
– 통합 모델 아키텍처 : 단일 Transformer, 통합 학습, Unified 모델
– 크로스모달 학습 : Matching, Translating, Referencing, Contrastive Learning
– 생성·출력 계층 : Multimodal Generation, VLM, Diffusion 기반 생성

### [인공지능] Affective AI

**[정의]**

- 인간의 감정, 기분, 정서 상태를 데이터로 인식·표현·반응하는 기술
- 단순 분류를 넘어 감정의 원인과 맥락을 이해하고, 인간과 유사한 정서적 상호작용 구현 지향
- (발전 방향): 초기 단일 신호 분류 
- 멀티모달 통합, 대규모 학습, 개인화 모델링으로 확장

**[핵심/키워드]**

* Affective AI 기술의 발전 단계
 - (1세대) 표정 · 음성 기반 감정 표현
 - (2세대) 멀티모달 감정인식, 실시간 상호작용
 - (3세대) 감정 예측, 개인화, 장기 정서 모델링 
* Affective AI 기술 동향 
 - 멀티모달 감정인식 기술
 - 맥락 기반 감정이해 기술
 - 감정의 불확실성 해소 기술
 - 감정 기반 의사결정 및 행동 생성 기술
 - 공감적 응답 생성 기술
 - 윤리 · 프라이버시를 고려한 Affective AI 기술

### [인공지능] Alignment AI

**[정의]**

AI Alignment  개념:
– AI의 행동과 결과가 인간의 가치·의도·목표와 일치하도록 만드는 기술·연구 분야
목적:
– AI가 의도와 다르게 행동하는 위험 방지
– 안전하고 신뢰 가능한 AI 시스템 구축
핵심 문제:
– 목표 불일치(Misalignment)
– 보상 해킹(Reward Hacking)
– 환각(Hallucination)
– 예측 불가능성
AI Alignment 주요원칙:
– RICE(견고성·해석가능성·제어가능성·윤리성) + 3H(유익성·정직성·무해성) 기반 안전·신뢰 AI 구현

**[핵심/키워드]**

주요 접근 방법:
– RLHF / RLAIF: 인간·AI 피드백 기반 정렬
– Constitutional AI: 규칙 기반 행동 제어
– Interpretability: 모델 내부 이해 가능성 확보
– Safety Guardrails: 정책·필터 기반 통제
구성 요소:
– 목표 정의(Objective)
– 보상 설계(Reward Design)
– 행동 제어(Policy Control)
– 평가 및 피드백(Evaluation Loop)
특징:
– 기술 + 윤리 + 정책 결합 영역
– 모델 성능보다 안전성·신뢰성 중시
– 지속적 학습 및 개선 필요
적용 영역:
– 생성형 AI(ChatGPT 등)
– 자율주행, 로보틱스
– 금융·의료 의사결정 AI

### [인공지능] RLHF, RLAIF

**[정의]**

RLHF 개념:
– 인간 평가자가 모델 출력에 대해 선호/품질 피드백을 제공하고 이를 강화학습에 반영 

RLAIF 개념:
– AI 모델이 다른 모델의 출력에 대해 자동 평가/피드백을 생성하고 이를 강화학습에 활용

**[핵심/키워드]**

RLHF 동작 구조:
– 인간 피드백 수집 → 보상모델(Reward Model) 학습 → RL로 모델 최적화 

RLAIF 동작 구조:
– 원칙설정(보상 기준) →  AI 평가 생성 → 보상모델 구성 → RL로 모델 개선

### [인공지능] AI 반도체의 성능 평가 지표

**[정의]**

- AI 학습·추론을 수행하는 반도체의 연산 처리 능력, 메모리 처리 특성 및 전력 효율을 정량적으로 측정하여 시스템 성능을 평가하기 위한 기준 체계

**[핵심/키워드]**

– TTFT(Time to First Token) : 첫 토큰 출력 시각 − 요청 시작 시각
– TPOT(Time per Output Token) : 총 디코딩 시간 ÷ 생성된 출력 토큰 수
– TPS per user(Tokens Per Second) : 처리된 토큰 수 ÷ 총 처리 시간
– TDP 평균 전력소모(Thermal Design Power) : 전 구간 소비전력 ÷ 측정 구간  
– FLOPS(Floating Point Operations Per Second) : 부동소수점 연산 횟수 ÷ 실행 시간
– TOPS(Tera Operations Per Second) : 정수 연산 횟수 ÷ 실행 시간
– Memory Capacity : 저장·처리 가능한 총 메모리 용량
– Memory Bandwidth : 전송된 데이터 양 ÷ 전송 시간
– Latency : 결과 출력 시점 − 요청 시점&lt;/ai&gt;

### [데이터분석] 결측값 (Missing Value)

**[정의]**

- 데이터 수집·입력·처리 과정에서 특정 변수의 값이 누락되어 존재하지 않거나 비어있는 상태

**[핵심/키워드]**

* 미존재
 * 원인 : 수집오류, 기록오류, 형식불일치 
 * 종류 : 완전무작위, 무작위, 비무작위
 * 표현 : NA, NaN, inf, NULL
 * 처리방법 : 삭제, 대치, 자체활용, 모델기반
 * 삭제 : 단일값삭제, 목록삭제(행/열)
 * 대치 : 완전분석, 핫덱, 콜드덱, 근접이웃, 비조건부평균, 조건부평균, 다중대치

### [데이터분석] 교차표분석

**[정의]**

두 범주형 변수간의 연관관계를 볼때 교차표(분할표)를 작성하여 변수들간 관계를 분석하는 기법 

- (관측값-기대값)^2/기대값

**[핵심/키워드]**

- 적합도 검정 , 독립성 검정, 동질성 검정 
 - 승산비 , 상대위험도(Relative Risk)

### [데이터분석] 다중공선성  (Multicollinearity)

**[정의]**

회귀분석에서 독립변수들 간에 강한 상관관계가 나타나는 문제

**[핵심/키워드]**

ρ(Xi, Xj) ≈ ±1
 확인(산포도, 상관계수, 허용/공차, 분산팽창지수(VIF &gt;=10))
 해결(무시, 변수제외, 변수통합,  FA, PCA, Ridge)

### [데이터분석] 대응표본 t-검정  (Paired t-test)

**[정의]**

같은 집단에서 두 번 측정된 값(또는 짝지어진 두 집단 : 이전 이후)의 평균 차이를 비교하는 통계적 검정 방법 

* 가정사항 : 정규성
 * 하나의 모집단 내부 두 집단 간 t-검정

### [데이터분석] 데이터 거버넌스 (Data Governance)

**[정의]**

데이터 자산을 관리하고 활용하기 위한 정책, 프로세스, 표준, 역할 및 책임을 정의하고 실행하는 체계

**[핵심/키워드]**

* 분석 관리 체계
 * 대상 : 마스터데이터, 메타데이터, 데이터사전, 빅브라더
 * 구성 : 원칙, 조직, 프로세스
 * 체계 : 표준화, 관라체계, 저장소 관리, 관리활동

### [데이터분석] 데이터 메시 (Data Mesh)

**[정의]**

- 도메인 중심의 분산형 데이터 관리방식(탈중앙화)을 적용하는 데이터 아키텍처 패러다임 
- 중앙 집중형 데이터 레이크의 한계를 극복하기 위해, 도메인 중심의 분산형 데이터 관리 방식(탈중앙화)을 적용하는
데이터 아키텍처 패러다임
- 각각의 분산 된 서비스 형태로 개발 관리하는 탈중앙형 데이터 아키텍처 모델

**[핵심/키워드]**

* 도메인 중심, 탈중앙화, 자율운영
 * 4원칙 : 도메인소유권, 데이터제품화, 셀프서비스, 연합형계산 
&lt;핵심요소&gt; 
- 도메인: 도메인 팀, 데이터 계약, 데이터 제품, 셀프서비스 데이터 플랫폼
- 플랫폼: 데이터 플랫폼 팀, 인터페이스/API
- 거버넌스: 연합형 거버넌스(Federated Governance)
- 지원조직: Enabling Team

### [데이터분석] 독립표본 t-검정  (Independent t-test)

**[정의]**

두 개의 독립적인 집단 간의 평균 차이를 검정하기 위한 통계적 방법 
- 서로 독립인 두 모집단의 모분산이 알려져 있지 않고, 두 모집단의 각각의 표본 크기 작은 경우(또는 𝑛1, 𝑛2&lt;30) 𝑡분포를 이용하여 검정 하는 방법

**[핵심/키워드]**

* 가정사항 : 독립성, 정규성, 등분산성
 - 서로 다른 두 집단 간 t-검정
 - 두 집단이 같은 모집단에서 나왔는지를 평균값을 기준으로 비교하는 가설검정 방법 
&lt;둥분산, 이분산 에 따라 통계량 산정 방법 상이&gt;

### [데이터분석] 모수통계, 비모수통계

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

### [데이터분석] 베이즈 정리

**[정의]**

사전적 확률을 구한후 확률에 영향을 미치는 변수의 확률을 반영하여 사후 확률을 구하는 방법 

𝑃(𝐴1|𝐵)=  P(B|A1)P(A1)/P(B) = (𝑃(𝐴1∩𝐵) / 𝑃(𝐵)

**[핵심/키워드]**

사전확률, 조건부확률, 사후확률
 확률의 곱셈법칙
 전확률, 확률계산, 베이즈 정리

### [데이터분석] 불균형 데이터 (Imbalanced Data)

**[정의]**

각 변수가 가진 데이터에서 각 집단에 속하는 데이터의 수가 동일하지 않은 상태의 데이터

**[핵심/키워드]**

* 집단간 데이터 불균형
 * 해결 : 오버샘플링, 언더샘플링
 * 오버샘플링(랜스보아) : 랜덤, 스모트, 보더라인 스모트, 아다신
 * 언더샘플링(랜토CO) : 랜덤, 토멕링크, CNN, OSS

### [데이터분석] 상관관계 분석

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

### [데이터분석] 유클리디안 거리 (Euclidean Distance)

**[정의]**

벡터 공간 내 두 노드 사이의 직선 거리를 이용하여 유사도를 산출하는 벡터 거리 기반 유사도 측정법

### [데이터분석] 이산확률분포, 연속확률분포

**[정의]**

&lt; 이산확률 분포 &gt;
- 확률 변수가 셀 수 있는 이산 값을 가질 때의 확률분포
&lt; 연속확률 분포 &gt;
- 확률 변수가 무한히 많은 연속 값을 가질 때의 확률분포

**[핵심/키워드]**

&lt; 이산확률 분포 &gt;
* 정수, 셀 수 있는 값, 특정 값 합산
* 확률 질량 함수 (PMF), 누적 질량 함수 (CMF)
* 유형 : 이산형 균등, 베르누이, 이항, 음이항, 기하, 초기하, 포아송
&lt; 연속확률 분포 &gt;
* 실수, 연속적인 값, 구간 단위 적분
* 확률 밀도 함수 (PDF), 누적 분포 함수 (CDF)
* 유형 : 연속형 균등, 정규, t, 감마, 지수, 카이제곱, F

### [데이터분석] 점추정 (Point Estimation)

**[정의]**

표본자료를 이용하여 모수의 참값이라고 추정되는 하나의 값을 결정하는 추정 기법

**[핵심/키워드]**

* 단일 값 추정
 * 4가지 준거 : 불편성, 유효성, 일치성, 충분성
 * 벙법 : 평균제곱오차, 적률법, 최대가능도

### [데이터분석] 최대우도추정법(Maximum Likelihood Estimation, MLE)

**[정의]**

- 관측된 데이터가 가장 자연스럽게 나올 수 있도록 하는 확률분포의 파라미터를 찾는 방법 

– 주어진 관측 데이터가 가장 높은 확률로 발생하도록 만드는 모수(parameter) 값을 추정하는 통계적 추정 방법

### [데이터분석] 추론통계 (Inferential Statistics)

**[정의]**

모집단으로부터 샘플을 추출, 분석하여 그 결과로부터 모집단에 대한 특성을 추론하는 과정

**[핵심/키워드]**

* 샘플 → 모집단
 * 표본기반 모집단, 통계적 가정
 * 기법 : 가설검정, 점추정, 구간추정, 회귀분석, 분산분석

### [데이터분석] 카프카(kafka)

**[정의]**

- 실시간 데이터 처리, 비동기 메시징, 데이터 파이프라인 구축을 위해 사용되는 고성능 메시지 브로커 
- 브로커 중심의 단일 계층 구조 
Kafka → 고성능 스트리밍 처리에 강점, 구조 단순하지만 확장 시 관리 복잡.
Pulsar → 저장 분리형 구조로 내구성·확장성 우수, 멀티테넌시·큐/스트림 통합 환경에 적합.(브로커와 BookKeeper가 분리)

**[핵심/키워드]**

* 발행, 구독 중심, 분산구조, 실시간처리 
* 구성 :producer, broker, message, topic, partition, consumer, offset, zookeeper 
- 데이터 모델  : 토픽, 파티션

### [데이터분석] 탐색적 데이터 분석(EDA, Exploratory Data Analysis)

**[정의]**

데이터 분석과정에서 수집된 데이터 입력 시 데이터의 구조, 특성, 패턴 등 넓은 시각에서 직관적으로 이해 및 관찰한 후 연구자의 가설 수립을 위한 분석 기법

**[핵심/키워드]**

1) 저항성 
 2) 잔차의 해석 
 3) 데이터의 재표현 
 4) 데이터의 현시성

### [데이터분석] 텍스트 마이닝 (Text Mining)

**[정의]**

비정형 텍스트 데이터에서 유용한 정보, 패턴, 지식을 자동으로 추출하고 발견하는 과정

**[핵심/키워드]**

* 기법 : 정보 추출, 문서분류(군집화), 문서요약, Concept Linkage:, Question Answering, Topic Tracking
 * 절차 : 데이터 수집/클리닝/반환 > 전처리 > 정보추출 > 클러스터링/범주화 > 요약/검색
 * 전처리 : 토큰화, 불용어, 형태소, 어간/어미, 대소문자 통일
 * 표현 : BoW, TF-IDF, Word Embedding, Doc2Vec
 * 마이닝 : 분류, 군집, 토픽모델링, 감성분석

### [데이터분석] 판다스(pandas)

**[정의]**

데이터조작과 분석을 위한 오픈소스 라이브러리로서 데이터 처리와 구조화된 데이터를 다루는데 최적화된 도구

**[핵심/키워드]**

* 파이썬, 데이터 처리 및 구조, 
 * 구조 : 시리즈, 데이터 프레임
 * 기능 : 결측값처리, 데이터 필터링, 다양한 형식, 시계열 데이터, 넘파이 통합

### [데이터분석] 포아송 분포 (Poisson Distribution)

**[정의]**

- 단위 시간 또는 공간 내에서 발생하는 사건의 개수를 모델링하는 이산확률분포

**[핵심/키워드]**

- 단위 시간/공간 내 발생 건수를 셈
- 사건은 서로 독립적
- 단위 내에서 평균 발생률(λ)은 일정
- 희박한 사건에 적합 (드물지만 일정하게 발생)
- 이항분포의 극한형태 

 * 가정 : 독립성, 비례성, 비집락성

### [데이터분석] 표준정규분포 (Standard Normal Distribution)

**[정의]**

표준화 확률변수 Z에 의해 변환 과정을 거쳐 평균이 0이고 표준편가 1로 정리된 정규분포

**[핵심/키워드]**

* 평균 0, 표준편차 1 정규분포 
* 종모양/ 좌우 대칭 
 * Z-값, Z분포표
 * 기댓값 0, 분산 1

### [데이터분석] 회귀분석

**[정의]**

하나 혹은 그 이상의 원인(독립변수)이 결과(종속변수)에 미치는 영향을 추정하여 식으로 표현할 수 있는 통계 기법

**[핵심/키워드]**

&lt;유형&gt; 
- 단순회귀분석 
- 다중회귀분석
- 비선형 회귀분석
- 로지스틱 회귀분석 

&lt;회귀식 검정&gt;   
- 회귀계수 추정 : •최소제곱법, 최대가능도법, 적률추정법 등 사용
- 모델 적합성 확인 : 분산분석(ANOVA)의 𝑭검정
- 모델 설명력 확인 : 결정계수(𝑹^𝟐) 
- 회귀계수 유의성 확인 : t검정  
- 다중공선성 : VIF  
- 회귀식의 영향력 진단 : 쿡의 거리, 레버리지 등

### [데이터분석] ANOVA/분산분석 (Analysis Of Variance)

**[정의]**

독립집단 3개 이상의 집단간 평균이 서로 차이가 있는지 확인하기 위한 검정 방법

**[핵심/키워드]**

* 통계량 : f =  MSE/MSE 
* 일원 분산분석, 이원 분산분석, 반복측정분산분석, 이원반복측정분산분석 

사후검정 
 - 튜키 HSD, 쉐페, 던칸, 본페로니, 피셔LSD

### [데이터분석] 대수의 법칙(Law of Large Numbers)과&nbsp;&lt;div&gt;중심 극한의 정리(Central Limit Theorem) 비교&lt;/div&gt;

**[정의]**

&lt;대수의 법칙과 중심 극한의 정리의 정의와 가정 사항 비교&gt;
- 대수의법칙: 동일한 확률분포에서 표본 수가 증가할수록 표본평균이 모평균에 수렴함을 설명하는 확률 법칙
 - 𝑛 → ∞ 일 때 표본평균 𝑋&nbsp;̅ → μ 

- 중심 극한의 정리: 동일한 확률분포에서 표본 수가 충분히 크면 표본평균의 분포가 정규분포로 수렴함을 설명하는 확률 법칙

### [데이터분석] 카이제곱 분포

**[정의]**

개념:
– 정규분포를 따르는 독립 변수의 제곱합이 따르는 분포 
- 정규화 된 오차의 크기를 측정

정의:
– 자유도  k인 카이제곱분포는 표준정규변수 𝑍𝑖의 제곱합

### [데이터분석] F-분포

**[정의]**

- 카이제곱분포 2개의 비율 확률 분포 
- 두 카이제곱분포의 비율로 정의되는 분산 비교용 분포
- 두집단의 산포를 비교하는데 이용  


활용:
– 분산 분석(ANOVA)
– 두 집단 분산 비교(F-test)
– 회귀모형 유의성 검정

### [데이터분석] 델타 아키텍처

**[정의]**

데이터 레이크(DataLake)기반으로 데이터를 단계적으로  정제하여 품질을 향상시키기 위해 기존 시스템을 유지하면서 변경(Delta)되는 부분만을 추가하거나 수정하는 방식의 아키텍처

**[핵심/키워드]**

Bronze Layer는 원천 원시 데이터 저장 계층,  
Silver Layer는 정제·표준화된 데이터 계층, 
Gold Layer는 분석·비즈니스 활용에 최적화된 큐레이션 데이터 계층

### [데이터분석] 가설검정

**[정의]**

모집단에 대해 세운 귀무가설(H0) 이 타당한지 표본 데이터를 근거로 검증하여, 기각할지 여부를 판단하는 통계적 의사결정 절차

**[핵심/키워드]**

검정요인:
– 귀무가설(H0): 변화 없음, 차이 없음, 효과 없음이라는 기본 가설
– 대립가설(H1): 차이 있음, 효과 있음, 관계 있음이라는 대안 가설
– 유의수준(α): 귀무가설 기각 기준이 되는 허용 오차 수준
– 검정통계량: 표본 데이터로 계산한 판단 수치(Z, t, F 등)
– 기각역/채택역: 검정통계량이 들어가는 구간에 따라 기각 또는 기각하지 않음 결정
– p값: 귀무가설이 참일 때 현재와 같은 극단적 결과가 나올 확률
– 결론: 검정통계량 또는 p값과 유의수준 비교를 통해 귀무가설 기각 여부 판단

### [데이터분석] 시계열분석(TimeSeriesAnalysis)

**[정의]**

– 시간의 흐름에 따라 순차적으로 수집된 데이터의 패턴(추세, 계절성, 순환, 불규칙)을 분석하여 미래 값을 예측하는 분석 기법

**[핵심/키워드]**

– 평활법: 과거 관측값에 가중치를 부여해 노이즈를 줄이고 미래 값을 예측하는 방법
– 분해법: 시계열을 추세, 계절성, 순환, 불규칙 요소로 분리해 분석·예측하는 방법
– 자기회귀모델(AR): 현재 값을 과거 자신의 값들의 선형 결합으로 설명하는 모델
– 이동평균모델(MA): 현재 값을 과거 오차항의 결합으로 설명하는 모델
– ARIMA: 자기회귀와 이동평균에 차분을 결합해 비정상 시계열을 예측하는 모델

