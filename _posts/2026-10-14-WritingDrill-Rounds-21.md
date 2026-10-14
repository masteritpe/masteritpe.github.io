---
layout: post
title: "WritingDrill_Rounds_21"
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

## [생성형AI] 양자화 (Quantization)



**[정의]**

모델의 Weight / Activation / KV Cache를 FP32 / FP16 같은 고정밀 표현에서 INT8 / INT4 등 저비트 표현으로 변환하는 경량화 기술

**[핵심/키워드]**

&lt;핵심원리&gt;  
 - 저비트 변환, Scale, Zero-point, Clipping

&lt; 유형 &gt;  
 - Weight Quantization : 가중치 저비트 변환  
 - Activation Quantization : Activation 저비트 변환  
 - Weight + Activation Quantization : Weight와 Activation 동시 양자화  
 - KV Cache Quantization : Key / Value Cache 압축  
 - PTQ(Post-Training Quantization) : 추가 학습 없이 양자화  
 - QAT(Quantization-Aware Training) : 양자화 오차 반영

&lt;대표기술&gt;  
 - GPTQ (GPT Quantization) : Weight PTQ, 사후 양자화  
 - AWQ (Activation-aware Weight Quantization) : 중요 Weight 정보 보호  
 - SmoothQuant : 분포 조정 W8A8 양자화  
 - QLoRA (Quntized Low-Rank Adaptation) : 4bit Quantization + LoRA  
 - TurboQuant : KV Cache / Embedding Vector 저비트

## [생성형AI] 터보퀀트 (TurboQuant)



**[정의]**

구글이 개발한 벡터 양자화 (VQ, Vector Quantization)기반의 AI 메모리 압축기술

**[핵심/키워드]**

&lt;등장배경&gt;  
 - LLM 서비스 확장, 장문 컨텍스트 확대, 인프라 비용 증가, 추론 최적화 필요성  
 - KV Cache 메모리, 연산 병목 문제 해결

&lt;2단계 압축 메커니즘&gt;  
 - 1단계 Polar-Quant : 정보 압축, 플립 회전 + 극좌표 변환, 스칼라 양자화  
 - 2단계, QJL : 정확도 보정, 압축 시 발생 오차를 저비트 방식 추가 보정, 1비트 보정

&lt;동작과정&gt;  
 1) 입력벡터 수집 > 2) 랜덤회전 (Hadamad) > 3) 극좌쵸 변환 (Polar Transform) > 4) 스칼라 양자화 (Lloyd-Max) > 5) 오차 계산 (잔차) > 6) JL 변환 (1비트 양자화) > 7) 최종 출력

&lt;인플라이트역양자화&gt;  
 - 연산 파이프라인에서 실시간 역양자화

&lt;적용효과&gt;  
 - 정확도 손실 없이 3비트 압축, 메모리 1/6감소, 연산 8배 가속

## [생성형AI] 맘바 (Mamba)



**[정의]**

입력에 따라 중요한 정보는 유지하고, 불필요한 정보는 잊는 선택적 상태 갱신 구조 기반의 시퀀스 모델

**[핵심/키워드]**

&lt;특징&gt;  
 - 선형시간 처리, 선택적 정보 처리, 긴 문맥 확장, Attention-Free  
 - Self-Attention 연산 및 메모리 한계 감소 / 대체, Selective SSM  
 - O(n) 시간복잡도 (n: 시퀀스길이) , 상태기반 공간복잡도 효율 증가

&lt;구성요소&gt;  
 - 입력 처리 : Input Embedding, Linear Projection  
 - 지역정보 추출 : ConvID  
 - 활성화 처리 : SiLU Activation  
 - 상태공간 처리 : Selective SSM, State Update  
 - 선택 제어 : Gating  
 - 출력 처리 : Output Projection  
 - 안정화 처리 : Residual Connection, Normalization

&lt;버전&gt;  
 - Mamba-1 : SSM  
 - Mamba-2 : SSD (상태공간 듀얼리티)  
 - Mamba-3 : 고차 수치적분, 추론효율 강화

## [생성형AI] 페이지드 어텐션 (Paged Attention)



**[정의]**

LLM 추론 시 KV Cache를 고정 크기 Block / Page 단위로 관리하여 메모리 낭비를 줄이는 기술

**[핵심/키워드]**

&lt;특징&gt;  
 - 가상메모리 페이징 기법 활용, KV 블록, 블록단위 공유  
 - 외부단편화 제거 및 내부 단편화 최소

&lt;구성요소&gt;  
 - KV 블록 (KV Block) : 고정크기 블록 분할  
 - 논리블록 (Logical Block) : 논리적 가상, 연속적  
 - 물리블록 (Physical Block) : 비연속적 저장공간, 실제 저장  
 - 블록 테이블 (Block Table) : 논리-물리 매핑  
 - 블록 관리자 (Block Manager) : 참조 카운터

&lt;주요기술&gt;  
 - Copy on Write : 쓰기 시점 복사, 분기시점에만 블록 복사  
 - Prefix Caching : 공통 프롬프트 KV 캐시 재사용  
 - Beam Search : 다중 후보 시퀀스 생성  
 - Gang Scheduling : 분산 / 병렬 연산 동시 실행  
 - Re-computation : 메모리 부족 시 재연산

&lt;활용&gt;  
 - vLLM (Virtual LLM) : Paged Attention 오픈소스 서빙 프레임워크  
 - Paged Flash Attention : Paged Attention + Flash Attention

## [생성형AI] 플래시 어텐션 (Flash Attention)



**[정의]**

기존 Self-Attention의 연산 결과는 유지하면서, GPU 메모리 접근방식을 최적화하여 Attention을 빠르고 메모리 효율적으로 수행하는 기술

**[핵심/키워드]**

&lt;특징&gt;  
 - GPU 메모리 IO 최소화, IO-Aware, Tile 단위 분할

&lt;효과&gt;  
 - HBM I/O 감소, 메모리 사용량 감소, 학습 / 추론 속도 향상

&lt;동작원리&gt;  
 - Tiling / Block Processing : Tile 단위 분할  
 - SRAM : SRAM, Shared Memory 적용  
 - Online Softmax : Block별 Softmax 계산  
 - Recomputation : 필요 시 재연산

&lt;기술요소&gt;  
 - IO-Aware Attention : HBM과 SRAM 데이터 이동 비용 고려  
 - Kernel Fusion : 하나의 GPU 내 Kernel 처리, 이동 및 호출 감소  
 - Memory-efficient Attention : HBM에 Materialization 하지 않음  
 - Exact Attention : 기존 Dense 결과와 동일한 정확한 결과

&lt;버전&gt;  
 - Flash Attention-1 : Tiling, Online Softmax  
 - Flash Attention-2 : Work Partitioning, Parallelism  
 - Flash Attention-3 :  Warp Specialization, TMa, FP8  
 - Flash Attention-4 : CuTe-DSL, Co-Design (Kernel+Pipeline)

## [생성형AI] 사전학습 모델 (Pre-trained Model)



**[정의]**

대규모 또는 특정 도메인 데이터로 미리 학습되어 특징 / 패턴 / 지식을 획득한 AI 모델

**[핵심/키워드]**

- 사전학습, 재사용 관점, Transfer Learning / 재사용 목적 활용  
 - 학습데이터 규모 : 특정 도메인 또는 태스크 중심 데이터셋  
 - 활용 가능성 : 특정 태스크(분류,감성 분석,음성 인식 등)에 최적화  
 - 프롬프트 기반 사용 : 불가능 또는 제한적  
 - 파인튜닝 필요성 : 새로운 데이터에 맞춰 추가 학습 필요 가능  
 - 적용 범위 : 특정 분야(의료,법률,금융 등)에 특화 가능  
 - 대표 모델 : BERT, RoBERTa, ResNet, DeepSpeech, Wave2Vec 2.0

## [생성형AI] 파운데이션 모델 (Foundation Model)



**[정의]**

대규모 데이터와 강력한 연산 능력을 활용하여 사전학습(Pretraining)된 범용 인공지능 모델

다양한 AI 태스크에 쉽게 적용(Fine-tuning)할 수 있는 기반이 되는 모델

**[핵심/키워드]**

&lt;특징&gt;  
 - 사전 학습 (Pretraining) 기반, 자기지도학습 (Self-Supervised Learning) 기반  
 - 창발성 (Emergence), 균일화 (Homogenization)  
 - 다양한 태스크에 적용 가능, Fine-tuning 및 Prompting 지원  
 - 멀티모달 확장 가능, Zero-shot / Few-shot Learning 지원

&lt;파운데이션 모델 최적화 기법 및 알고리즘&gt;  
 - 지식증류 (Knowledge Distillation) : Soft Label Distillation (교사모델 확률분포 학습)  
 - 가중치 가지치기 (Weight Pruning) : TinyBERT, DistilBERT, Magnitude Pruning, Structured Pruning, L1/L2 Pruning  
 - 양자화 및 이진화(Quantization & Binarization) : Post-Training Quantization (PTQ), Quantization-Aware Training (QAT), XNOR-Net  
 - 파라미터 효율적 미세 조정(PEFT, Parameter Efficient Fine-Tuning) : LoRA (Low-Rank Adaptation), LoRA Adapters, Prompt Tuning  
 - 희소성 유도 (Sparsity Induction) : Lottery Ticket Hypothesis, Dynamic Sparsity, Sparse Transformer  
 - 지연된 가중치 업데이트(Delayed Updates) : Gradient Accumulation, Periodic Weight Updates

&lt;대표모델&gt;  
 - GPT, Gemini, Claude, Llama

## [생성형AI] 대규모 멀티모달 모델 (Large Multimodal Model, LMM)



**[정의]**

텍스트, 이미지, 오디오 등 다양한 형태의 데이터를 처리하고 생성하기 위해 훈련된 인공지능 모델

**[핵심/키워드]**

- 다양한 모달리티 연관 학습 및 생성  
 - 멀티모달 응용

&lt;주요기술요소&gt;  
 - 통합 데이터 처리, 멀티모달 임베딩, 모달별 서브모델

&lt;대표모델&gt;  
 - SORA, Gemini Pro, Emu, GPT-4o

## [생성형AI]  파인튜닝 (Fine-Tuning)



**[정의]**

전이학습의 일종으로, 기존 모델의 일부 또는 전체 가중치를 조정하여 새로운 데이터셋에 맞게 추가 학습하는 방법

**[핵심/키워드]**

&lt;특징&gt;  
 - 사전 학습 모델 활용, 도메인 특화 최적화, 빠른 학습 속도, 일반화 성능 보존, 고성능 GPU

&lt;파인튜닝 단계 및 적용기법&gt;  
 1) 모델별 아키텍처 이해 : 모델 아키텍처 시각화 (TensorBoard, Netron), Zero-Shot & Few-Shot 평가  
 2) 파인튜닝 데이터 준비 :  데이터 증강, 노이즈 제거, 토큰화(Tokenization)  
 3) 사전 학습 모델 선택 및 로드 :  Hugging Face Transformers, Pretrained Model Loading (PyTorch, TensorFlow)  
 4) 미세조정 수행(Fine-Tuning) : Full Fine-Tuning, Partial Fine-Tuning, PEFT (LoRA, Adapter)  
 5) 하이퍼파라미터 튜닝 : Grid Search, Bayesian Optimization, Learning Rate Scheduling (Warmup, Cosine Decay)  
 6) 모니터링 및 적용 : Early Stopping, Weight Regularization (Dropout, L2 Norm)  
 7) 모델 성능 평가 및 테스트 : Accuracy, Precision, Recall, F1 Score, BLEU, ROUGE (NLP 평가), Confusion Matrix

&lt;파인튜닝 기법&gt;  
 - 전체 조정 : Full Fine-Tuning  
 - 부분 조정 : Partial Fine-Tuning  
 - PEFT(Parameter-Efficient Fine-Tuning) : LORA(Low-Rank Adaptation), QLORA(Quantized LoRA), Adapter Tuning, Prefix Tuning, Prompt Tuning, BitFit (Bias Tuning)

## [생성형AI] LoRA  (Low-Rank Adaptation)



**[정의]**

모델의 원래 파라미터를 그대로 유지하면서,일부 파라미터의 변형만으로 효과적인 학습이 가능하도록 낮은 랭크의 행렬로 근사하여 FineTuning을 수행하는 기법

**[핵심/키워드]**

&lt;특징&gt;  
 - 기본 아이디어 : Low-Rank 근사화  
 - 구조 : W = B x A  
 - 학습방식 : 선형 독립 변화 방향만 학습, 2개의 저랭크 행렬곱  
 - Base Model 상태 : Base Weight Freeze  
 - 학습 대상 : 추가된 Low Rank Adapter, 일부 파라미터만 학습  
 - 저장 방식 : 경량화 된 체크포인트  
 - 효율성 : 낮은 메모리 사용량, 낮은 연산 비용  
 - 적용 방법 : 기존 Layer에 LoRA 모듈 추가  
 - 태스크 전환 : 모듈 교체 방식  
 - 대표 활용 예시 : 대규모 언어모델, 멀티모달 모델

## [생성형AI] QLoRA (Quantized Low-Rank Adaptation)



**[정의]**

Base Model을 4-bit로 양자화하고, 기존 Weight는 Freeze한 상태에서 LORA Adapter만 학습하는 PEFT 기법

**[핵심/키워드]**

&lt;특징&gt;  
 - Base Model : Base Model 4bit 양자화 후 Freeze  
 - 학습 : 추가된 LoRA Adapter  
 - 원리 : 4bit 양자화+LoRA  
 - 효율성 : 매우 낮은 메모리 사용, 매우 적은 학습 비용  
 - 저장 : Adapter만 저장

&lt;주요단계&gt;  
 1) 4bit NF 양자화 > 2) 이중 양자화 (양자화 상수 양자화) > 3) Paged Optimizers (페이지 단위 전송)

## [생성형AI] 도메인 특화 언어모델 (Domain-Specific Language Model, DSLM)



**[정의]**

특정 산업의 데이터로 학습하여 고정밀, 고신뢰 예측이 가능한 특화 LLM (가트너 2026)

금융, 의료 등 특정 도메인의 문제를 정확히 이해하고 해결하기 위해 해당 도메인의 지식을 학습하여 전문적 언어처리능력을 제공하는 모델

**[핵심/키워드]**

&lt;특징&gt;  
 - DSLM 학습 데이터셋(산업, 조직, 업무 특화 데이터) 학습

&lt;기술요소&gt;  
 - 데이터 : 도메인 전용 데이터셋, 데이터 정제 / 라벨링  
 - 모델 학습 : 파인 튜닝(Fine-tuning), From Scratch 학습  
 - 지식 확장 : RAG, 벡터 데이터베이스  
 - 지식 구조화 : 지식 그래프(KG)  
 - 입력 최적화 : 프롬프트 엔지니어링, 인컨텍스트 러닝(ICL)  
 - 추론 제어 : 룰 기반 제어  
 - 안전성 : 도메인 안전 가드레일  
 - 평가 : 도메인 특화 평가 지표  
 - 운영 : 지속적 학습 (MLOps,  LLMOps)  
 - 보안 / 거버넌스 : 접근통제, 감사가능성

&lt;사례&gt;  
 - DarkBert (다크웹), CyBERTuned (사이버보안)

## [생성형AI] RLHF (Reinforcement Learning from Human Feedback)



**[정의]**

인간 평가자가 모델 출력에 대해 선호 / 품질 피드백을 제공하고 모델의 응답을 의도에 맞게 정렬하는 학습 방식

**[핵심/키워드]**

&lt;특징&gt;  
 - 인간 기준 정렬(Human Alignment)  
 - 안전성, 윤리성 확보에 유리

&lt;수행단계별 설명&gt;  
 1. 관찰(Observation) : Prompt / Context 입력  
 2. 행동(Action) : LLM이 Response 생성  
 3. 보상 예측(Reward Predictor) : Reward Model / Reward Score  
 4. 인간 피드백(Human Feedback) : Preference / Ranking Data Reward Model 학습  
 5. 예측된 보상(Predicted Reward) : 높은 Reward를 받도록 Policy 개선  
 6. Policy 최적화 : PPO / KL Penalty 기반 Parameter Update

&lt;핵심 메커니즘&gt;  
 - Human Preference, Reward Modeling, PPO / KLPenalty

## [생성형AI] RLAIF (Reinforcemen tLearning from AI Feedback)



**[정의]**

AI 모델이 다른 모델의 출력에 대해 자동 평가 / 피드백을 생성하고 이를 강화학습에 활용하는 기술

**[핵심/키워드]**

&lt;특징&gt;  
 - 자동화 기반 피드백 생성, 대규모 데이터 생성 가능, 빠른 학습 반복

&lt;원칙설정&gt;  
 1) 행동 원칙 : 안전성, 정확성, 유해성 금지  
 2) 가이드라인 : 답변 스타일, 금지 주제, 응납 톤

&lt;평가기준&gt;  
 - 정확성(correctness), 유용성(helpfulness), 무해성(harmlessness), 일관성(consistency)

&lt;동작구조&gt;  
 1) 원칙 설정 > AI 평가 > 보상 모델 > RL로 모델 개선

&lt;핵심 메커니즘&gt;  
 - AI 피드백, AI Judge, ConstitutionalAI, Reward Modeling, PPO / DPO 계열

## [생성형AI] 소형 대규모 언어모델 (Small Large Language Model, SLLM)



**[정의]**

LLM의 강력한 기능을 유지하면서도 효율적으로 경량화된 모델

**[핵심/키워드]**

&lt;특징&gt;  
 - LLM / SLM의 중간 형태, 성능과 효율성 고려  
 - Latency, 비용 최적화  
 - 학습데이터 : 범용 데이터 + 고품질 데이터 / 합성 데이터  
 - 경량화 기술 : Distillation / Quantization / Pruning / PEFT 적극 활용  
 - 배포 환경 : Cloud / On-premise / Private AI  
 - 주요 활용 : 기업업무 / 도메인 AI / Private AI

## [생성형AI] 전문가 혼합모델 (Mixture of Experts, MoE)



**[정의]**

여러 개의 전문가 네트워크(Expert Network)를 두고, Gating Network가 특정 입력에 적합한 전문가를 선택하여 최적의 결과를 도출하는 모델

여러 전문가 모델(Experts) 중 일부만 선택적으로 활성화하여 입력을 처리하는 딥러닝 아키텍처

**[핵심/키워드]**

&lt;특징&gt;  
 - Gating Network 활용, 다중 태스크 학습 지원, 희소 계산(Sparse Computation) 가능  
 - 토큰라우팅(Token Routing)

&lt;구성요소 및 역할&gt;  
 - 입력 (Query) 처리 : 입력 전달  
 - 게이트 네트워크(Gate Network) : 전문가 선택, Softmax 기밙 Top-K  
- 전문가 네트워크 (Experts) : 입력 처리, Spare Attention  
- 로딩 밸런싱(Load Balancing) : 부하 분산, 연산 쏠림 방지, 추가 손실함수  
- 추론 레이어(Inference Layer / MoE Layer) : 출력 통합  
- 출력 (Output) : 결과 제공

&lt;활용 모델&gt;  
 - Google Switch Transformer, Google GShard, DeepSeek

## [생성형AI] 프롬프트 엔지니어링 (Prompt Engineering)



**[정의]**

생성형 인공지능 솔루션을 안내하여 원하는 결과를 생성하는 프로세스

사용자가 거대 언어 모델(LLM)에 원하는 결과를 얻기 위해 효율적인 입력 문장을 설계하는 기술

**[핵심/키워드]**

&lt;특징&gt;  
 - 입력최적화, 문맥 반영, 단계별 사고 유도, 롤플레잉 가능, 명확한 출력

&lt;구성요소&gt;  
 - 지시/명령어 (Instruction), 문맥 (Context), 예제 (Examples), 입력/출력 형식 (Output Format), 페르소나 (Persona)

&lt;기술 요소&gt;  
 - 지시 설계 : 지시 프롬프팅(Instruction Prompting), 역할 프롬프팅(Role Prompting), 프롬프트 템플릿(Prompt Template)  
 - 예시 활용 : 제로샷 프롬프팅(Zero-shot Prompting), 원샷 프롬프팅(One-shot Prompting), 퓨샷 프롬프팅(Few-shot Prompting)  
 - 추론 강화 : 사고사슬 (Chain-of-Thought, CoT), 자기일관성(Self-Consistency), 최소에서 최대 프롬프팅(Least-to-Most Prompting)  
 - 복합 작업 : 프롬프트 체이닝(Prompt Chaining), 추론 / 행동 (ReAct, Reasoning + Acting), 컨텍스트 프롬프팅(Context Prompting)  
 - 출력 제어 : 그라운딩 (Grounding), 구조화 프롬프팅(Structured Prompting), 제약 프롬프팅(Constraint Prompting)

<추론 강화 프롬프트 기법(엔지니어링 기법)>
 - 사고의 사슬(CoT) 프롬프트, 사고의 나무(TOT) 프롬프트, 산파술 프롬프트, 복잡성 기반 프롬프트, 생성된 지식 프롬프트, 최소-최대 프롬프트, 자기 개선 프롬프트, 방향 자극 프롬프트

## [생성형AI] 컨텍스트 엔지니어링 (Context Engineering)



**[정의]**

LLM에 제공되는 다양한 정보 소스(정보 페이로드)를 체계적으로 설계하고 조합하여, AI의 추론 및 응답 품질을 극대화하는 통합 프레임워크

**[핵심/키워드]**

&lt;특징&gt;  
 - 답변을 생성하는 데 필요한 맥락을 어떻게 구성, 정보 환경 제공

&lt;구성요소&gt;  
 - 기반 구성요소 : 컨텍스트 검색 / 생성, 컨텍스트 처리, 컨텍스트 관리  
 - 시스템 구현 : RAG 기반 시스템, 메모리 기반 시스템, 도구 통합 추론, 멀티 에이전트 시스템

&lt;수행 절차&gt;  
 1) 사용자 입력 전처리 : 목적/의도 파악, 입력 정제  
 2) 컨텍스트 수집 : 정적 정보, 동적 정보, 대화 이력  
 3) 컨텍스트 처리 및 통합 : 정보 요약, 필터링, 중요도 정렬, 체인 구조 설계  
 4) 프롬프트 생성, LLM 호출 : 자연어 기반 질문 최적화, LLM 호출  
 5) 응답 후처리 결과 전달 : 응답 구조화, 요약(토큰화), 포맷 정리, 사용자 UI호출, 알림

## [생성형AI] 검색증강 생성기술 (Retrieval Augmented Generator, RAG)



**[정의]**

대규모 언어 모델(LLM)에서 질문에 대한 답변이나 텍스트를 생성하기 전에 광범위한 문서 집합에서 관련 정보를 검색하고, 이를 이용하여 응답을 생성하는 방법

**[핵심/키워드]**

&lt;동작&gt;  
 1) 사용자 요청 질의 > 2) 검색 > 3) 데이터 결과 / 추출 > 4) 결과와 질의 결합 전달 > 5) LLM 응답 > 6) 사용자 응답

&lt;구성요소&gt;  
 - 데이터 수집 : 데이터 소스(Data Source)  
 - 전처리 : 문서 로더 / 정제 (Document Loader / Preprocessing), 청킹(Chunking)  
 - 벡터화 : 임베딩 모델(Embedding Model)  
 - 저장 / 인덱싱 : 벡터 DB(Vector Database), ANN 인덱스(Approximate Nearest Neighbor Index)  
 - 질의 처리 : 질의 처리(Query Processing)  
 - 검색 : 검색기(Retriever), 유사도 계산(Similarity Search)  
 - 검색 고도화 : 하이브리드 검색(Hybrid Search), 재순위화기(Reranker)  
 - 컨텍스트 구성 : 컨텍스트 빌더(Context Builder), 생성 모델 (Generator / LLM)  
 - 검증/출력 : 검증 / 출처 (Validation / Citation)

&lt;유형&gt;  
 - 구현 관점 : Naive RAG, Advanced RAG, Modular RAG  
 - 사용 / 동작 관점 : Vanilla RAG, Conversational RAG, Multi-hop RAG, Tool-RAG, Agentic RAG, GraphRAG

<벤치마크 / 평가기법>
 - RGB, RECALL, CRUD-RAG, RAGAS, ARES, TruLens

## [생성형AI] 검색 통합 생성 (Retrieval-Integrated Generation, RIG)



**[정의]**

LLM의 성능을 향상시키기 위해, 모델이 응답 생성 과정 중에 실시간으로 데이터베이스와 상호작용 하는 방식

**[핵심/키워드]**

* 필요한 정보를 검색하여 생성 과정 중 필요시, 업데이트  
&lt;동작&gt;  
 1) 요청 질의 > 2) 프롬프트 생성 > 3) 부분 응답 생성 > 4) 정보 검색 및 추출 > 5) 응답 생성 > 6) 최종 응답 생성 > 7) 사용자 응답 전달

&lt;특징&gt;  
 - 처리방식 : Generation, Retrieval 반복 / 교차  
 - 질문 Query : 동적 Query

## [생성형AI] 벡터 데이터베이스 (Vector Database)



**[정의]**

고차원 벡터 형태로 표현된 데이터(임베딩)를 저장하고, 유사한 벡터를 빠르게 검색할 수 있도록 최적화된 데이터베이스 시스템

방대한 양의 고차원 데이터를 벡터 형태로 최적화하여 보관하고 쿼리하기위해 특화된 데이터베이스

**[핵심/키워드]**

&lt;특징&gt;  
 - 벡터화 된 데이터의 저장 및 검색, 근사 최근접 이웃 검색(ANN), LLM, RAG 활용

&lt;구성요소&gt;  
 - 임베딩 벡터 (Embedding Vector), 벡터 인덱스 (Vector Index), 저장 엔진(Storage Engine), 유사도 함수(Similarity Function), 메타데이터 저장소

&lt;절차&gt;  
 1) 데이터 임베딩 > 2) 벡터 저장  > 3) 인덱싱 (ANN) > 4) 쿼리 임베딩 > 5) 유사도 계산 > 6)  결과 반환

&lt;유형&gt;  
 - Pinecone, Weaviate, Milvus, Faiss

<구축 시, 고려사항>
 - 성능 및 내결함성, 모니터링 기능, 액세스 제어, 확장성 및 조정성, 다중 사용자 및 데이터 격리, 백업 기능, API 및 SDK 지원

## [생성형AI] 근사 최근접 이웃 검색 (Approximate Nearest Neighbor, ANN)



**[정의]**

고차원 공간에서 입력 벡터와 유사한 이웃을 빠르게 찾는 근사 검색 기법

벡터 DB에서 입력 벡터와 가장 유사한 벡터를 빠르게 찾아주는 핵심 기술

**[핵심/키워드]**

&lt;필요성&gt;  
- 기존 KNN은 정확하지만 느리고 연산 비용 큰 단점 해결, 속도와 효율성 향상

&lt;절차&gt;  
 1) 벡터 임베딩 > 2) 벡터 인덱싱 (Indexing) > 3) 쿼리 입력 및 탐색 (일부 후보만 탐색) > 4) 근사 최근접 이웃 반환 (유사도, Top-K) > 5) 후처리 (선택적)

&lt;주요알고리즘 및 적합 환경&gt;  
 - HNSW(Hierarchical Navigable Small World) : 계층적, 고속, 고정확, 실시간 LLM, RAG  
 - IVF(Inverted File Index) : K-means 클러스터링, 대용량 문서 검색, 분산 벡터 DB  
 - PQ(Product Quantization) : 분할, 압축, 저사양·모바일 환경, IVF와 병행 사용  
 - ScaNN(Scalable Nearest Neighbors) : IVF+PQ+Rerank,  Google 대규모 서비스  
 - ANNOY(Approximate Nearest Neighbors Oh Yeah) : 랜덤트리, 읽기 전용 환경

## [생성형AI] HNSW (Hierarchical Navigable Small World)



**[정의]**

벡터를 다층 그래프 구조로 연결하고, 상위 계층에서 탐색 범위를 빠르게 좁힌 후 하위 계층에서 정밀 탐색하여 근사 최근접 이웃(ANN)을 찾는 그래프 기반 검색 알고리즘

**[핵심/키워드]**

&lt;특징&gt;  
 - 탐색속도 : O(log(N))  
 - Multi-layer Graph 구조 : 상위 레이어는 Sparse, 하위 레이어는 Dense

&lt;하이퍼 파라미터&gt;  
 - M : Node당 최대 이웃 연결 수  
 - efConstruction : 인덱스 구축 시 후보 탐색 범위  
 - efSearch : 검색 시 후보 탐색 범위

&lt;절차&gt;  
 - 인덱스 구축  
  1) 벡터 입력 > 2) 계층 레벨 결정 > 3) 상위 계층 탐색 > 4) 근접 후보 탐색 > 5) Graph Edge 구성 > 6) HSNW Index 구축  
 - 검색  
   7) Query Vector 입력 > 8) Top-down 탐색 > 9) Layer 0 후보 확장 > 10) Top-K 반환

## [생성형AI] IVF (Inverted File Index)



**[정의]**

전체 벡터 공간을 K-means등으로 클러스터링한 뒤, 쿼리 벡터와 인접한 일부 셀만 한정하여 스캔하는 알고리즘

**[핵심/키워드]**

&lt;특징&gt;  
 - 탐색속도 : O(K+ (nprobe / K) • N)  
 - 역색인 구조(Inverted List) : 데이터 클러스터링 후, 벡터 데이터 역색인 구조로 연결

&lt;구성요소&gt;  
 - Centroid, Inverted List, Quantizer, Cluster, nprobe

&lt;절차&gt;  
 - 학습 및 분할  
  1) 데이터 클러스터링 > 2) 중심점 확정  
 - 색인 및 저장  
  3) 데이터 매칭 > 4) 역 색인 생성  
 - 검색 및 합산  
  5) 후보군 관리 > 6) 부분 거리 계산

## [생성형AI] PQ (Product Quantization)



**[정의]**

고차원 벡터를 서브 벡터로 분할하고, 코드북을 생성하여 압축된 인덱스 간의 거리를 룩업 테이블로 계산하는 알고리즘

**[핵심/키워드]**

&lt;특징&gt;  
 - 탐색속도 : O(N• M)  
 - Quantization, Product 구조 : 고차원 벡터를 양자화 하여 압축

&lt;구성요소&gt;  
 - Sub-space, Centroid, Codebook, Code, 룩업 테이블 (LUT)

&lt;절차&gt;  
 - 학습 및 생성  
  1) 차원 분할 (Splitting) : Sub-vector (m)  
  2) 코드북 학습 (Training) : K-means, Centroids  
 - 압축 및 저장  
  3) 양자화 (Quantizing) : Assignment  
  4) 인덱스 변환 (Encoding) : Code (Index)  
 - 거리 계산  
  5) 거리 표 생성 (Table) : Look-up Table (LUT)  
  6) 누적 합산 (ADC) : Asymmetric Distance

## [생성형AI] Re-ranking 알고리즘



**[정의]**

1차 검색을 통해 얻은 후보 문서/벡터 집합을 대상으로 Query와의 관련도를 다시 정밀 평가하여 순위를 재조정하는 검색 후처리 기법

**[핵심/키워드]**

&lt;동작&gt;  
 1) 1차 검색(ANN / BM25 / Hybrid Search) > 2) Top-K 후보 > 3) Re-ranking > 4) 최종 Top-N

&lt;알고리즘&gt;  
 - Cross-Encoder 기반 : Cross-Encoder, MonoBERT  
 - Embedding 기반 : Bi-Encoder  
 - Late Interaction 모델 : ColBERT  
 - Learning to Rank (Pointwise) : MART, GBRank  
 - Learning to Rank (Pairwise) : RankNet, LambdaRank  
 - Learning to Rank (Listwise) : ListNet, ListMLE, LambdaMART

&lt;활용&gt;  
 - Vector DB, RAG, 검색 엔진, 추천 시스템

## [생성형AI] 지식그래프 (Knowledge Graph)



**[정의]**

현실 세계의 개체(Entity)와 관계(Relationship)를 그래프 형태로 표현한 의미 기반 데이터 구조

**[핵심/키워드]**

&lt;특징&gt;  
 - 의미 기반 맥락 표현, 관계 연결, 확장 용이, 추론 가능, LLM 성능 향상

&lt;그래프 이론 기반 표현방식&gt;  
 - 노드(Node): 엔티티(Entity)  
 - 엣지(Edge): 관계(Relationship)  
 - 속성(Attribute) : 엔티티나 관계의 특성

&lt;데이터 중심 표현방식&gt;  
 - 엔티티(Entity) : 사람,장소,사물,개념  
 - 속성(Attribute) : 엔티티 특성(이름,나이,위치 등)  
 - 관계(Relationship) : 엔티티 간 의미적 연결(예:A-고용→B)

&lt;지식 그래프의 지식 표현 체계&gt;  
 - 온톨로지(Ontology): 개념·관계 정의 체계  
 - RDF(Resource Description Framework): 웹 표준 데이터 표현 언어  
 - SPARQL: 그래프 질의(Query)언어  
 - 트리플 저장소(Triple Store): RDF기반 데이터 저장 시스템  
 - 그래프 데이터베이스: Neo4j,TigerGraph 등  
 - 추론 엔진(Inference Engine): 논리 규칙 기반 자동 추론  
 - 엔티티 정규화(Entity Linking): 동일 개체 식별·연결

## [생성형AI] RAG as a Service (RAGaaS)



**[정의]**

문서 수집, 청킹, 임베딩, 벡터 인덱싱, 검색, 재순위화, LLM 생성, 모니터링 등 RAG 전 과정을 API / SDK / Cloud 기반으로 통합 제공하는 관리형 서비스 (Managed Service)

**[핵심/키워드]**

&lt;주요기능&gt;  
 - 데이터 처리 : Chunking, Embedding, Vector Database  
 - 검색시스템 : HNSW, IVF, 유사도검색  
 - 생성형 AI 모델 : LLM, 프롬프트 엔지니어링  
 - 운영관리 : API 통합 인터페이스, ScaleOut, ScaleUp, 모니터링

 - AWS = Amazon Bedrock Managed  
 - Azure = Azure AI Search  
 - GCP = Vertex AI RAG Engine

## [생성형AI] 멀티모달AI (Multimodal AI)



**[정의]**

다양한 모달리티를 동시에 인식하는 AI 모델

텍스트와 시각적 정보, 소리, 영상, 촉감 등 인간의 다양한 감각기관을 통합하여 학습 후 새로운 창작물을 생성하는 차세대 인공지능 모델

**[핵심/키워드]**

&lt;기술요소&gt;  
 1) 입력모듈 (Input Module) : 전처리 및 인코딩  
   - 다양한 모달 데이터 처리, 데이터 인코딩 (Modality Encoding), 자연어 처리 (NLP), 컴퓨터 비전 (CV)  
 2) 융합모듈 (Fusion Module) : 데이터 통합, 의미 학습, 연관성 분석  
  - 멀티모달 Transformer, Cross-Modality Learning (교차 모달 학습), Contrastive Learning (대조 학습), 분산학습 (Distributed Learning), 지식증류 (Knowledge Distillation)  
 3) 출력모듈 : 결과 생성  
  - 멀티모달 생성 (Multimodal Generation), Vision-Language Model (VLM) 기반 생성, Diffusion Models (이미지 / 영상 생성), 다양한 출력 형식 지원

&lt;퓨전방식&gt;  
 - Early / Intermediate / Late Fusion

&lt;사례&gt;  
 - CLIP, Flamingo, Kosmos-1

## [생성형AI] 옴니모달 AI (Omni-Modal AI)



**[정의]**

텍스트, 이미지, 음성, 영상, 행동 등 모든 모달 데이터를 하나의 통합 모델에서 학습·이해·생성하는 AI 구조

**[핵심/키워드]**

* 공유 잠재 공간(Shared Latent Space) 기반 일체형, Any to Any  
&lt;특징&gt;  
 - 단일 Transformer, 공통 토큰화(Tokenization), Sequence-to-Sequence 통합, Interleaved 데이터 흐름(모달 혼합 시퀀스 처리), 이해·추론·생성의 일체형 구조

&lt;핵심 기술&gt;  
 - 입력토큰화 : 공통 토큰화 (동일 토큰 변환)  
 - 공유잠재공간 : 모달 정렬(Alignment) (동일 임베딩 공간 정렬)  
 - 크로스 모달 학습: Matching(의미적 일치), Translating(모달 변환), Referencing(참조)  
 - 생성 : Multimodal Generation, Diffusion Models, VLM 기반 생성

&lt;대표모델&gt;  
 - Unified-IO, Meta-Transformer, 네이버 하이퍼클로바 X 옴니

&lt;멀티모달 vs 옴니모달&gt;  
 - 멀티모달 : 모달별 분리 인코더 → 융합 모듈 → 출력  
 - 옴니모달 : 공통 토큰화 → 공유 잠재공간 → 단일 Transformer 통합학습 → 멀티모달 생성

## [생성형AI] Affective AI (정서/감성 AI)



**[정의]**

인간의 감정, 기분, 정서 상태를 데이터로 인식·표현·반응하는 기술

**[핵심/키워드]**

&lt;진화단계&gt;  
 - 1세대 : 표정 · 음성 기반 감정 표현  
 - 2세대 : 멀티모달 감정인식, 실시간 상호작용  
 - 3세대 : 감정 예측, 개인화, 장기 정서 모델링

&lt;기술요소&gt;  
 - 멀티모달 감정인식 기술 : 얼굴 움직임 부호화, 음성 특징 추출, 텍스트감성 분석  
 - 맥락 기반 감정이해 기술 : 대화 상태 추적, 문맥 임베딩,사용자 프로파일링  
 - 감정의 불확실성 해소 기술 : 베이지안 추론, 신뢰도 점수, 앙상블 학습  
 - 감정 기반 의사결정 및 행동 생성 기술 : 강화 학습, 정책 네트워크, 감정상태 모델  
 - 공감적 응답생성 기술 : 공감 대화 모델, LLM, RLHF  
 - 윤리, 프라이버시 고려 기술 : 차분 프라이버시, 연합학습, 온디바이스 AI

&lt;한계 및 해결방안&gt;  
 - 감정 모델링의 개념적 한계 : 차원 감정 모델(Valence-Arousal), 범주형 감정 모델  
 - 멀티모달 감정인식의 기술적 난제 : 멀티모달 융합, 교차 주의집중, 신뢰도 기반 가중치  
 - 맥락 이해 및 일반화 한계 : 대화 상태 추적, 사용자 프로파일링, 장기 메모리  
 - 윤리적, 사회적 쟁점 : 프라이버시 보호, 설명가능성, 가드레일, 사용 목적 제한

## [생성형AI] 에이전틱 AI (Agentic AI)



**[정의]**

사용자의 명확한 지시나 명령 없이도 스스로 작업을 수행하는 자율적인 소프트웨어(가트너2025)

**[핵심/키워드]**

&lt;특징&gt;  
 - 자율성, 목표 지향성, 계획 수립 능력, 지속적 상호작용 및 피드백, 학습 및 적응력

&lt;구성요소&gt;  
 - User (사용자), Al Agent, LLM, Database, Vector DB, Action (행동 수행 모듈), Model Customization(모델 맞춤화), Data Flywheel (데이터 플라이휠)

&lt;기술요소&gt;  
 - 인식 : 컨텍스트 인식(Context Awareness), 멀티모달 처리(Multimodal Processing), 데이터 수집(Data Acquisition)  
 - 추론 :  LLM 추론(LLM Reasoning)  
 - 계획 : 작업 분해(Task Decomposition), 계획 수립(Planning), 목표 관리(Goal Management)  
 - 지식 : RAG, 지식 그래프(Knowledge Graph)  
 - 기억 : 단기 기억(Short-term Memory), 장기 기억(Long-term Memory)  
 - 행동 : 도구 호출(Tool Calling), API 연동(API Integration), 코드실행 (Code Execution), 외부 시스템 제어(System Control)  
 - 평가 : 결과 평가(Evaluation)  
 - 적응 : 재계획(Re-planning)  
 - 학습 : 피드백 학습(Feedback Learning), 강화학습(Reinforcement Learning), 파인튜닝(Fine-tuning)  
 - 오케스트레이션 : 라우팅(Routing), 상태 관리(State Management), 워크플로 제어(Workflow Control), 멀티에이전트 협업(Multi-Agent Coordination)  
 - 거버넌스 : 가드레일(Guardrail), 보안(Security), 모니터링(Monitoring), Human-in-the-Loop

## [생성형AI] AI 가상비서 (AI Virtual Assistant, AI Digital Assistant)



**[정의]**

AI 플랫폼을 활용하여 인간의 생산성과 편의를 높이는 노무형 AI 서비스

**[핵심/키워드]**

&lt;특징&gt;  
 - 음성 및 텍스트 기반 상호작용, 지능형 자동화, 맞춤형 서비스, 지속적 학습 및 개선

&lt;주요기능&gt;  
 - 일정 관리, 알람 설정, 미디어 제어, 금융 및 쇼핑, 스마트 홈 연동, 언어 번역 및 학습

&lt;기술요소&gt;  
 - 자연어 이해/생성(NLU / NLG), 대규모 언어모델(LLM)  
 - 음성 인식(STT), 음성 합성(TTS)  
 - 대화 관리(Dialog Management), 맥락 인식(Context Awareness)  
 - 메모리(Memory), 정보 검색 / RAG, 도구 호출(Tool Calling)  
 - 오케스트레이션(Orchestration), 컴퓨터 비전(CV)  
 - 감성 인식(Emotion / Sentiment Recognition)  
 - loT 연동, 개인화(Personalization), 보안 / 인증(Security/Authentication)

&lt;발전단계&gt;  
 - 1단계 : 명령 중심 : 규칙 기반, 기본 NLP, 음성 명령 수행  
 - 2단계 : 상황화 비서 : 맥락 이해 및 대화형 상호작용, 머신러닝 기반 NLP  
 - 3단계 : 능동형 비서 - 개인화된 서비스 제공 및 복합 작업 처리, 딥러닝, loT 연동  
 - 4단계 : 숙련형 비서 : 의사결정 및 창의적 문제 해결, 강화 학습, 대규모 언어 모델  
 - 5단계 : 감성 비서 : 감정 인식 AI 및 정서적 지원, 감성 인식 Al, 감성 컴퓨팅

## [생성형AI] Agentic RAG (Agentic Retrieval-Augmented Generation)



**[정의]**

RAG 파이프라인 에에이전트(AI agents)를 통합하여, 스스로 검색 전략을 계획, 조정하고 도구를 호출하여 반복적으로 결과를 개선해가는 자율형 AI 시스템

**[핵심/키워드]**

* 단순 1회 검색을 넘어 질의 난이도와 상황에 따라 검색 경로 / 도구를 동적으로 선택  
&lt;처리 흐름&gt;  
 1) 입력(Query) > 2) Router Agent(요청 분석) > 3) 각 Retrieval Agent가 동작 수행 > 4) LLM Core 전달 > 5) 응답(Response) 생성

&lt;레이어별 구성요소&gt;  
 1) Agent Layer : 질의분석, 검색 오케스트레이션  
  - Retrieval Router Agent (LLM Planning), Retrieval Agent X/Y/Z (Dense / Sparse / Hybrid Retrieval),  Action / Tool Agent (MCP / AZA / JSON-RPC 2.0)  
 2) RAG Core Layer : 검색, 생성 처리  
  - Retriever (Dense/ Sparse/ Hybrid 검색), Re-ranker (MonoT5, ColBERT), Generator (LLM)(CoT, ToT), Vector DB (FAISS, Milvus, Pinecone)  
 3) Evaluator / Feedback Layer : 품질 검증, 피드백 루프  
  - Self-Evaluator (Self-Reflection), External Evaluator (RAGAS, TruLens), Memory Module (Memory Buffer)

 - 제어권: RAG-사용자 입력 중심 / Agentic RAG-에이전트 자율 추론  
 - 구조: RAG-단일 검색→생성 루프 / Agentic RAG-다단계 추론 및 행동 루프  
 - 응용: RAG-QA 중심 / Agentic RAG-자율 태스크 수행 및 복합 의사결정

&lt;주요 Framework&gt;  
 - LangChain + LangGraph, LlamaIndex(GPT Index), CrewAI, AutoGen(Microsoft)

## [생성형AI] 다중 에이전트 시스템 (Multi-Agent System, MAS)



**[정의]**

여러 독립적·자율적 에이전트가 상호 작용하여 개발 및 시스템 운영 등 전체 목표를 달성하는 시스템 아키텍처 패러다임 (가트너 2026)

여러 개의 자율적(Autonomous) 에이전트(Agent)가 상호 협력 / 경쟁 / 조정을 통해 공동의 목표를 달성하거나 복잡한 문제를 해결하는 시스템

**[핵심/키워드]**

&lt;특징&gt;  
 - 자율성(Autonomy), 협력성(Cooperation), 분산성(Distribution), 적응성(Adaptability), 지능성(Intelligence)

&lt;기술요소&gt;  
 - 통신·협력 : FIPA ACL, KQML  
 - 의사결정 / 추론 : 메시징, 오케스트레이션, 강화학습 (MARL), 지식기반 추론, LLM  
 - 환경 / 시뮬레이션 : NetLogo, Mesa, GAMA, JADE  
 - 플랫폼 / 미들웨어 / 프레임워크 : SPADE, CrewAl, AutoGen, Lang Graph, Swarm

&lt;구성요소&gt;  
 - 에이전트(Agent), 환경(Environment), Coordinator / Manager, 통신(Communication)

&lt;활용분야&gt;  
 - 산업/제조: 로봇 협업 제어, 분산 생산관리  
 - AI 서비스: 에이전트 간 역할 분담형 대화•검색 시스템 (예: AutoGen, LangGraph)  
 - 시뮬레이션 : 군집 행동, 스마트시티, 자율주행 협력

## [생성형AI] Multi-Agent Reinforcement Learning (MARL)



**[정의]**

여러 Agent가 동일 / 연계 환경에서 상호작용하며 보상(Reward)을 기반으로 정책(Policy)을 학습하는 강화학습 구조

**[핵심/키워드]**

&lt;특징&gt;  
 - 상호의존성, 분산 학습 구조, 환경 불확실성, 지율시스템 지능화, 분산화, 실시간화

&lt;구성요소&gt;  
 - 에이전트 (Agent), 공유 환경 (Shared Environment), 보상 함수 (Reward Function), 통신 프로토콜 (Communication Protocol)

&lt;대표알고리즘&gt;  
 - MADDPG (Multi-Agent DDPG), QMIX, COMA, MAPPO

 - Cooperative MARL (전체 보상 극대화, 공동 목표, 협력)  
 - Competitive MARL (보상 상충, 제로섬, 이익 극대, 경쟁)

## [생성형AI] 에이전트 군집 (Swarm) 코딩



**[정의]**

여러 AI Coding Agent가 역할을 분담하고 상호협력하여 설계 / 개발 / 테스트 / 리뷰를 병렬 또는 반복 수행하는 개발방식

**[핵심/키워드]**

&lt;특징&gt;  
 - 자율성, 컨텍스트 이해, 분산제어, 협업 및 조정

&lt;구성요소&gt;  
 - 에이전트 : 자율성, 목표 지향성, 환경 인지  
 - Hand-off : 에이전트 간 제어권이나 작업을 위임  
 - 통신 메커니즘 : 메시지 큐, API호출  
 - Coordination : 전체 군집의 행동, 작업할당  
 - Environment : 코드베이스, 버전 관리 시스템(Git),개발 도구(IDE)

&lt;기술요소&gt;  
 - 멀티에이전트 오케스트레이션 : Microsoft Agent Framework, LangGraph, CrewAI, AutoGen  
 - LLM / 추론 모델 : GPT계열, Claude계열, Gemini계열, Open-source LLM  
 - 지식 / Context : Vector DB, RAG, Codebase Index  
 - 상태 / 메모리 : Shared State, Agent Memory, Task Memory  
 - 도구 실행 : Tool Calling, MCP, API, Sandbox  
 - 버전관리 : Git, GitHub, GitLab  
 - 테스트 / 품질 : Unit Test, Static Analysis, CI/CD  
 - 관찰 / 통제 : Tracing, Logging, Human-in-the-Loop, Guardrail

## [생성형AI] 하네스 엔지니어링 (Harness Engineering)



**[정의]**

프롬프트 단계를 넘어 AI에게 도구, 메모리, 제어 환경을 제공하여 실수를 방지하고 결과물의 품질을 높이는 엔지니어링 기술

강력한 AI 에이전트(LLM)가 안전하고 안정적으로 작업을 수행하도록 감싸는, 스캐폴딩(구조)과 피드백 루프를 설계하는 기술

**[핵심/키워드]**

&lt;구성 요소&gt;  
 - 파일시스템 & 저장소  
 - 코드 실행 & 샌드박스  
 - 컨텍스트 관리 : 컨텍스트 부패(Context Rot)방지  
 - 서브 에이전트 : 작업 분리 및 컨텍스트 격리  
 - Hook : 사전/사후 동작 자동 삽입 → 자동 검증 및 정책 적용  
 - Backpressure : 처리 과부하 시 실행 속도 자동 조절 → 파이프라인 안정성 및 처리량 보장

&lt;기술요소&gt;  
 - Context 관리 : Context Retrieval, Context Compression  
 - 실행환경 : Sandbox, Workspace / Runtime  
 - Tool 연계 : Tool Calling, MCP / API Integration  
 - Agent 오케스트레이션 : Workflow / Routing, Task Delegation / Handoff  
 - 검증 / 피드백 : Test / Validator, Retry / Feedback Loop  
 - 안전 / 운영 : Guardrail / Permission

&lt;설계전략&gt;  
 - 최소 개입(Minimal Intervention) : 모델이 스스로 교정할 수 없을 때만 개입  
 - 점진적 공개(Progressive Disclosure) : 최소 권한으로 시작, 필요에 따라 확장  
 - 빠른 실패와 복구(Fail-fast with Recovery) : 실패를 빠르게 감지하고 fallback(대체 동작) 메커니즘 제공  
 - 단순하게 시작(Start Simple) : 복잡한 제어 흐름 지양, 원자적 도구 제공  
 - 삭제를 위해 구축(Build to Delete) : 모듈식 아키텍처, 새 모델에 맞춰 교체 가능

## [생성형AI] 루프 엔지니어링 (Loop Engineering)



**[정의]**

AI 에이전트(Agent)가 사람의 지속적 개입 없이 목표와 완료 기준에 따라 작업을 스스로 발견, 계획, 실행, 검증하고, 결과를 반영해 반복 개선하도록 피드백 루프를 설계 운영하는 엔지니어링(공학)

**[핵심/키워드]**

&lt;동작 절차&gt;  
 1) 발견(Discover) : Agent 가 목표 이해, 필요 정보 탐색  
 2) 계획(Plan) : 수집 정보 기반 계획 수립  
 3) 실행(Execute) : 실제 작업 수행  
 4) 검증(Verify) : 결과물과 목표 검증  
 5) 반복(Iterate) : 검증 결과 기반 피드백, 개선 반복

 - 실행 조건 : 트리거(Trigger)  
 - 상태 관리 : 상태 / 메모리 (State / Memory)  
 - 반복 실행 : 에이전트 루프(Agent Loop)  
 - 검증 : 검증기 / 평가기(Verifier / Evaluator)  
 - 종료 제어 : 종료 조건 / 예산 (Stop Condition / Budget)  
 - 복구 / 재시도 : 재시도 / 복구 (Retry / Recovery)  
 - 인간 개입 : 인간 에스컬레이션 / 게이트(Human Escalation / Gate)

&lt;루프 엔지니어링 6가지 구성요소&gt;  
 1) 자동화(Automations) : 일정 기반 루프 실행  
 2) 워크트리(Worktrees) : 멀티 에이전트 작업시 독립 환경 제공  
 3) 스킬(Skills) : 프로젝트 규칙, 구조, 맥락 문서화  
 4) 플러그인/커넥터(Plugins & Connectors) : 외부 시스템 연결 작업  
 5) 서브에이전트(Sub-agents) : 에이전트 별 역할 분리  
 6) 메모리(Memory) : 루프 간 상태 유지, 실행 결과 기록

## [생성형AI] 재귀적 자기 개선 (Recursive Self-Improvement, RSI)



**[정의]**

AI가 자신의 성능/전략/구조를 평가하고 개선한 결과를 다시 다음 자기 개선에 활용하는 재귀적 개선 메커니즘

**[핵심/키워드]**

&lt;필요성&gt;  
 - 지속적 성능 향상, Al 연구개발 자동화, 환경/문제 변화 대응

&lt;동작&gt;  
 1) 자기 평가 > 2) 자기 수정 > 3) 검증 > 4) 개선된 AI

<위험성/개선방안>
 - 프론티어 AI 개발 가속 : 프론티어 페이싱  
 - 오류/정렬 실패 증폭 : 독립 검증  
 - 인간 통제권 약화 : 권한 제한/인간 개입  
 - 자원/비용 폭증 : 예산/종료 제어

## [생성형AI] 가디언 에이전트 (Guardian Agent)



**[정의]**

신뢰할 수 있고 안전한 AI상호작용을 지원하기 위해 다른 AI 에이전트를 감독하도록 설계된 AI에이전트

**[핵심/키워드]**

&lt;발전단계&gt;  
 - Phase1. 품질관리(Quality Control) > Phase2. 관찰(Observation) > Phase3. 보호(Protection)

&lt;기술영역&gt;  
 - 보안 (Security) : IDS, 접근 제어,암호화  
 - 관측 가능성(Observability) : 로그분석, APM  
 - 필터링/모니터링 : 데이터 필터  
 - 다중 에이전트 시스템 : 분산AI, 협력 자율시스템  
 - 에이전트오케스트레이션 : 워크플로 자동화

&lt;예상 영향 분야&gt;  
 - 보안 운영, 인간 개입형 모니터링, 자가 치유 프로세스, AI 신뢰 관리, 자율 시스템  
* AI 가드레일 → 가디언 에이전트

## [생성형AI] 봇시팅 (Bot-sitting)



**[정의]**

AI 결과물을 실무에 적용하기 위해 사람이 추가로 다듬는 작업

AI 결과물로 인한 맥락 재입력, 결과 검토, 오류 수정, 재프롬프트 등 추가 작업

**[핵심/키워드]**

&lt;등장 배경&gt;  
 - 높은 실패율, 시간의 재투입

&lt;봇시팅 작업의 유형 및 기술적 개선 방안&gt;  
 - 맥락 재입력 : AI가 조직 지식 또는 권한 맥락에 미접근 → RAG, KG(지식그래프), MCP  
 - 결과 검토 : 산출물 신뢰도 신호 부재 → 근거 인용, 신뢰도 스코어, LLM-as-Judge  
 - 오류 수정 : 할루시네이션 → 그라운딩, 스키마 강제, 툴 기반 검증  
 - 재프롬프트 : 의도-지시 간 표현 격차 → 프롬프트 템플릿, 컨텍스트 엔지니어링  
 - 에이전트 감독 : 자율실행 처리량보다 인간 검토 속도 느림 → 트레이싱, 가드레일, 인터럽트 조건 설정

&lt;봇시팅에 대한 고려사항&gt;  
 - 맥락 판단, 인간 역할 확대, 기술 한계, 핵심 과제

## [생성형AI] Agent Native Platform, 몰트북(Molt book)



**[정의]**

&lt;몰트북&gt;  
 - 인간이 아닌, AI 에이전트만 활동하는 전용 SNS로써, 게시글, 댓글 생성, 토론을 수행하는 AI 전용 소셜 네트워크 플랫폼

 - 인간이 아닌 AI 에이전트가 주도적으로 활동하며 상호작용하는 구조

**[핵심/키워드]**

&lt;운영 핵심 요소&gt;  
 - 자율성, 신원 레이어 : Identity Token 기반, Heartbeat

&lt;주요내용&gt;  
 - 주요목적 : AI Agent가 활동 주체인 Agent Native Platform  
 - 상호작용 : AI 간 자율토론, 게시, 평가  
 - 실행방식 : 주기적 (Heartbeat) 자동 실행  
 - 지능구조 : 다중 에이전트 협업, 역할 기반 구조  
 - 평판/신원 : 에이전트 평판, 토큰 기반 가능  
 - 데이터 생성 : AI가 스스로 콘텐츠 생성  
 - 산업적 의미 : 디지털 거버넌스, 에이전트 생태계 모델  
 - 사례 : 몰투북, 봇마당

## [생성형AI] 에이전트 커머스 (Agent Commerce)



**[정의]**

사용자의 의도를 파악한 Al Agent가 상품탐색, 금액비교, 최종결제와 배송확인까지 자율적으로 수행하는 새로운 상거래 모델

**[핵심/키워드]**

* 의도기반(Intent-based) 자동실행으로 전환  
&lt;절차&gt;  
 1) 거래절차 : 자연어 명령 > 의도 해석 및 탐색 (LLM) > Catalog API 연동 > 보안 토큰(SPT) 발행 > 결제 및 승인

&lt;핵심 요소&gt;  
 - LLM 의도 해석, 자동 결정 (플래닝/툴 선택), 표준화 상품 메타데이터, Catalog / Inventory API, A2A (Agent-to-Agent), MCP, SPT(Shared Payment Token)

&lt;결제 프로토콜&gt;  
 - ACP (OpenAI). AP2 (Google), UCP (Google), X402

## [생성형AI] AI Scientist (AI기반 자율 과학 연구 에이전트)



**[정의]**

인간 연구자를 보조하거나 대체해 과학적 발견, 가설 수립, 실험 설계, 논문 작성까지 수행하는 자율 연구형 인공지능 시스템

**[핵심/키워드]**

&lt;구현기술요소&gt;  
 - 대규모 언어모델(LLM), 지식 그래프(Knowledge Graph), 멀티모달 AI(Multimodal AI), 자동화된 과학탐구(Automated Science Discovery), 강화학습(Reinforcement Learning), 에이전트 협업 시스템(Multi-Agent Collaboration)

&lt;메커니즘 구성요소&gt;  
- LLM 기반 지식 엔진, AI 실험 디자이너, Al 해석자(Analyzer), AI 저자(Writer)

&lt;수행프로세스&gt;  
 1) Idea Generation(아이디어 생성 단계)  
  - LLM Ide / Plan Innovation, Novelty Check, Idea Scoring / Archiving  
 2) Experiment Iteration(실험 반복 단계)  
  - Experiment Template / Code Update via LLM, Experiment Execution Script, Numerical Data / Plots, Update Plan  
 3) Paper Write-Up(논문 작성 단계)  
  - Manuscript Template, Text Update via LLM, LLM Paper Reviewing

## [생성형AI] 모델 컨텍스트 프로토콜 (Model Context Protocol, MCP)



**[정의]**

Al 모델이 외부 애플리케이션, 도구, 데이터 소스 등과 안전하고 유연하게 상호작용할 수 있도록 설계된 개방형 통신 프로토콜

**[핵심/키워드]**

&lt;특징&gt;  
 - 개방형 표준, JSON-RPC 2.0, 양방향 연결, 범용성, 표준화, 보안, 신뢰성

&lt;주요기능&gt;  
 - Context-Aware, Agent-Ready, 플러그인 기반 확장성, 실시간 연결

&lt;구성요소&gt;  
 - MCP 핵심 : MCP Host, MCP Client, MCP Server  
 - AI 구성요소 : AI 모델(LLM), Context Provider  
 - Context Provider : Local Filesystem, Database, Web APIs  
 - 연동,확장 : MCP 브리지, 플러그인 도구

&lt;수행과정&gt;  
 - 1) 연결 설정 > 2) 컨텍스트 교환 > 3) 도구 호출 > 4) 결과 처리

&lt; 최근 변화 &gt;  
 - stateless, Long-running Task, Progressive Discovery, Agent / Enterprise Identity, Core+Extension

<보안 취약점 / 대응방안>
 - 인증·채널 미흡, 공급망 취약점, MCP 서버 환경, 권한 과다, 입력 검증 부재, 프롬프트 엔젝션, 툴 인젝션, Tool-Poison-Attack, 데이터 유출, 비밀관리 미흡, 가시성 부족, 자원남용, 멀티테넌시 취약  
 - mTLS, OIDC, TLS 1.2+, 코드서명, SBOM, SCA, 컨테이너 격리, AppArmor, SELinux, 권한 분리, DLP, PII 마스킹, 단기 토큰, 테넌트별 프로세스 관리

## [생성형AI] 비인간 디지털 신원 (Non-Human Identity, NHI)



**[정의]**

사람이 아닌 애플리케이션, 서비스, 기기, Al 에이전트 등이 시스템에 접근하고 인증을 수행하기 위해 사용하는 디지털 신원(Identity)

**[핵심/키워드]**

- 시크릿/토큰 : API Key, OAuth Token, JWT  
 - 서비스 계정 : K8s Service Account, GCP Service Account  
 - 워크로드 신원 : IAM Role for Service Account, SPIFFE/SPIRE  
 - 자동화 주체 : CI/CD (Jenkins, GitHub Actions), RPA 봇  
 - Al Agent : LLM 에이전트, MCP 서버, A2A 통신 주체  
 - 디바이스 : IoT/엣지 디바이스 인증서

 1) Provisioning(신원 등록) : Agent / Workload 고유 신원 생성 •동록  
 2) Attestation(실행 검증) : 실행 주체 / 실행 환경의 무결성 확인  
 3) Credential Issuance(자격증명 발급) : 단기 인증서 / Token 발급  
 4) Authentication(신원 인증) : Agent 신원 확인  
 5) Authorization(권한 부여) : 최소 권한(Least Privilege)기반 접근 허용  
 6) Audit(감사 기록) : 행동/권한/실행 이력 기록

 - API Key/Secret 탈취 : Short-lived Credential, Secretless 인증, 자동 Rotation  
 - Agent 위장/Impersonation : mTLS, Workload Attestation, 암호학적 Identity  
 - 과도한 권한 : Least Privilege, RBAC/ABAC, Scoped Token  
 - Credential 재사용 : Token Expiration, Rotation, Replay 방지  
 - 권한 위임 오남용 : Delegation Scope, Policy 기반 실행 통제  
 - 행동 추적 불가 : Audit Log, Trace, Identity-based Observability

## [생성형AI] Agent2Agent (A2A)



**[정의]**

서로 다른 AI Agent 간의 통신 및 협업을 위한 표준 프로토콜

**[핵심/키워드]**

&lt;특징&gt;  
 - 에이전트 간 상호운용성, 표준화된 통신 방식 (HTTP, JSON-RPC, SSE)  
 - 보안 중심 설계 (OAuth 2.0), 멀티모달 데이터, 오픈소스 표준

 - 에이전트 능력 수용, 기존 표준 기반 개발, 기본 보안 보장, 장기 실행 작업 지원, 모달리티 독립적 설계

&lt;동작과정&gt;  
 - 1) 발견 (Discovery) > 2) 작업요청 (Initialization) > 3) 처리 (Execution) > 4) 추가입력 (Interaction) > 5) 완료  (Completion) > 6) 푸시알림

&lt;구성요소&gt;  
 - 에이전트 메타 : Agent Card, Agent Discovery  
 - 통신 주체 : A2A서버, A2A 클라이언트  
 - 작업단위 : Task, Task Lifecycle  
 - 메시지 구조 : Message, Part, Artifact  
 - 통신 및 확장 : 통신프로토콜, STreaming, Push Notifications

<보안 취약점 / 대응방안>
 - 프롬프트 인젝션, 세션 하이재킹, 인증 우회, 공급망 공격, 교차 에이전트 공격  
 - 입력검증, TLS, OAuth2.1, RBAC, ABAC, 화이트리스트, 아티팩트 검증

## [생성형AI] 월드모델 (World Model)



**[정의]**

텍스트, 이미지, 영상을 넘어 현실 세계의 물리 법칙, 공간, 상호작용까지 이해, 시뮬레이션하는 인공지능 모델

AI가 주변 환경의 물리 법칙과 인과 관계를 예측하는 '개념 및 아키텍처'

**[핵심/키워드]**

&lt;특징&gt;  
 - 현실 세계의 내재적 이해, 멀티 모달리티, 상호작용 가능한 환경, 예측 및 상상 기반 학습  
 - 내부 학습 후 행동 전에 결과 예측

&lt;구성요소&gt;  
 - 입력 : 관찰 (Observation)  
 - 표현 : 상태 표현 (State Representation)  
 - 모델링 : 동역학 모델 (Dynamics Model)  
 - 예측 : Prediction  
 - 시뮬레이션 : Simulation  
 - 계획 : Planning

&lt;유형&gt;  
 1) 패러다임별 유형 : 명시적, 암묵적, 시뮬레이션, 하이브리드 / 지시  
 2) 목적별 유형 : 비디오 생성, 자율주행, 자율에이전트

&lt;평가&gt;  
 - Prediction Error / Rollout Quality / Environment Consistency / Policy Performance

## [생성형AI] LAM (Large Action Model, 대규모 액션 모델)



**[정의]**

사용자 목표/명령을 이해하고 계획/의사결정/도구 사용/행동 실행까지 수행하는 행동 중심 AI 모델

LLM의 언어 이해 / 추론 능력을 실제 API/UI/로봇/외부 시스템의 Action 실행으로 확장한 모델

**[핵심/키워드]**

<등장 배경 / 특징>
 - LLM의 텍스트 생성 중심 한계 극복, Al Agent의 자율적 Task 수행 요구  
 - Goal → Plan → Action → Feedback

&lt;구성요소별 기술요소&gt;  
 1) Perception (인지) : Vision Encoder, Multimodal Encoder, UI / Environment Parser  
 2) Goal Understanding(목표 이해) : Intent Understanding, Constraint Extraction, Context Modeling  
 3) Planning(계획) : Task Decomposition, Action Planning, ReAct / Reasoning Planning  
 4) Action Generation(행동 생성) : Action Tokenization, Tool / Function Calling, Policy Model  
 5) Execution (실행) : АРI / Tool Executor, Computer Use / GUI Control, Robot / Control Interface  
 6) Feedback / Verification(피드백/검증) : State Verification, Error Detection / Recovery, Replanning

<대표모델:>
 - Rabbit LAM, UI-TARS 계열 GUI Agent

## [생성형AI] 물리AI (Physical AI, 피지컬 AI)



**[정의]**

인공지능(Al)이 물리적 환경에서 직접 동작하며, 감각, 학습,행동을 수행하는 시스템

가상공간(디지털트윈,메타버스)과 실제 물리환경에서 학습한 지능을 기반으로 현실 세계에서 인식,판단, 행동을 수행하는 인공지능 기술

물리적인 세계를 이해하고,그 안에서 작용하는 힘과 에너지를 모델링하여 예측하고 제어하는 인공지능

**[핵심/키워드]**

&lt;유형&gt;  
 - 휴머노이드형, 자율주행차형, 드론형, AGV/AMR형

&lt;아키텍처별 기술요소 및 핵심기술요소&gt;  
 1) Perception Layer(인지)  
  - Visual Sensors : Camera / LiDAR / Computer Vision  
  - Tactile Sensors : Tactile Sensor / Haptic Sensor  
  - Position Sensors : GPS / IMU / Encoder / SLAM  
  - Force Sensors : Force / Torque Sensor  
  - Sensor Fusion : Multimodal Encoder / Sensor Fusion  
 2) Cognitive Layer(생각/판단)  
  - Multimodal Understanding : VLM  
  - World Modeling : LWM  
  - Physics Models : Physics-informed Model / Digital Twin  
  - Decision Making : Action Planning / MPC  
  - Adaptive Learning : Reinforcement Learning / Imitation Learning  
  - Simulation Transfer : Sim-to-Real / Domain Randomization  
 3) Action Layer(행동)  
  - Action Intelligence : VLA  
  - Motion Control : Trajectory Planning / Motion Control  
  - Robotic Actuators : Motor / Servo / Actuator Control  
  - Force Application : Force / Impedance Control

## [생성형AI] 로봇 파운데이션 모델 (Robotic Foundation Model)



**[정의]**

대규모 데이터와 사전학습(pretraining)을 기반으로 구축된 범용 인공지능 모델로, 로봇의 지각, 계획, 조작 등 다양한 도메인 전반에서 활용이 가능한 범용 로봇 제어 아키텍처

다양한 로봇 작업과 환경에 적용 가능한 사전 학습된 AI 모델

**[핵심/키워드]**

&lt;기술요소&gt;  
 - 인지/상호작용 : 비전(Vision), 언어(Language), 센서(Sensors), 행동(Action)  
 - 이해/추론 : 멀티모달 인식(Multimodal Perception), 자연어 이해(NLU), 의미 매핑(Semantic Mapping), LLM/VLM  
 - 계획/제어/학습 : 상위 계획(High-level Planning), 동작 제어(Motion Control), 디지털 트윈/ 시뮬레이션, 강화학습

## [생성형AI] 휴머노이드 로봇 (Humanoid Robot)



**[정의]**

인간과 유사한 형태(팔, 다리, 얼굴)를 가진 로봇

인간과 유사한 형태와 동작을 갖춘 로봇으로, Al, 로보틱스, 센서 기술이 결합되어 인간과 상호작용 가능한 로봇

**[핵심/키워드]**

&lt;유형&gt;  
 - 외형 기반 분류 : 완전, 부분, 기능 특화  
 - 기능 및 역할 기반분류 : 산업용, 서비스, 의료, 연구 및 실험용  
 - 이동 방식에 따른 분류 : 이족 보행형, 바퀴 기반, 혼합형

&lt;기술요소&gt;  
 1) 센싱 시스템  
  - 카메라 : RGB, Depth, 열화상  
  - 각종 센서 : 가속도, 자이로, 촉각, 초음파 센서  
 2) 인공지능 시스템  
  - AI반도체 : NVIDIA Jetson AGX Orin, Google EdgeTPU,Tesla Dojo AI  
  - 시스템 SW : ROS, RTOS, YOLO  
  - 애플리케이션 SW : 음성인식AI, 얼굴인식AI, 행동예측AI  
  - LLM : GPT-4, Gemini, Mistral, LLama2  
 3) 액추에이션 시스템  
  - 서보 시스템 : Dynamixel XH/XM시리즈, Maxon ECX 모터  
  - 모터 : BLDC모터, 유압 모터  
  - 감속기 : 하모닉 감속기, 유성 기어 감속기  
  - 제어기 : PID제어기, MPC, 강화학습 기반 제어 (PPO, SAC)  
 4) 바디 및 기타 시스템  
  - 금속 합금 : 알루미늄 합금, 티타늄 합금  
  - 카본 파이버 : CFRP  
  - 플라스틱 파트 : ABS, PC  
  - 배터리 팩 : 리튬이온배터리, 고속 무선 충전 기술

## [생성형AI] 자율주행 AI (Autonomous Driving AI)



**[정의]**

인공지능 기술을 활용하여 인간 운전자의 개입 없이 차량이 스스로 주변 환경을 인식하고, 판단하며, 주행 경로를 결정하여 운행하는 기술 체계

**[핵심/키워드]**

&lt;자율주행 AI 기술 유형 및 주요 기술&gt;  
 - 규칙 기반(Rule-based) : 사람이 정의한 규칙, FSM, Rule-based Control  
 - 모듈형(Modular AI) : 분리구조, CNN, SLAM, EKF, Planning 알고리즘 (A*, MPC)  
 - End-to-End Al : 하나의 신경망, Deep Neural Network, Transformer 기반 모델

&lt;자율주행 AI 센싱 및 알고리즘&gt;  
 1) 센싱  
  - 카메라 : CNN, Vision Transformer (ViT)  
  - 라이다 (LiDAR) : PointNet, Voxel Net  
  - 레이더 (Radar) : FMCW Radar, CFAR  
  - 초음파 : Time-of-Flight (ToF)  
 2) Al알고리즘  
  - 인식(Perception) : YOLO, Faster R-CNN  
  - 센서퓨전 : BEVFormer  
  - 위치추정 (Localization) : EKF, SLAM  
  - 예측(Prediction) : Transformer  
  - 경로계획/제어 : A*, MPC

## [생성형AI] 엣지 AI (Edge AI)



**[정의]**

&lt;기술적 개념&gt;  
 - 데이터가 생성되는 디바이스 또는 인근 네트워크 엣지에서 AI모델을 직접 실행하여 분석/처리하고, NPU,TPU,FPGA 등 전용 AI가속기와 모델 경량화, 최적화 기술을 활용하는 기술

&lt;아키텍처 개념&gt;  
 - 중앙 클라우드로 데이터를 전송해 분석하는 기존 방식과 달리, 로컬 디바이스나 엣지 서버에서 즉시 분석,처리하여 지연을 최소화하고 필요 시 클라우드와 연계하는 분산형 AI 처리구조

**[핵심/키워드]**

&lt;특징&gt;  
 - 실시간/저지연성, 데이터 프라이버시, 보안 강화, 맞춤형 개인화, 네트워크 비용 절감, 에너지 효율성

&lt;엣지 컴퓨팅 기반 생성형 AI기술요소&gt;  
 - 하드웨어 : GPU, NPU, TPU, FPGA  
 - AI 모델 최적화 : 모델경량화, 양자화, 프루닝, 지식증류  
 - 엣지 인프라 아키텍처 : MEC기반 분산 처리 구조  
 - 온디바이스AI : 단말 내 모델 실행  
 - 연합학습 : 모델 파라미터만 공유  
 - 네트워크 융합 : 5G/6G, IoT, MEC통합  
 - 데이터 프라이버시 : 차등 프라이버, 보안 모듈(TPM/TRM)  
 - 실시간 처리·추론 : 자율주행, 스마트팩토리, AR/VR, 헬스케어  
 - 그래프 신경망(GNN) : GraphNeuralNetwork기반 모델  
 - 그래프 데이터베이스 : Graph DB(Neo4j 등)  
 - SLM : 경량화된 언어 모델

&lt;활용분야&gt;  
 - 제조업 : 생산 공정 최적화  
 - 헬스케어 : 의료 영상 실시간 진단 지원  
 - 스마트시티 : 교통 흐름 실시간 관리  
 - 금융 서비스: 사기 탐지 시스템  
 - 국방/보안 : 엣지 기반 AI 경계 감시 시스템

## [생성형AI] 양자 AI (Quantum AI)



**[정의]**

- 양자 컴퓨팅 기술을 인공지능(AI)알고리즘에 적용해 성능을 극대화하는 융합 기술

**[핵심/키워드]**

* 양자중첩, 얽힘 등의 양자역학 원리를 활용해 고속 병렬 연산 가능

&lt;기술요소&gt;  
 -  머신러닝 : 양자머신러닝(QML)  
 -  최적화 : QAOA, VQE  
 -  자연어처리 : QNLP  
 -  이미지 처리 : FRQI, NEQR  
 -  시스템 구조 : 하이브리드 아키텍처  
 -  회로 설계 : 양자 회로 설계  
 -  데이터 처리 : 양자 데이터 표현/샘플링

&lt;활용분야&gt;  
 - 신약 개발, 금융 모델링, 물류 최적화, 고차원 AI 학습

&lt;현재한계&gt;  
 - 양자 하드웨어 개발 미비, 오류율·디코히런스 문제 존재

## [생성형AI] 양자 머신러닝 (QML, Quantum Machine Learning)



**[정의]**

양자컴퓨팅의 원리(중첩, 얽힘, 간섭)를 활용하여 머신러닝 알고리즘을 고도화하는 기술

**[핵심/키워드]**

&lt;절차&gt;  
 1. 데이터 인코딩 (큐비트 변환) > 2. 양자 회로 설계(PQC) > 3. 하이브리드 학습 (양자+고전) > 4. 패턴 추출 > 5. 오류 보정 > 6. 실행 환경(스택)

&lt;주요 알고리즘 및 모델&gt;  
 1) 머신러닝  
  - QSVM(Quantum SVM), 양자 커널 방법, Variational Classifier/Regressor, Q-means, Quantum PCA, Quantum KNN  
 2) 강화학습  
  - QRL(Quantum Reinforcement Learning), Quantum Q-Learning/Variational Q-Learning, Quantum Policy Gradient/Actor-Critic, Quantum DQN, Quantum Bandits , QAOA기반 RL  
 3) 최적화 및 시뮬레이션  
  - VQE(Variational Quantum Eigensolver), QAOA(Quantum Approximate Optimization Algorithm)  
 4) 선형대수  
  - HHL 알고리즘  
 5) 생성모델  
  - QGAN, QBM, Born Machine

&lt;한계점&gt;  
 - 노이즈/디코히런스, 스케일 한계, 데이터 로딩 병목, Barren Plateau, 벤치마크 문제

## [생성형AI] AI-DLC (AI-Driven Development Life Cycle)



**[정의]**

AI가 SDLC 전 과정의 계획, 생성, 실행을 주도하고, 인간이 검증, 의사결정을 수행하는 AI 중심의 개발 방법론

**[핵심/키워드]**

* AI-driven + Human Oversight, AI 생성+사람 검증  
&lt;필요성&gt;  
 - 기존 SDLC 비효율성, AI 보조형 개발의 한계, 전주기 통합, 신속 대응 요구  
 - Al Agent 7E Spec-driven / Agentic Development

&lt;수행단계 별 핵심 Activity&gt;  
 1) Inception : 무엇을 만들지 정의, Unit of Work 도출, User Story, NFR, Risk 정의  
 2) Construction : 어떻게 만들지 구현, Domain / Architecture,  짧은 실행주기인 Bolt 단위  
 3) Operation : 어떻게 배포, 운영, Telemetry 분석 및 모니터링, 이상 탐지 장애 대응

## [생성형AI] SDD (Spec-Driven Development)



**[정의]**

명세를 단일 진실 공급원(SSoT)으로 활용하여 AI가 구현, 테스트, 문서를 생성하고, 사람은 설계, 검증, 개선을 담당하는 개발 방식

**[핵심/키워드]**

- 명세를 단일 기준으로 코드-명세 불일치 최소화, AI 기반 구현, 자동화, 코드 생성 확산  
 - 개발 중심이 코드 작성 → 명세 기반 구현, 명세 중심 개발 패러다임

&lt;핵심원칙&gt;  
 - Spec First(명세 우선), Spec as Source of Truth(명세 단일 기준)  
 - Al Guided by Explicit Rules(명시적 규칙 기반 AI 수행), Feedback Back to Spec(명세 중심 피드백 반영)

&lt;절차&gt;  
 1) 스펙 정의 > 2) 계획 수립 > 3) 가드레일 설정 > 4) AI 구현 생성 > 5) 검증 및 피드백

## [생성형AI] 전방 배치 엔지니어링 (Forward Deployed Engineering, FDE)



**[정의]**

고객 현장에 직접 배치되어 문제 정의, 기술 구현, 운영 적용까지 수행하는 활동

엔지니어가 고객, 현업 가까이에 직접 배치되어 실제 업무 문제를 정의,데이터, AI, 소프트웨어 솔루션을 구현해 운영까지 연결하는 실행중심 방식 (팔란티어 정의)

**[핵심/키워드]**

* AI를 만드는 역할이 아니라, 현장에서 실제로 작동하게 만드는 실행체계  
&lt;주요역할&gt;  
 - 업무 문제 정의, 데이터 / 프로세스 분석, AI 모델, 시스템 연계, 현장 적용, 검증, 운영 안정화

&lt;핵심내용&gt;  
 - 현장 직접 배치, 융합형 엔지니어, 현장 실행형

&lt;주요역량&gt;  
 - 주요 활동 : API, 데이터, 기존 시스템 통합  
 - 필요 역량 : 분석 능력, 커뮤니케이션, 문제해결  
 - 운영 방식 : 공동 수행, 짧은 개발 및 검증 반복, 현장 적용 후 표준화 및 확산  
 - 기존 SI 차이 : 현장 참여, 문제 정의부터 운영 개선까지 지속 수행  
 - 기존 컨설팅 차이 : 직접 분석, 설계, 개발, 배포, 운영 수행  
 - 적용 영역 : 물류 최적화, 고객 서비스, 생성형 AI, 업무 자동화 등  
 - 성과 지표 : 시간 절감, 처리속도 향상, 운영 안정성 등

&lt;주요기술&gt;  
 - RAG, 데이터 파이프라인, 프로토타이핑, API 및 워크플로우 설계, AI Agent 적용

&lt;대표기업&gt;  
 - 팔란티어(Palantir), OpenAI, Salesforce

## [생성형AI] 바이브 코딩 (Vibe Coding)



**[정의]**

사용자가 자연어로 원하는 기능/결과를 설명, LLM / AI Coding Agent가 코드 생성, 사용자는 결과를 확인하며 프롬프트 기반으로 반복 수정하는 개발방식

**[핵심/키워드]**

&lt;특징&gt;  
 - 자연어·음성 명령만으로 소프트웨어 구성, 의도 중심 개발

&lt;개발사이클&gt;  
 1) Ideation (아이디어화) > 2) Prompting (프롬프팅) > 3) Generation (생성)  
 > 4) Testing(테스팅) > 5) Deployment (배포) > 6) Feedback / Iteration (피드백 / 반복)

&lt;개발사이클별 기술요소&gt;  
 1) Ideation : Requirement Prompting / Spec / User Story / Prototype Design  
 2) Prompting : Prompt Engineering / Context Engineering / Few-shot Prompt / MCP  
 3) Generation : LLM / AI Coding Agent / Code Generation / Tool Function Calling  
 4) Testing : Unit Test / Test Automation / Static Analysis / Security Scan  
 5) Deployment : CI/CD / DevOps / Container / Cloud Deployment  
 6) Feedback/Iteration : Error Log / Observability / User Feedback / Agentic Loop

&lt;주요 도구&gt;  
 1) 요구사항 문서화/모델링 : Markdown, PRD, BRD, Mermaid  
 2) 개발환경/플랫폼 : Cursor, Windsurf, Replit, MCP  
 3) 협업 운영/배포 : GitHub, CI/CD, Jenkins, Slack, Notion

* 토큰 사용량 증가 : Context 최적화, Prompt 압축, 불필요한 대화 이력 제거, 캐시 활용  
* AI 사용 비용 증가 : Model Routina, Token Budaet, Usage Monitorina, 비용 한도 설정

## [생성형AI] LiteLLM 공급망 공격



**[정의]**

정상 패키지로 위장한 LiteLLM 변조 버전을 PyPI와 같은 공개 저장소에 유포함으로써 사용자의 신뢰를 악용하여 수행되는 소프트웨어 공급망 공격

**[핵심/키워드]**

&lt;특징&gt;  
 - 확산성, 지속성, 은밀성

 - 대상 : 인공지능 오픈소스 라이브러리 LiteLLM  
 - 공격 주체 : 해킹 그룹 TeamPCP  
 - 유포 방식 : PyPI에 악성 코드가 삽입된 버전(1.82.7, 1.82.8) 배포  
 - 동작 방식 : 설치 및 실행시 자동으로 백도어 실행  
 - 주요 목표 : 자격 증명(Credential) 탈취  
 - 탈취 대상 : SSH 키, 클라우드 인증 정보, 쿠버네티스 시크릿, 환경 변수(.env)

&lt;공격절차&gt;  
 1) 악성 패키지 제작 > 2) PyPI 업로드 > 3) 사용자 설치 > 4) 백도어 실행 > 5) 정보 수집  
 > 6) 외부 전송 > 7) 권한 확장

&lt;대응방안&gt;  
 - 가시성 확보 : SBOM / AI-BOM 구축  
 - 접근 통제 : 최소 권한 원칙 적용  
 - 유출 차단 : Egress 트래픽 통제  
 - 운영 관리 : 보안 점검 및 업데이트

## [생성형AI] AI OS (Artificial Intelligence Operating System)



**[정의]**

대규모 언어모델(LLM)을 운영체제의 뇌로 삼아, 지능형 에이전트로서의 기능을 내재화한 새로운 패러다임의 운영체제

LLM을 중심으로 에이전트 기반 작업 수행과 컨텍스트 자원 관리를 통합 제공하는 지능형 운영체제

**[핵심/키워드]**

&lt;특징&gt;  
 - LLM 커널 역할 수행, 다중 에이전트 환경

 1) Application Layer : Agent, Applications, AIOS SDK  
 2) Kernel Layer (LLM) :  
  - LLM 관리자(Core), LLM 스케줄러, 컨텍스트 관리자, 메모리 관리자  
  - 저장소 관리자, 도구 관리자, 접근 관리자  
 3) Kernel Layer (OS) : OS kernel  
 4) Hardware Layer : CPU, GPU, Memory, Disk, 주변 장치

&lt;주요기능&gt;  
 - 스케쥴 관리 : LLM 스케줄링  
 - 메모리 관리 : 토큰 기반, 벡터 DB, 장기 메모리, 단기 메모리  
 - 컨텍스트 관리 : 스냅샷, KV Cache  
 - 스토리지 관리 : LLM API 호출, AI OS SDK

## [생성형AI] AI 웹 브라우저 (Artificial Intelligence Web Browser)



**[정의]**

기존 웹 탐색 기능에 LLM / 멀티모달 AI / Agent 기능을 결합, 사용자의 의도를 이해하고 웹 정보를 검색/요약/비교/추론/행동 실행까지 지원하는 지능형 브라우저

**[핵심/키워드]**

&lt;특징&gt;  
 - Context-Aware Browsing + Agentic Action  
 - AI비서 내장, 콘텐츠 요약, 고도화된 개인화, 작업 자동화

&lt;기술요소&gt;  
 - 인공지능 : LLM, NLP, Edge AI  
 - 인식 : Context 인식, Agent Mode, Contents 분석/요약  
 - OS 운영 : 개인화, WebGPU, 스킬시스템, 헤드리스 브라우저

&lt;주요내용&gt;  
 - 검색방식 : 자연어 이해, 대화형  
 - 결과제공 : 요약, 분석, 맥락 기반 답변  
 - 주요기능 : 콘텐츠 요약, 질문 답변, 자동화  
 - UX : 대화영, 능동적  
 - 개인화 : 맞춤형 제공

&lt;동향&gt;  
 - Perplexity Cornet, Arc Browser, Edge Copilot, Chrome Gemini, Brave Leo

## [생성형AI] CPMAI (Cognitive Project Management for AI)



**[정의]**

PMI(Project Management Institute)프레임워크 기반, AI, ML프로젝트를 체계적으로 관리하기 위한 전문 방법론

**[핵심/키워드]**

&lt;필요성&gt;  
 - AI프로젝트 특성, PM방식 리스크 관리 한계, 데이터분석 강화, 생애주기 접목

&lt;6단계 프로세스 절차&gt;  
 1. 비지니스 이해 : 비즈니스 문제, 목표, KPI  
 2. 데이터 이해 : 접근성, 품질, 편향 평가  
 3. 데이터 준비 : 데이터 경제, 표준화, 가공  
 4. 모델 개발 : 알고리즘, 모델 선정  
 5. 모델 평가 : 성능평가  
 6. 운영 모니터링 : 배포 및 성능 모니터링

 &lt;기대 효과&gt;  
 - 프로젝트 실패율 감소, 데이터 활용 역량, 비즈니스 목표 성과, AI도입 가속화

## [생성형AI] SNAP (Software Non-functional Assessment Process)



**[정의]**

IFPUG에서 제정한 소프트웨어 비기능 요구사항(NFR)의 규모를 정량적으로 측정하는 방법

**[핵심/키워드]**

* 기능 요구사항 측정 FPA(Function Point Analysis) 보완  
* 4개 Category / 14개 Sub-category 구성  
* ISO/IEC/IEEE 32430:2025  
&lt;필요성&gt;  
 - 기능/비기능 통합 반영, 데이터/모델 개발 공수 정량화, AI 생명주기 전체 비용 반영  
 - 객관적 발주/성과관리 기준 확보, 기능 규모 + 비기능 규모를 활용한 전체 SW 규모 분석

&lt;절차&gt;  
 - 서브 카테코리 식별 > 비기능 규모 식별 > 비기능 규모 계산

&lt;측정항목&gt;  
 1. Data Operations(데이터 처리) :  
  - 데이터 입력 검증, 논리/수학 연산, 데이터 포맷팅, 내부 데이터 이동  
  - 데이터 구성 기반 사용자 부가가치 제공  
 2. Interface Design(인터페이스 설계)  
  - 사용자 인터페이스, 도움말 방식, 다중 입력 방식, 다중 출력 방식  
 3. Technical Environment(기술 환경)  
  - 다중 플랫폼, 데이터베이스 기술, 배치 프로세스  
 4. Architecture(아키텍처)  
  - 컴포넌트 기반 소프트웨어, 다중 입출력 인터페이스

## [생성형AI] 토큰 이코노미 (Token Economy)



**[정의]**

Al 모델이 처리, 생성하는 Token을 AI의 생산, 소비, 비용, 수익 단위로 보고 Token 생산성과 단위 비용을 중심으로 AI 인프라의 경제성을 관리하는 체계

**[핵심/키워드]**

* Al Factory가 생산하는 핵심 산출물은 Token 기반 Intelligence  
* Al Factory는 데이터와 에너지를 Token으로 변환하는 인프라  
* Token = 생산물, 가치 측정 단위  
&lt;핵심지표&gt;  
 - TPS(Token Per Second), TTFT, Token/Watt, Cost per Token

&lt;주요전략&gt;  
 - 토큰 맥싱(Token Maximizing) : 긴 문맥 처리와 고도화된 추론 성능에 집중  
 - 토큰 미니마이징(Token Minimizing) : 적은 토큰으로 동일 성능을 구현해 비용 절감

## [생성형AI] 인공지능 팩토리 (AI Factory)



**[정의]**

데이터/모델/컴퓨팅/운영체계를 통합하여 AI 모델/Agent와 Token 기반 Intelligence를 지속적으로 생산/배포/최적화하는 AI 생산 플랫폼

**[핵심/키워드]**

* GPU, HBM, 서버, 데이터센터, 냉각 설비를 단일 체계로 연결  
 → 학습•추론 성능과 운영 효율 동시 최적화  
&lt;특징&gt;  
 - 전력, 데이터를 투입해 토큰 생산, 하나의 생산체계, 인공지능 전 생애주기 지원

&lt;계층구분&gt;  
 - 애플리케이션 & 모델 계층 : 데이터 수집부터 학습, 추론까지 Al 전 생애주기 지원  
 - 인프라 계층 : 서버, 네트워크, 스토리지 및 최첨단 냉각 설비  
 - 칩 계층 : GPU, HBM 등 초고속 연산 특화 반도체  
 - 에너지 계층 : 막대한 연산을 뒷받침하는 대규모 전력 공급망

## [생성형AI] 다크 팩토리 (Dark Factory)



**[정의]**

AI, IoT 등 최첨단 기술을 활용해 사람의 개입 없이 생산, 검사, 포장 등 모든 공정이 자동으로 이뤄지는 무인화된 암흑공장

**[핵심/키워드]**

&lt;특징&gt;  
 - 완전 자동화, 24시간 무중단 생산, 비용 절감, 안전성 향상, 사람 개입 거의 없음

&lt;기술요소&gt;  
 - 데이터 수집 : lOT 센서/lIoT, RFID/바코드, OPC-UA/MQTT, Edge Gateway  
 - 지능형 분석 : Al/ML 모델, MLOps, AutoML  
 - 실행/제어 : 로보틱스/피지컬AI, AVG/AMR, PLC/MES 연동  
 - 통합 운영 : CPS, 디지털트윈, SDF

&lt;동향&gt;  
 - 중국 : 샤오미 (베이징 다크 팩토리), 폭스콘 (선전 등끈공장)  
 - 독일 : 지맨스 (암베르크 공장)  
 - 미국 : 테슬라 (상하이 기가 팩토리)  
 - 일본 : 화낙 (로봇 제조로봇)  
 - 한국 : 현대자동차 (미국 메타플랜트), 다이소 (세종허브센터), 삼성전자 (Autonomous Fab)

## [생성형AI] 인공지능 데이터센터 (AIDC)



**[정의]**

대규모 인공지능 연산(학습, 추론)에 특화된, 고성능 GPU, 가속기, 초고속 네트워크, 대용량 스토리지, 고효율 냉각 전력 시스템 등의 IT인프라를 제공하는 데이터 센터

**[핵심/키워드]**

&lt;특징&gt;  
 - 고성능 Al 전용 하드웨어 : GPU, TPU, NPU 등 AI 가속기  
 - 초저지연, 고대역폭 네트워크 : InfiniBand, Ultra Ethernet, NVLink 등  
 - 고밀도 전력냉각 인프라 :  수백 KWV급 랙 전력, 액침냉각, 수랭식

&lt;기술요소&gt;  
 - 컴퓨팅 : GPU / NPU / TPU / AI Accelerator  
 - 메모리/인터커넥트 : HBM, CXL  
 - 네트워크 : NVLink / InfiniBand / 400G•800G Ethernet  
 - 스토리지 : NVMe SSD / NVMe-oF / Parallel File System / Object Storage  
 - 전력 : High-density Power / UPS / PDU / HVD/  
 - 냉각 : D2C Liquid Cooling / CDU / Immersion Cooling / HVAC / Air Cooling  
 - AI 플랫폼 : Container / Kubernetes / Scheduler / MLOps / Model Serving  
 - 운영/관리 : DCIM / Observability / Predictive / Maintenance  
 - 보안 : Zero Trust / IAM / NHI / Encryption / Micro-segmentation  
 - 친환경/지속가능성 : PUE / Renewable Energy / Energy Optimization  
 - 확장성/유연성 : Modular Data Center / Scale-out Architecture

## [생성형AI] 인공지능 데이터센터 (AIDC) 냉각기술



**[정의]**

서버, 스토리지, 네트워크 장비 등 IT 장비에서 발생하는 열을 효과적으로 제거하여 시스템의 안정적인 운영과 에너지 효율을 유지하기 위한 열 관리(Thermal Management) 기술

**[핵심/키워드]**

&lt;성능지표&gt;  
 - 냉각 에너지 효율 평가(PUE, VUE, CUE, DCiE) + 에너지 재사용/총효율 지표(ERE, TUE)

## [생성형AI] All reduce



**[정의]**

Al 분산 컴퓨팅 환경에서 여러 GPU 노드가 각자 연산, 보유한 데이터를 하나의 연산 결과로 통합(reduce), 결과를 모든 노드에 동일하게 배포(broadcast)하는 집합 통신 연산 기술

**[핵심/키워드]**

&lt;기술요소&gt;  
 - 통신 라이브러리 : NCCL  
 - 노드 내부 : NVLink / NVSwitch  
 - 노드 외부 : Infiniband  
 - 데이터전송 : RDMA  
 - GPU 통신 : GPU Direct  
 - 집계 방식 : Ring Al-Reduce, Tree Al Reduce  
 - 오프로딩 : In-Network Computing

&lt;동작&gt;  
 1) 각 노드 로컬 계사 > 2) All-Reduce 연산 > 3) Broadcast

* Ring All-Reduce, Reduce-Scatter, AI-Gather, Closed Loop

## [생성형AI] GPUaaS (GPU as a Service)



**[정의]**

자체 GPU서버 구축 없이,클라우드에서 필요한 만큼의 GPU 리소스를 할당 받아 사용하는 서비스 모델

**[핵심/키워드]**

&lt;특징&gt;  
 - 온디맨드 확장성, 비용 효율성, 접근성,유연성, 빠른 연산성능, 동적할당, 회수

 &lt;사용절차&gt;  
 1. GPU사양, 환경 선택 >  2. 컨테이너 또는 VM 생성 >  3. 작업 실행 >  4. 사용료 지불

&lt;기술요소&gt;  
 - GPU 하드웨어, NVIDIA A100, V100, RTX등 고성능 GPU, 과금 시스템  
 - 클라우드 인프라, 병렬처리 프레임워크(CUDA, cuDNN)  
 - ML프레임워크(TensorFlow, PyTorch), 가상화,컨테이너 기술 (Docker, Kubernetes)  
 - 멀티 GPU클러스터 관리 기술, 운영체제 및 클러스터링 기술  
 - 고속 네트워크(GbE, InfiniBand), 고성능 스토리지(SSD/NVMe)  
 - 네트워크 보안 기술(VPN, TLS), IAM(Identity Access Management)  
 - 데이터 암호화 기술, 모니터링 도구(Prometheus, Grafana)  
 - 클라우드 관리 플랫폼, 자동 스케일링(Auto-scaling)기술

&lt;서비스유형&gt;  
 - BareMetal GPU, Virtual GPU(vGPU), Container GPU,  Serverless GPU

## [생성형AI] LPU (Language Processing Unit)



**[정의]**

대규모 언어 모델(LLM)의 추론 성능을 극대화하기 위해 설계된 반도체 칩

AI 추론을 위해 연산/메모리/통신을 결정적으로 스케줄링하고 스트리밍 방식으로 처리하여 저지연/고처리량 LLM 추론을 제공하는 AI 전용 프로세서

**[핵심/키워드]**

* 주요 기능 : LLM 추론 가속. 지연시간 최소화  
&lt;특징&gt;  
 - TSP(Tensor Streaming Processor): 스트림 방식 데이터 처리, 언어 처리  
 - SRAM 중심 설계: 칩 내부 고속 SRAM 직접 활용  
 - 결정론적 아키텍처(Deterministic Architecture): 실행 시간 정확한 예측, 데이터 흐름 최적화  
 - 소프트웨어 예약 네트워킹: 비결정성 제거, 효율성과 예측 가능성 보장

&lt;구성 요소&gt;  
- 처리장치 : TSP, MXM, VXM, SXM  
- 저장장치 : On-chip SRAM(MEM)  
- 데이터 이동 : Streaming Register File (SRF)  
- 칩 간 통신 : C2C(Chip-to-Chip) Interconnect  
- 네트워크 : Deterministic Network  
- 제어/스케줄링 : Software-defined Static Scheduling  
- 실행 방식 : Deterministic Dataflow

## [생성형AI] ZAM (Z-Angle Memory)



**[정의]**

기존 HBM (고대역폭 메모리)의 발열 문제를 해결하기 위해 D램을 수직이 아닌 사선(Z) 형태로 배치하고 연결해, 대용량·고대역폭·저전력 성능을 구현한 차세대 메모리 (인텔의 전략)

**[핵심/키워드]**

&lt;특징&gt;  
 - 사선 회로 배선, 중앙 백본(backbone) 방식, 발열 제어 개선(중앙부 발열 빠르게 발산)  
 - 고용량·고성능(D램 면적 확장, HBM 대비 2~3배 저장)

&lt;기술요소&gt;  
 - Z-Angle : 대각선 인터커넥트  
 - One TSV : 단일 TSV (+contact ring)  
 - 구리-구리 Hybrid Bonding : Cu-Cu 직접 접합  
 - EMIB Packaging : 고속 다이간 통신  
 - Non-TSV : 대체 인터커넥트 경로

## [생성형AI] HBF (High Bandwidth Flash)



**[정의]**

HBM에 쓰이는 실리콘 관통 전극 (TSV)기반 적층을 NANDFlash에 적용해 대역폭을 높이고 용량을 키우는 메모리

**[핵심/키워드]**

&lt;등장배경&gt;  
- HBM 용량 확장의 구조적 제약, 전력발열 부담, AI 모델 추론 등의 TB 만족 어려움

&lt;특징&gt;  
 - NAND Flash,TSV 통한 적층, GPU직접 결합, I/O병렬 연결

&lt;기술요소&gt;  
 - Nand Flash, TSV, CBA (Base Die, 웨이퍼 별도 제조), 온-패키지 FTL (칩, 하드웨어)

## [생성형AI] 공동 패키징 광학 (Co-Packaged Optics, CPO)



**[정의]**

네트워크 스위치 ASIC 바로 옆에 광통신 엔진(Optical Engine)을 함께 배치해 데이터를 빠르게 광신호로 변환 전송하는 기술

AI 연산 칩(GPU, ASIC 등)과 광학 소자를 하나의 패키지 기판 위에 직접 통합하는 차세대 반도체 패키징 기술

**[핵심/키워드]**

* 주로 AI 데이터센터의 서버.GPU 클러스터 간 네트워크에 적용  
&lt;특징&gt;  
 - 광 신호 전송(구리선 대신 광 신호로 데이터 전송), 동일 패키지 사용  
 - 저전력, 초고대역폭·저지연·고집적화(Tbps급 전송)

&lt;연결 대상&gt;  
 - 칩↔칩(GPU↔GPU·CPU↔GPU), 칩↔스위치, 스위치↔스위치

&lt;구성요소&gt;  
 - 스위치 ASIC : SerDes, Digital PHY  
 - 광학엔진 : 실리콘 포토닉스, InP  
 - MZM 변조기 : 마하-젠더 변조기  
 - PD 수신기 : 포토 다이오드 어레이  
 - WDM 다중화 : CWDM, DWDM  
 - 레이저 광원 : CW 레이저, EIC  
 - 패키지 기판 : 패키징, UCIe

 - 칩↔패키지 내 광엔진 직접 연결→바로 광 전송  
 - Substrate 기반 통합 구조로 전기 구간 최소화

## [생성형AI] 프론티어 AI (Frontier AI)



**[정의]**

기존 AI 기술을 넘어서는 기술로, 인간의 복잡한 문제 해결 능력을 모방하거나 능가하는 AI

파운데이션 모델과 유사하지만, 위험한 기능 발현 가능성이 높은 인공지능

기존의 인공지능(Al) 모델보다 뛰어난 능력을 보유하여, 다양한 작업에서 고도화된 성능을 발휘하는 범용 AI 시스템

**[핵심/키워드]**

&lt;프론티어 AI 역량&gt;  
 - 창발성, 활용성(다양한 활용 가능), 접근성(저렴한 API 비용)

&lt;프론티어 AI의 위험성&gt;  
 - 악용 가능성, 예측 불가능성, 환각/탈옥, 프라이버시 침해, 경제 불평등 야기

&lt;프론티어 AI 규제 방안&gt;  
 - 윤리적 교육 및 인식제고, 안전성 검증, 책임 강화, 데이터 투명성, 사용제한  
 - 악의적 사용 금지, 지속적 관리, 글로벌한 거버넌스 및 체계

&lt;동향&gt;  
 - 국내 국가 주도의 프론티어 AI 개발 논의 중  
 - AI 보안 사고에 대한 프론티어 AI 규제 증가

## [생성형AI] 프론티어 페이싱 (Frontier Pacing)



**[정의]**

프론티어 AI의 성능 향상 속도를 의도적으로 조절하여, 정렬(Alignment)/해석가능성(Interpretability)/안전성 평가/보안 통제가 모델 능력 향상을 따라갈 수 있도록 시간을 확보하는 AI 안전 거버넌스 접근법

**[핵심/키워드]**

&lt;프론티어 페이싱 필요성&gt;  
 - Recursive Self-Improvement(RS)/Agent 고도화로 Frontier AI의 성능 발전 속도 급가속  
 - 자율행동/사이버공격/통제 실패 등 고위험 AI 위험 증가  
 - Capability 발전 대비 Alignment/Interoretability Safety 기술 격차 확대  
 - 기업 간 경쟁 심화로 충분한 안전검증 시간 확보 필요

<다리오 아모데이 프론티어 페이싱 3단계 거버넌스〉
 1단계 : 상주 평가자(Embedded Evaluators)  
  - 기업 내부 상주형 제3자 평가자,  안전기준 준수/사고/학습 프로세스 독립 검증  
 2단계 : 민주주의 진영 공조(Democratic Coordination)  
  - 기업 간 공동 안전기준/개발속도 기준, 정부의 제도적 지원, 공조 체계  
 3단계 : 글로벌 공조(Global Coordination)  
  - Level 1 : 위험 용도 금지 (명백한 위험한 AI 사용 제한)  
  - Level 2 : 고위험 사전 평가  
  - Level 3 : RSI 속도 제한  
  - Level 4 : 개발 속도 제한/일시 중단(Pause)

## [생성형AI] 오픈소스 AI



**[정의]**

소프트웨어, 데이터, 사전 학습된 가중치/바이어스 등 모델 파라미터, 도구, 문서 등의 구성요소를 오픈소스 라이선스 하에 공개하여 누구나 사용, 연구, 수정, 재배포할 수 있도록 허용하는 AI시스템

**[핵심/키워드]**

* Open Source AI = Data Information + Code + Parameters  
<오픈소스A 조건 (4대 자유)>
 - 사용 (Use), 연구 (Study), 수정 (Modify), 공유 (Share)

&lt;오픈소스 필수 공개 항목&gt;  
 - 데이터정보 : 학습 데이터 관련 정보  
 - 코드 : 전체 소스코드  
 - 매개 변수 : 모델 가중치 및 설정

## [생성형AI] 오픈 웨이트(Open Weight)



**[정의]**

인공지능 Model의 학습이 완료된 가중치(Weights)와 파라미터(Parameter)를 공개하여 누구나 다운로드, 실행, 미세조정(Fine-tuning)할 수 있도록 한 공개 방식

**[핵심/키워드]**

* 파라미터 중심  
&lt;필요성&gt;  
 - 인공지능 기술 확산과 연구 협력 촉진, 기업, 기관의 자체 인공지능 구축 수요 증가  
 - 투명성과 주권(Sovereign AI) 확보 요구 확대

&lt;공개 대상&gt;  
 - 학습 완료된 모델 가중치(Weights), 학습 데이터(Dataset), Model 파라미터  
 - 추론(Inference)용 Model

&lt;비공개 대상&gt;  
 - 학습 코드(Training Code), 학습 과정 및 파이프라인, 데이터 전처리 과정

&lt;대표 모델&gt;  
 - Llama A|2|Z (Meta), Mistral  
 - Qwen, Kimi K2/K3, DeepSeek

&lt;장점&gt;  
 - 데이터 외부 전송 최소화, Model 커스터마이징 가능, 벤더 종속성 감소  
 - 인공지능 주권 확보, API 비용 절감

&lt;한계&gt;  
 - 학습 과정 재현 불가, 라이선스 제한 가능, GPU 등 자체 인프라 필요  
 - 보안 운영 책임 사용자 부담

## [생성형AI] AI Washing (워싱)



**[정의]**

AI 기술을 실제보다 과장하거나 존재하지 않는데도 적용된 것처럼 표시, 광고하는 행위

**[핵심/키워드]**

* 그린워싱에서 파생  
&lt;발생원인&gt;  
 - AI 열풍, 정보 비대칭, 투자 유치 경쟁, 규제 공백

&lt;유형&gt;  
 1) 허위표시형 : Al 미적용 제품에 'AI 탑재' 문구 사용  
 2) 과장표시형 : AI 일부 기능만 있으나 전체가 AI인 것처럼 광고  
 3) 모호표시형 : 'A 지원', '스마트 인공지능' 등 구체적 근거 없는 표현 사용

&lt;대응방안&gt;  
 - 법적 규제 근거 : 표시·광고의 공정화에 관한 법률, 전자상거래법, AI 기본법(안) 명확화  
 - 규제 기관 동향 : 공정거래위원회, 한국소비자원, 개인정보보호위원회  
 - 예방 가이드라인(예정) : 'AI 기능 표시 기준(안)' 명시  
 - 기업 대응 방향 : AI Inventory, Evidence, Disclosure, AI 사용 사실 표시  
 - 광고 실증 : AI 기능, 성능 근거 확보, 객관적 시험 / 평가  
 - 투명성 확보 : AI 사용 사실, 생성물 표시  
 - 내부 통제 : AI 거버넌스, Claim Review, 사전 검증, 검토 체계

## [생성형AI] AI 해킹 (AI Hacking)



**[정의]**

성능 저하, 정보 유출, 오작동 유도를 목적으로 인공지능 모델, 데이터, 서비스를 목표로 한 공격

**[핵심/키워드]**

&lt;공격목표&gt;  
 - 모델 무력화, 정보 유출

&lt;주요 공격 유형&gt;  
 - 데이터 포이즈닝(Data Poisoning), 모델 도용, 탈취, 추출(Model Theft/Stealing)  
 - 모델 인버전(Model Inversion), 프롬프트 인젝션(Prompt Injection)  
 - 적대적 예제(Adversarial Example), 운영환경 침해(Access Compromise)

&lt;주요 취약점&gt;  
 - 데이터 파이프라인 신뢰성 부족, 검증 및 모니터링 미흡, 권한 관리 취약

<공격 도구/기법>
 - API 정보 노출, 자동화 쿼리 및 스크립트 공격, 합성 데이터 생성기 활용, 적대적 패턴 최적화

&lt;법 윤리 이슈&gt;  
 - 개인정보/민감정보 유출, 설명가능성 및 책임성 부족. 라이선스 및 저작권 문제

&lt;대응방안&gt;  
 - 데이터 무결성 확보, 모델 안전성 강화 (적대적 학습, 차등 프라이버시), 최소 권한 원칙  
 - 실시간 데이터 dift(드리프트) 감지, 이상 입력 패턴 자동 알림, 거버넌스 검증 체계

## [생성형AI] AI 탈옥 (AI Jailbreak)



**[정의]**

생성형 인공지능에 설정된 안전 정책, 응답 제한, 금지 규칙을 우회해 원래 거부해야 할 답변을 유도하는 공격 방식

**[핵심/키워드]**

&lt;핵심원리&gt;  
 - 규칙 회피, 역할 변경, 우회 지시

&lt;주요 목적&gt;  
 - 금지 정보 생성, 유해 콘텐츠 출력, 악성 코드 작성 지원, 내부 지침 노출, 민감정보 유출

&lt;대표 탈옥 유형&gt;  
 - 역할극(Role-play) : AI에 다른 인격, 캐릭터 부여  
 - 가상 시나리오 : 허구적 소설, 가상 상황 맥락 부여해 실제 요청 위장  
 - 단계적 질문 : 일반 질문부터 점진적으로 민감 요청으로 유도  
 - 번역, 요약 우회 : 언어 변환, 요약으로 필터 우회 시도  
 - 정책 혼동 : 모델의 우선순위, 규칙 혼란 야기  
 - 긴 문맥 삽입 : 긴 문맥에 악성 의도 은닉, 위험 신호 은폐  
 - 간접 프롬프트 주입 : 외부 데이터 악성 지시를 AI가 실행하도록 유도

&lt;주요 대응 방안&gt;  
 - 입력 필터링, 출력 검증, 정책 기반 거부, 레드팀 테스트, 권한 분리  
 - 감사 로그, 인간 승인 절차(HITL)

## [생성형AI] 프레데터 봇 (Predator Bot)



**[정의]**

인공지능(AI)과 자동화 기술을 결합하여 특정 대상이나 데이터를 선별·추적·공격적으로 활용하는 고도화된 자동화 프로그램

**[핵심/키워드]**

* CAPTCHA, IP 차단 등 기존 방어 방식 무력화  
* 섀도 API, 미 관리 엔드 포인트 추가 공격면 형성, API 기반 공격  
&lt;특징&gt;  
 - 인공지능 + 자동화 기반 특정 대상 선별·추적·공격 수행  
 - 정상 사용자 행동 모방. 실시간 공격 방식 변경, 능동적·지능형 공격 수행

&lt;주요 공격 방식 및 활용사례&gt;  
 - 계정 탈취 → 사용자 계정 탈취 및 권한 악용  
 - 데이터 수집 → 개인정보 및 서비스 데이터 수집  
 - 허위 계정 생성 → 대량 계정 생성 및 악성 활동 수행  
 - 매크로 및 거래 조작 → 상품 선점 및 대규모 매크로 거래 조작  
 - 금융 서비스 및 게임 어뷰징 → 금융 및 서비스 타겟 공격

 &lt;주요 대응 방안&gt;  
 - 전체 API 가시성 확보 : API 식별 및 통합 모니터링 체계 구축  
 - 행위 기반 봇 탐지 : 이상 징후 실시간 분석, 자동화 탐지  
 - 패치 주기 단축 → 취약점 자동 패치 파이프라인 구축  
 - 다중인증(MFA) 강화→ 생체 인식 및 하드웨어 보안 키 도입  
 - 로그 관리 및 모니터링 강화→ SIEM 및 EDR/XDR  
 - AI 보안 대응 체계 전환 → 제로트러스트 아키텍처 및 Security by AI 구축

## [생성형AI] 프로젝트 글래스윙 (Project Glasswing)



**[정의]**

AI 기반 코드·바이너리 분석을 통해 취약점을 자동 탐지하고 공격 가능성까지 평가하는 보안 연구 프로젝트

AI 공격에 대응하기 위해, AI로 취약점을 선제 탐지·방어하는 글로벌 협력 보안 프로젝트

**[핵심/키워드]**

* 앤트로픽(Anthropic)에서 주도. 이 프로젝트의 핵심 AI 모델이 Claude Mythos  
&lt;추진 배경&gt;  
 - AI 공격 능력 진화, AI 악용 리스크 확대

&lt;핵심 기술&gt;  
 - Claude Mytos 기반 보안 AI, 취약점 자동 탐지, Expolit 생성 가능

&lt;목적&gt;  
 - 핵심 인프라 보안 강화, 보호, 선제적 보안 체계 구축

&lt;추진 방식&gt;  
 - 글로벌 협력 생태계 : AWS, Google, MS 등 빅테크 공동 참여

&lt;적용 대상&gt;  
 - 핵심 SW + 오픈소스 : 기업 시스템, 오픈소스 까지 전방위 보안 점검

&lt;특징&gt;  
 - AI 기반 보안 자동화, AI vs AI 보안 구조, 보안 속도 경쟁, 보안 패러다임 전환

## [생성형AI] AI 레드팀 (AI RedTeam)



**[정의]**

인공지능 시스템(특히 LLM,생성형 AI 등)에 대해 의도적 공격·취약성 검증을 수행하는 전문팀

**[핵심/키워드]**

* AI 레드팀, AI 블루팀, AI 퍼플팀  
&lt;특징&gt;  
 - 공격자 시뮬레이션, 사전 대응 및 개선, 다양한 공격기법 활용, 데이터 보안 및 신뢰도 평가

&lt;주요역할&gt;  
 - 취약점 탐색, 윤리적 문제 및 편향성 검증, 신뢰성 및 안정성 강화

&lt;실행단계&gt;  
 1. 목표 정의 > 2. 공격벡터 선정 > 3. 테스트 세트 구축  > 4. 테스트 실행 > 5. 재검증

&lt;테스트 시나리오 방식&gt;  
 - 공격자 관점, 적대적 테스트, AI 시뮬레이션, 지속 개선

&lt;산출물&gt;  
 - Attack Scenario, Finding Report, Risk Score,  
 - Mitigation Plan, Regression Test

## [생성형AI] KISA「AI보안 위협 대응 매뉴얼」



**[정의]**

한국인터넷진흥원(KISA)과 과학기술정보통신부가 인공지능 시스템 확산에 따른 보안 위협과 실무 대응 방안을 담은 국내 첫 정부 차원의 가이드

**[핵심/키워드]**

1) 내재적 위협(Intrinsic Threat)  
  - AI 자체의 한계나 고유 특성에서 비롯되는 위협, 외부 공격자 없어도 발생 가능  
  - 학습 데이터 편향, 환각, 정렬 실패, 확률적 비결정성  
 2) 외재적 위협(Extrinsic Threat)  
  - AI를 도구로 활용하는 외부행위자에 의해 발생하는 위협, 외부 위협 행위자의 의도적 행위  
  - 탈옥, 모델 추출, 공급망 인프라 공격, 고성능 모델 위협

 1) 데이터 위협 : 불균형 데이터, 부정확 데이터, 개인정보 비식별화 미흡  
 2) 모델 위협 : 학습 데이터 유출, 환각, 탈옥, 부적절한 출력처리, 모델 DoS  
 3) 에이전트 위협 : 부적절한 도구 설계,에이전트 하이재킹, 에이전트 DoS, 메모리 오염  
 4) 공급망 위협 : 데이터 포이즈닝, 모델 포이즈닝, 취약 버전의 추론 엔진 및 에이전트  
 5) 고성능 모델 위협 : 고도화된 사이버 공격 지원 위협, 통제 상실 위협

 1) 데이터 계층 : 데이터 품질 관리, 개인정보 보호 및 법규 준수, 개인정보 감사 로깅  
 2) 모델 계층 : 모델 정렬, 가드레일 도입, 안전한 모델 API 설계,  
 3) LLM 애플리케이션 계층 : 시스템 프롬프트 강화, 모델 출력 보안 처리  
 4) 에이전트 계층 : 최소 권한, 위험기반 접근제어, Human-in-the-Loop, 에이전트 가드레일, 에이전트 레드팀  
 5) 공급망 계층 : 백도어 및 데이터 오염 탐지, 외부 구성요소 출처 및 무결성 검증, 자산 목록화 및 정기적 보안 업데이트

## [생성형AI] KISA「AI 보안 레드티밍 가이드」



**[정의]**

AI 시스템의 보안 허점을 선제적으로 진단하고 대응하기 위한 실무 운영 지침서

&lt;레드티밍&gt;  
 - AI 시스템을 분석해 취약점 식별·보안 대책 제시 수행하는 활동

* 대상별 위협  
 - AI 보안 위협 대응 매뉴얼의 위협과 동일 항목

**[핵심/키워드]**

* AI 시스템 대상, 조직 목표에 따라 선정  
&lt;계층별 테스트 대상&gt;  
 1) 데이터 계층 (학습/평가 데이터,  데이터 파이프라인, 입출력 데이터)  
 2) 모델 계층 (AI 모델, 파인튜닝, 도메인특화모델)  
 3) 애플리케이션/인터페이스 (에이전트 확장요소, 사용자 인터페이스, 가드레일)  
 4) 인프라 계층 (서버, 컨테이너, CI/CD 파이프라인, 접근제어, 권한 관리)

&lt;레드티밍 방법론&gt;  
 - 위험도·보안요구사항·수행역량·가용자원·내부정보 접근수준 고려  
 - 수행방식 (자체 수행, 외부 전문기관 활용)  
 - 점검 관점 활동 (적대적 레드티밍, 선량한 레드티밍)  
 - 접근 수준 분류 (블랙박스, 화이트박스, 그레이박스)

&lt;레드티밍 인력 구성&gt;  
 - 리더·PM, AI 레드팀 전문가,  보안 테스트 전문가, AI 엔지니어, AI 법률 자문가, 도메인 전문가

 1단계 : 준비 과정 (사전 협의·교전 규칙, 목표·범위, 평가기준, 공격표면 및 위협 시나리오)  
 2단계 : 이행 과정 (공격 수행, 영향 분석, 근본 원인 분석, 기록 관리)  
 3단계 : 결과 보고 과정 (결과 보고서, 개선 계획, 후속 조치, 지속적 개선)

## [생성형AI] MITRE ATLAS (Adversarial Threat Landscape for AI Systems)



**[정의]**

Al/ML 시스템을 대상으로 실제 공격 사례를 기반으로 공격자의 TTP(Tactics, Techniques, Procedures)를 체계화한 AI 보안 위협 지식베이스

**[핵심/키워드]**

* MITRE ATT&CK 구조를 AI영역으로 확장  
&lt;전술 및 대표 기법&gt;  
 1) 정찰(Reconnaissance) : 공개 기술 DB 검색, 능동 스캐닝, RAG 인덱싱 대상 수집  
 2) 자원 개발(Resource Development) : 공개 AI 아티팩트 확보, LLM 프롬프트 제작, 오염된 AI 아티팩트 배포  
 3) 초기 접근(Initial Access) : AI 공급 침해, 피싱, 공개 애플리케이션을 통한 프롬프트 침투  
 4) AI 모델 접근(Al Model Access) : Al 모델 추론 API 접근, 전체 Al 모델 접근, AI 기반 제품 서비스 접근  
 5) 실행(Execution) : LLM 프롬프트 인젝션, AI 에이전트 도구 호출, AI 에이전트 배포  
 6) 지속성 유지(Persistence) : 학습 데이터 중독, RAG 중독, AI 에이전트 컨텍스트 중독  
 7) 권한 상승(Privilege Escalation) : LLM 탈옥, Al 에이전트 도구 호출, 호스트 탈출  
 8) 방어 회피(Defense Evasion) : AI 모델 회피, LLM 탈옥, LLM 프롬프트 난독화  
 9) 자격 증명 접근(Credential Access) : RAG 자격증명 수집, AI 에이전트 설정정보 자격증명 수집, AI 에이전트 도구 자격증명  
 10) 탐색(Discovery) : Al 아티팩트 탐색, LLM 시스템 정보 탐색, AI 에이전트 설정 탐색  
 11) 내부 이동(Lateral Movement) : 피싱, AI 에이전트 도구 호출, 대체 인증정보 사용  
 12) 수집(Collection) : AI 아티팩트 수집, AI 서비스 데이터 수집, 정보 저장소 데이터 수집  
 13) Al 공격 준비(AI Attack Staging) : 프록시 AI 모델 생성, 적대적 데이터 생성, AI 모델 조작  
 14) 명령 및 제어(Command and Control) : 리버스 셀, AI 서비스 API 악용, AI 에이전트 활용  
 15) 유출(Exfiltration) : AI 추론 API를 통한 유출, LLM 데이터 유출, AI 에이전트 도구 호출을 통한 유출  
 16) 영향/피해(Impact) : AI 서비스 거부, AI 모델 무결성 훼손, 비용 유발 공격, 시스템 침해

