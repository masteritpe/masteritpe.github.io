---
layout: post
title: "303.Big&Up3(Union Survival)_COM"
date: 2026-07-16
categories: 키노트
tags: [키노트]
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

### 데이터 차원축소(Data Dimensionality Reduction)

**[리드]**  

차원의 저주 해결, 데이터 차원축소  

**[개념]**  

고차원 데이터를 저차원으로 변환하여 데이터의 중요한 정보를 유지하면서 연산 비용을 줄이는 기법  
-인공지능 차원축소 활용 : 데이터 시각화, 노이즈 제거, 모델 성능 향상, 과적합 방지, 차원의 저주 해결 등  
→ 차원 축소를 통해 인공지능 모델이 더 효율적이고 해석 가능하도록 개선  

**[상세설명 및 해결방안]**  

데이터 차원축소 알고리즘 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfMzkg/MDAxNzQzMTcwODcyNzUy.uTPcd3YwGtmGcGzzyiEbabg0wAYU0-PxBhBr-ig_dqwg.8p8_2weMeJvERlbxDnLgCDFBBMY0HvdTHpibIO60M5og.PNG/001.png?type=w1600)  

- 데이터의 선형/비선형 구조를 보존하며 저차원 공간으로 변환  

- 차원 축소 적용시 의미를 축소하여 발생하는 해석력 저하에 대한 지속적 확인 필요  

데이터 차원 축소 적용 시 정보손실가능성에 대한 최소화 기법 설명  

정보 손실 가능성  

ㄴ누적 분산 비율 확인 (PCA)  

ㄴ차원 축소 전후 모델 성능 비교  

해석력 저하  

ㄴ주성분과 원본 변수 관계 분석  

ㄴ t-SNE, UMAP 등 시각화 활용  

적절한 차원 수 선택  

ㄴ엘보우 기법 및 설명된 분산 분석  

ㄴ교차 검증을 통한 최적 차원 탐색  

비선형 데이터 대응  

ㄴt-SNE, UMAP, Isomap 등 비선형 기법 적용  

ㄴAutoencoder, VAE 등 딥러닝 기법 활용  

### 모집단의 특성을 추론하는 점추정과 구간추정 비교

**[리드]**  

표본 통계량을 이용하 모수의 확률적 추론, 점추정과 구간추정  

**[개념]**  

점추정 : 모수에서 추출된 표본으로 부터 모집단의 모수를 하나의 값(점)으로 추정하는 통계적 방법  

구간추정 : 모수에서 추출된 표본으로 부터 모집단의 모수를 일정한 신뢰구간 내에서 추정하는 통계적 방법  

--&gt; 점추정은 간결하지만 불확실성을 반영하지 못하며, 구간추정은 신뢰도를 포함해 보다 안정적인 추론이 가능함  

**[상세설명 및 해결방안]**  

점추정과 구간추정의 정의 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfMjA4/MDAxNzQzMTcxMzA0MzM5.rwV7yEIfK_5CYcBi3RUUfMwClzeUddzYholLv547yokg.1ioLnAKtdG4yRVpHc_YaGMu45UwHW2r0LhQ0z2euMgsg.PNG/002.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfODIg/MDAxNzQzMTcxMzQ1NDIx.OZSISm0H9i9U6RURPrF7Fe9UcC8UVDpNtSC7PJbf3wkg.dIMVzAk40AduhxV6GxtgpBSiWS6N4S8_GgWTLk7LBSsg.PNG/003.png?type=w1600)  

### 요구사항명세서에 기술되어야 하는 항목 설명

**[리드]**  

요구사항의 완전한 구체화, 요구사항 명세서  

**[개념]**  

프로젝트의 목표, 기능, 성능, 제약 조건 등 소프트웨어가 충족해야 할 요구사항을 체계적으로 정리한 문서  

- 중요성 : 명확한 소통, 범위 관리, 리스크 감소, 테스트 기준 제공, 제안요청서의 명확화 공공SW사업 선진화 등  

-&gt;국내 공공, 정부 소프트웨어 프로젝트는 소프트웨어진흥법 제44조(소프트웨어사업의 과업범위)에 의거 작성을 필수로 함  

**[상세설명 및 해결방안]**  

요구사항명세서에 기술 해야하는 내용 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfNDgg/MDAxNzQzMTcxNDMyMjE1.gm6MJDDybHWMekHZU7WGs7gmNfh8NpEFofXKTW8VenMg.h_Ww2C9yLMXZlSYdlBIzBPst2_O7QnN7CTQPKPm8A7og.PNG/004.png?type=w1600)  

--&gt; 작성 원칙 : 명확성, 완전성, 검증가능성, 일관성, 수정 용이성, 추적 가능성, 개발 후 이용성  

요구사항의 진행 추적, 요구사항 추적표 추가 설명  

- 프로젝트의 요구사항이 프로젝트 진행 과정(설계, 개발, 테스트 단계)에서 일관되게 반영되고 충족되고 있는지를 추적하고 관리하기 위한 문서  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfMjYg/MDAxNzQzMTcxNTEzNTg2.8nC0RVwxVROh6DiFbzGfZuijKZKR_nvEyqGJR3CLu3wg.84su4rFafGd6m8qAYMNQvIO7HZqvYy014I-e_1tw4DUg.PNG/005.png?type=w1600)  

### 데이터옵스(DataOps)의 주요 기술을 설명하고, 데브옵스(DevOps)와의 차이점을 설명하시오

**[리드]**  

데이터파이프라인 최적화, 데이터옵스  

**[개념]**  

인공지능 학습용 데이터 품질관리 가이드라인  

**[상세설명 및 해결방안]**  

데이터파이프라인 최적화, 데이터옵스의 주요 기술  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfMjQ5/MDAxNzQzMTcxNjI1NDUx.oZqZrQxWt0SX7bigKPPu0KAdX2XGCymuHJo25xyp9REg.mG6XL0Yq0D8YVkbXBLJqKenlM2InmMdTnDSdOHc_D-Ug.PNG/006.png?type=w1600)  

-&gt; 머신러닝 및 AI 모델을 위한 고품질 데이터 제공이 목표, ModelOps 및 MLOps의 기반이 되는 데이터 운영 방식  

데이터옵스와 데브옵스와의 차이점 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfMjQg/MDAxNzQzMTcxNzIwNjQx.Udnq6IC-xzLKmIrzhZUFf1MIePtmaQXR5NtvmvMpgdUg.CN_5AThcSq2WwEaWUDLoqAoAp392PYqVgkPXCxviAc4g.PNG/007.png?type=w1600)  

-&gt; 데이터옵스는 데이터 처리와 품질 관리에 초점을 두고, 데브옵스는 소프트웨어 개발과 배포 자동화에 집중  

AI 시대 생산성 향상을 위한 AI관련 Ops 방식의 이해  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTAzMjhfOTQg/MDAxNzQzMTcxNzY4NjA2.TKzQNLBhJiA7gHAf4k7gZ5wxHG7uTSbkqj_k25Tw3Ywg.YGVgQXMyDnf80L1SaqOtJIh8DkEQDzc2FNAI-3RdA2cg.PNG/008.png?type=w1600)  

### 중심극한정리, t-검정, z-검정 설명

**[리드]**  

모집단의 특성 추론, 통계적 가설검정시 평균차이검정  

**[개념]**  

표본(Sample) 데이터를 분석하여 서로 다른 두 개 이상의 모집단(Population) 간에 평균의 차이 존재 여부를 통계적으로 검증하는 가설검정 방법  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTI2/MDAxNzQzNjA0Mjk3NDU4.HjJrPF4MGMLUJJJW4GzELi_Ftj6KTw3QuN3epDpH-mgg.vSS2s0q39VJF6shv9KhEPYMS1ktHkRJaAMew5a_PB8Ag.PNG/009.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfODYg/MDAxNzQzNjA0MzYxOTY0.8Eyzl-1dByjS6Jd1-hKnHkOEXFIgKlZzp7F4VqMmM5og.cNurarWqaRlazEjSneZ-96eOIhw4PG5d5ITU_KNRCd4g.PNG/010.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfNDQg/MDAxNzQzNjA0Mzk5NTM1.unDMVZbHhSZ4EF50vJAN1lQYlTHc-gm-58v9YESOuWcg.DCI0PYkix7reqf1pVCpPkx2SyoE-3arI1cskjk6gdlUg.PNG/011.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfODUg/MDAxNzQzNjA0NDM3NjE1.OZNwFAKWNU9Rk9R3e-9Hn2ZbNTI8a9y6kqH-HHyXI58g.JaNg_EKlojtfFes12snCBt26Oi_sKHIQLsE4_e14HYwg.PNG/012.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTgy/MDAxNzQzNjA0NDc5ODM2.jGP1T0oTF9RT4bn36deTueS6nrHxG8z0zb0fhHoMOFQg.I_hGGxJbs1eKIfutxAp0Wwpi1_ydnOJ3IwsmpJaQ4HUg.PNG/013.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTI0/MDAxNzQzNjA0NTQxNzA2.eSBrXAS5NOYHFWwkhStBuCKu3Ux647G1XzEqwnWEV10g.GZtRfJvnJYNZj1idKIGuZr8OuoW_nLnf7Kg0puzGsM0g.PNG/014.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfOTAg/MDAxNzQzNjA0NTgxNDU0.RU_FEF70ED-VFQvPx4KHhBjmZasOb5dtclSQp3NMdC0g.JLfEQkrs_N5Q4LQ09M74X5rNQvkKF84RMvs65gOfCKYg.PNG/015.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTc2/MDAxNzQzNjA0NjE5OTk5.EWJycs3Sn62NOhldYr8CYSQFS9kSoVRc_NqLGey0n6og.OI2fpsKlRiP9qzBaK6w1Ix2aVH-4oRCVQ823rfATMiMg.PNG/016.png?type=w1600)  

### 강화학습(Reinforcement Learning)은 최적의 행동정책을 찾아가는 기계학습 방법가. 가치기반 강화학습, 정책기반 강화학습, 액터 크리틱(Actor-Critic) 강화학습나. 정책경사(Policy Gradient) 방식 강화학습

**[리드]**  

가장 큰 보상을 얻기 위해 정책(Policy)의 스스로 학습, 강화학습  

**[개념]**  

데이터의 상태(State)을 인식하고 이에 반응한 행동(Action)에 대하여 환경으로부터 받는 포상(Reward)을 학습하여 행위에 대한 포상을 최적화하는 정책(Model)을 찾는 기계학습  

**[상세설명 및 해결방안]**  

가장 큰 보상을 얻기 위해 정책(Policy)의 스스로 학습, 강화학습의 개요  

- 강화학습 : 데이터의 상태(State)을 인식하고 이에 반응한 행동(Action)에 대하여 환경으로부터 받는 포상(Reward)을 학습하여 행위에 대한 포상을 최적화하는 정책(Model)을 찾는 기계학습  

- 학습 요소 : 에이전트, 환경, 상태, 행동, 보상, 정책, 가치 함수  

- 학습 매커니즘 : 에이전트가 환경과 상호작용하며, 상태(State)에 따라 행동을 선택하고, 그에 대한 보상을 최대화하는 정책을 학습  

- 강화학습의 분류 :  

ㄴ Model-Free (모델 없이 학습) : 정책기반(PPO), 가치기반(Q-Learning)  

ㄴ Model-Based(모델 기반 학습) : Learn the model(Dyna-Q), Given the Model(MCTS 기반)  

ㄴ Model-Free + Model-Based (혼합형): 액터 크리틱(Actor-Critic)  

-&gt; Agent 와 환경과의 상호 작용을 통해서 행동을 결정  

-&gt; 명시적인 정답이 없는 환경에서 경험을 바탕으로 최적의 정책을 스스로 학습한다는 점에서 큰 의의를 가짐  

가치기반 강화학습, 정책기반 강화학습, 액터 크리틱(Actor-Critic) 강화학습  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTI5/MDAxNzQzNjA0ODIwODUz.GVZcJB0S3eXMdhgFXzD6ou4MU3qA6grWJ1VVN9w1ORMg.oMafKc3blraNXpJi-Rf6cOoQO8XaPXJzDfHgOyA0hNQg.PNG/001.png?type=w1600)  

-&gt; 실제로 Critic이 Value Function을 학습하여 정책 최적화를 돕기 때문에 혼합형(Actor-Critic)으로 분류됨  

정책의 직접 최적화, 정책경사(Policy Gradient) 방식 강화학습 설명  

가. 정책경사(Policy Gradient) 방식의 개념과 특징  

- 개념 : 에이전트가 상태(State)에서 행동(Action)을 선택하는 확률을 학습하여 최적의 정책을 찾아가는 방식  

&lt;특징&gt;  

- 상태 S에서 행동 A를 선택하는 확률을 직접 학습  

- 확률적 정책(Stochastic Policy) : 행동 선택을 확률적으로 수행하여 탐색  

- 현재 실행 중인 정책(Policy)을 그대로 학습  

- Q-Learning과 달리 연속적인 행동(Continuous Action Space)에서도 사용  

--&gt; 보상을 최대화하는 방향으로 정책을 업데이트  

나. 정책경사 방식의 학습 매커니즘 및 주요 알고리즘 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTU1/MDAxNzQzNjA0ODU3MTA4.Dzkc7I7uYS-jmBVyMwuJKDEYWvZEEF2A_0xZDbMuaO0g.ajoKskjIZzqvZoviTJ2odSlf3l9Lx70onYl1EXfSBWAg.PNG/002.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTUz/MDAxNzQzNjA0OTAxMDc4.ghK8QPYBVtF7m8lWV1my1ij3FqflVt_zQXRhSOXMKwIg.aL0uNSUEtGfAHoWE091vpocLkRfp-fQdjT6jV9NTy34g.PNG/003.png?type=w1600)  

-&gt; 로봇 제어 분야의 산업용 로봇, 자율주행 로봇, 휴머노이드 로봇의 최적 행동 학습  

강화학습 각 모델 특성 별 활용 분야 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfNjUg/MDAxNzQzNjA0OTM3NDc5.Fv4E1FacNcr7juAlfEXvXqn-hISHC8HFj61E_MxKuLIg._sJBHYehsKtvh1rUIcyDMAUF1iQgJQAqI6sfVgdzORgg.PNG/004.png?type=w1600)  

### 고장허용(Fault Tolerant) 시스템과 고가용성(High Availability) 시스템가. 고장허용(Fault Tolerant)과 고가용성(High Availability) 시스템의 개념나. 하드웨어, 소프트웨어, 데이터 측면에서 고장허용(Fault Tolerant) 기법다. 고가용성(High Availability) 시스템의 구성 방법라. 고장허용(Fault Tolerant) 시스템과 고가용성(High Availability) 시스템의 비교

**[리드]**  

회복 탄력성(Resilience), 고장허용(Fault Tolerant) 시스템과 고가용성(High Availability) 시스템  

**[개념]**  

고장허용 시스템 : 시스템에 장애(고장)가 발생해도 지속적으로 운영될 수 있도록 설계된 시스템  

- 특징 : 무중단 운영, 이중화(Redundancy) 적용, 자동 장애 감지 및 복구, 비용 증가  

고가용성 시스템 : 시스템의 운영 중단 시간을 최소화하여 지속적인 서비스 제공을 목표로 하는 시스템  

- 특징 : 서비스 연속성 보장(Fail Over), 이중화 기반 설계, 다양한 구성 방식 지원, 부하 분산 및 자동 복구  

**[상세설명 및 해결방안]**  

고장허용과 고가용성 시스템의 개념, 하드웨어, 소프트웨어, 데이터 측면에서 고장허용(Fault Tolerant) 기법  

가. 고장허용과 고가용성 시스템의 개념  

&lt;고장허용 시스템&gt;  

- 개념 : 시스템에 장애(고장)가 발생해도 지속적으로 운영될 수 있도록 설계된 시스템  

- 특징 : 무중단 운영, 이중화(Redundancy) 적용, 자동 장애 감지 및 복구, 비용 증가  

&lt;고가용성 시스템&gt;  

- 개념 : 시스템의 운영 중단 시간을 최소화하여 지속적인 서비스 제공을 목표로 하는 시스템  

- 특징 : 서비스 연속성 보장(Fail Over), 이중화 기반 설계, 다양한 구성 방식 지원, 부하 분산 및 자동 복구  

-&gt; 고장허용 시스템 은 장애 발생 시에도 운영을 지속,  

-&gt; 고가용성 시스템은 장애 발생 후 빠르게 복구하여 서비스 중단 시간을 최소화하는 방식  

나. 하드웨어, 소프트웨어, 데이터 측면에서 고장허용(Fault Tolerant) 기법 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTcx/MDAxNzQzNjA1MDU1NTYx.ZOOcywJOJWkaN1i1TOZdnciHN8ei5gE2kdUj_MmoHbgg.YIvx5HSKHy0tEekNSFdvMY-LY7NRbp0WgqrokDx7dXkg.PNG/005.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfNDgg/MDAxNzQzNjA1MDYyOTA1.8O6IicJsCNtCrs_mNw366Nwm50cJf41KelCFUwMjLSMg.HKm-2doypWRzpRIQvjNRCEERAmChRn_PIsqbEw4c2FQg.PNG/006.png?type=w1600)  

--&gt; 고장허용은 비용이 높지만 신뢰성이 중요할 때 사용, 고가용성은 비용 대비 효율적인 방법으로 활용됨 따라서 기업 환경에 따라 두 시스템을 조합하여 사용 필요  

고가용성(High Availability) 시스템의 구성 방법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTkw/MDAxNzQzNjA1MTgyMDY1.kso5FUdEYeqO1qLKdJdjPLtcC7-URYe_pjDLnzfWm5Ug.qQgk_h15YLS_X7jWkhoGt7gjJv3U5GWYV1aRcGfqkA0g.PNG/007.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMjU3/MDAxNzQzNjA1MTgyMjY1.UGbQFtvBw5oWBUuzmi5OC9KbE6J0jVgzQTrrz4q38WYg.vNLfV7M7TqnLAEstsHvu_Xjhj0Kt5z9-2hPyQRvL0GQg.PNG/008.png?type=w1600)  

-&gt; 고가용성 시스템은 필요에 따라 구성 방식이 다르며, 서비스 연속성과 성능 요구에 맞춰 적절한 방식을 선택  

고장허용(Fault Tolerant) 시스템과 고가용성(High Availability) 시스템의 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMjY1/MDAxNzQzNjA1MjE5Njgw.LjJ5nUc5TxA_EfOZb_DQkc9PIbgZoKXr7JUSn0QTK7cg.uVX1-9m_87oVH6l-6GRKDBJxFWz9uXnGHcg022gysekg.PNG/009.png?type=w1600)  

-&gt; FT는 중요한 미션 크리티컬 시스템에서 사용되며, 일반적인 IT 서비스에는 HA가 더 적합함.  

Enterprise 측면의 비용효과 최적화를 위한 시스템 고가용성과 고장허용 선택 기준 제시  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMzEg/MDAxNzQzNjA1MjYyODYz.44y3mKY26VNvxW_MPQybj7YvftA3lAE2Uv5j9Q5Ltpsg.2xh2R7MrAjw5T9O_vK9mr3e2jNypoeb8St-4nmlww_Ug.PNG/010.png?type=w1600)  

--&gt; FT는 완전 무중단이 필수인 경우 선택, HA는 경제성과 효율성을 고려한 서비스에서 활용  

### 플랫폼 엔지니어링(Platform Engineering)

**[리드]**  

조직의 셀프서비스 개발 플랫폼, 플랫폼 엔지니어링  

**[개념]**  

개발자의 생산성을 향상시키기 위해 내부 개발 플랫폼(IDP)을 구축하고 유지 관리하는 소프트웨어 엔지니어링 분야  

- 특징 : 1) 개발자 경험(DX) 향상 2) 자동화 및 표준화 3) 보안 및 규정 준수 강화 4) 비용 효율성 증대  

-&gt; 클라우드 컴퓨팅, 빅데이터, 인공지능 등의 새로운 기술도입 확대로 플랫폼 엔지니어링이 기업의 디지털 이니셔티브로 자리잡고 있음  

**[상세설명 및 해결방안]**  

플랫폼 엔지니어링의 아키텍처 및 기술요소  

가. 플랫폼 엔지니어링의 아키텍처  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMjM2/MDAxNzQzNjA1NDEyNDE3.3m-QZ5qc4lGytGn6TTihJh5gGBz-o7kjCzCZiEhmpxQg.aZd8c-usMlvFlqMYgHPN67eg9KLVeWc830B-jn0TJ4wg.PNG/011.png?type=w1600)  

-&gt; 생산성 향상 및 효율적 운영을 위해 셀프서비스 가능한 내부 개발 포털(IDP, Internal Developer Portal)과 플랫폼 설계/제품화 전담조직(플랫폼 엔지니어링 팀)운영 역할이 필수적임  

나. 플랫폼 엔지니어링의 기술요소  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfNzEg/MDAxNzQzNjA1NDQ3MjQ3.LI_j8JuIlzudp7kzCXD958hYFZlV88OmEJCLneJMPMkg.Ln-bQwLukTLgTNkcTsoRGYwI2uREElHdpu3tbtv4qPEg.PNG/012.png?type=w1600)  

-&gt; DevOps로 인한 어플리케이션 개발과 운영의 통합에 관심이 높아지면서 플랫폼 엔지니어링은 DevOps의 최종진화 관점으로 주목 중임  

플랫폼 엔지니어링과 데브옵스 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfODgg/MDAxNzQzNjA1NDg2NzIy.gEXsEyMuARHOijiORnys5ryHQLtXGcqX4p8rlLxoxLcg.g6xvdlaGxMj9YjmYlNMV1Q-dIpTCBeBdM99OD6xiKlwg.PNG/013.png?type=w1600)  

-&gt; 플랫폼 엔지니어링을 통해 개발 표준화, 자동화도 지속적인 관심 확대 필요  

### 정보시스템마스터플랜(ISMP)의 기본 구성 내용(단계별 활동, 세부내용, 산출물)

**[리드]**  

기업/기관 정보화 시스템의 체계적 구현, ISMP  

**[개념]**  

특정 SW 개발 사업 상세분석과 RFP 마련을 위해, 기능점수 도출이 가능한 수준까지 기능적/비기능적 요건을 상세히 기술하며, 구축 전략 및 이행계획을 수립하는 활동  

(특징)  

1) 발주기관의 불명확한 요구사항, 잦은 과업변경에 따른 문제점 해소  

2) 객관적인 데이터와 기준을 근거로 사업규모와 일정 수립에 어려움 극복  

-&gt; 2022년 개정된 ISP/ISMP 수립 공통 가이드 제6판으로 ISMP 제도화의 기반이 마련되었으며, 2024.12월에 발표된 제8판에는 클라우드 네이티브 도입여부 검토 및 UI/UX 구성방안 제시 등이 추가됨  

**[상세설명 및 해결방안]**  

정보시스템마스터플랜의 기본 구성내용 단계별활동 세부내용 산출물) 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMjQ3/MDAxNzQzNjA1NjA5OTc1.8IozlDIYVNZG5uR_RTiG8ptR4PCbRzeKI9bIsnxwALkg.N17UCY4Yzi7spkqhB-jTwt19td9PpfI0gnwIdNePGHwg.PNG/014.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTE2/MDAxNzQzNjA1NjEwMDQx.H7MsoGy0JBxaIpy1KjigFIaGw6pt_HpoTtOt6pOsjXEg.JvoZwsJjuUy1PrD5GHa1U379_PjIbVAntAnECmce3IEg.PNG/016.png?type=w1600)  

-&gt; 정보시스템마스터플랜 수립을 통해 조직의 비즈니스 목표와 정보시스템 전략의 결합이 가능하며, 혁신적 기술도입과 운영성과 측정, 프로세스 개선으로 경쟁우위 확보 기대  

### 정보 시스템 감리와 PMO(Project Management Office) 비교

**[리드]**  

프로젝트의 성공 지원, 정보시스템 감리와 PMO  

**[개념]**  

감리 : 감리대상사업 현장에 상주하거나 주기적으로 투입되는 감리원  

PMO : 프로젝트와 관련된 자료, 방법론, 기술, 기법을 관리/공유하고 전사 프로젝트, 프로그램, 포트폴리오 관리를 통해 조직의 전략적인 목표를 달성하기 위한 프로젝트 관리 전담 조직  

**[상세설명 및 해결방안]**  

프로젝트의 성공 지원, 정보시스템 감리와 PMO의 개념 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfNTEg/MDAxNzQzNjA1NzExODU3.HUMvglJ1MgiYK1y2_-xn2vEyb5Cp0fus17YovuVnKa4g.phDc0TdO4Mb1_yOcFDZL5yLtFg2ABKZtH5MVibhdURwg.PNG/017.png?type=w1600)  

-&gt; 프로젝트성공 및 품질유지를 위해 감리 및 PMO 조직 필요  

정보시스템 감리와 PMO의 상세 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTEy/MDAxNzQzNjA1ODIyNTgw.dKUKvq7dWNxEPBnulB4D59VnwC_uLHjQX1NjQzgyd9Ag.hIKu0xxnrnJwryW9wrRhMDUD-pnCoI9m2JcdtfMhansg.PNG/018.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMjEx/MDAxNzQzNjA1ODIyNTg4.QT3H2iHbj7KQVV5RC0e1LW_IlYrEoBv2MsOoR4w53c4g.39C_0uYykXRM0z6LeRqESojuk1ySYpez7qOzkqoQDNQg.PNG/019.png?type=w1600)  

-&gt; PMO는 권고 사항 감리는 의무적용으로 감리절차에 따라 수행 필요  

정보시스템 감리 절차 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDJfMTYg/MDAxNzQzNjA1ODkzNDgx.gEk0dNHy364s24-RGxfql5jn2zfB8tpiunmEuPmOGyog.WTHotYArCwbzCK46S1jnwNFbSou0ijsSB_ahGQddeskg.PNG/020.png?type=w1600)  

-&gt; 프로젝트 성공 위해 감리와 PMO 협력관계로, 시정조치 확인완료까지 수행  

### 파인튜닝(Fine-tuning)

**[리드]**  

맞춤형 AI모델 생성, 파인튜닝  

**[개념]**  

전이학습의 일종으로, 기존 모델의 일부 또는 전체 가중치를 조정하여 새로운 데이터셋에 맞게 추가학습 하는 방법(기존 모델을 추가 학습하여 특정 데이터 셋에 최적화)  

(특징)  

1) 사전 학습 모델 활용, 2) 도메인 특화 최적화, 3) 빠른 학습 속도, 4) 일반화 성능 보존, 5) 고성능 GPU 필요  

-&gt; ChatGPT, BERT등 LLM 챗봇은 범용모델로, 기술, 금융 등 특정 도메인에 대한 워크플로우 대체를 위해 파인튜닝 기술이 필요  

**[상세설명 및 해결방안]**  

파인튜닝의 단계별 수행절차 및 세부기법 설명  

가. 파인튜닝의 단계별 수행절차  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMjEy/MDAxNzQzNjA2MDI3NDc3.tWppf1oK1R6PJ5mJmArvreZnO73CXFntYLK0gLS-Nkgg.2f5O28HqLPXffn0UR5N1FhATrsN2Y9VxjfFL84QBNnwg.PNG/021.png?type=w1600)  

-&gt; 대형모델의 완전한 튜닝은 Full Fine-tuning, 메모리가 제한된 환경에서는 LoRA 또는 QLoRA 기법 등이 활용 가능함  

나. 파인튜닝의 세부기법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMjMz/MDAxNzQzNjA2MTE1NTc0.aFxKo9lMHi6X_Wi2Xa_rWCuyCZbs29PkQdrvkkQXgZUg.Y2ggQgUYy9lcXtkfig4DyST31TNN4dV15FJx6ie_lnkg.PNG/022.png?type=w1600)  

-&gt; DALL-E, GPT-4와 같은 사전학습 된 모델을 파인튜닝 시 배포 이후 모델 드리프트(성능저하)현상이 발생 가능하므로, 검색증강생성(RAG), 프롬프트 엔지니어링 기술과 접목 필요  

파인튜닝과 검색증강생성(RAG)의 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMjM0/MDAxNzQzNjA2MTUyMzYw.GP1cSO71PS48OyyP-S7HYKxypnK3mFwCqvN2wBWgvKcg.gvQyoN_eEqQzeslkOrGs7mAxSnTpXA72-21Cub-Ritcg.PNG/023.png?type=w1600)  

-&gt; 파인튜닝 후에도 모델을 지속적으로 학습시키고, 성능관리가 필요하므로 RAG를 이용한 AI 모델생성 발향으로 발전되고 있음  

### 모놀리스(Monolith)와 마이크로서비스(Microservice) 아키텍처의 개념을 비교하여 설명하고 데브옵스(DevOps) 구현시의 장단점에 대하여 설명

**[리드]**  

모놀리스 아키텍처의 한계극복, 마이크로서비스 아키텍처  

**[상세설명 및 해결방안]**  

모놀리스 아키텍처의 한계극복, 마이크로서비스 아키텍처의 등장배경  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMTIz/MDAxNzQzNjA2MjE1MzU1.WH2k0Htl45DKbkmZLIu79vjFODXbGWRP4by-UMr3T5Qg.iOjte77LZVdHU38GY0RAeh50KM_JsD-QmlvBovT_A1kg.PNG/024.png?type=w1600)  

-&gt; 기존 모놀리식 아키텍처는 사용자 증가나 특정 기능의 수요 증가에 따른 확장성 부족과 유지보수 및 배포의 어려움이 있었음  

-&gt; 마이크로서비스 아키텍처는 클라우드 컴퓨팅의 발전과 애자일 개발방법론의 확산 등 유연함과 빠른 배포가 가능한 환경에서 소프트웨어 개발의 핵심적인 아키텍처로 주목받고 있음  

모놀리스와 마이크로서비스 아키텍처 개념의 비교 설명  

가. 모놀리스와 마이크로서비스 아키텍처의 개념도  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMTcw/MDAxNzQzNjA2Mzc0MDUw.vys9eqaV5ijl8i4CZ7dzFafxY2BqVfrk9l250602q0Ag.HJvJn4RUJ6kYEiEhcD4IkV-5vxJXDGBmxWKKeSSsyQsg.PNG/025.png?type=w1600)  

-&gt; 마이크로서비스 아키텍처의 등장으로 이전까지의 단일 아키텍처를 모놀리스라고 분류  

나. 모놀리스와 마이크로서비스 아키텍처 개념의 상세 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMjE3/MDAxNzQzNjA2NDAzMDM0.PrYTsEY89QDTEhcoW5t33vFTOq8Z8BfKsUqUTzi5gMYg.RX_pltghak6EBQe_YKr9pa-D11un4zSXeQEEBqxaWU0g.PNG/026.png?type=w1600)  

-&gt; 전체의 서비스를 포함하는지, 최소한의 서비스만 포함하는지의 여부로 구분 가능  

데브옵스 구현시, 모놀리스와 마이크로서비스 아키텍처의 장단점 설명  

가. 모놀리스 아키텍처를 이용한 데브옵스 구현시 장단점  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMjk1/MDAxNzQzNjA2NDM1NTU5._EY0H87Stg_7FQ_SHiqvIGrE63qWyN89YvFJYm8UbLAg.0Sds52-2eePwawnGVSoLQEjPV__NfnEVtLU7ySAVDLMg.PNG/027.png?type=w1600)  

-&gt; 서비스 규모 증가 시, 유연한 대응이 어려워 주로 마이크로서비스 방식을 이용  

나. 마이크로서비스 아키텍처를 이용한 데브옵스 구현시 장단점  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMTMx/MDAxNzQzNjA2NDY2MTY1.0GnDzHuYCbXzZkdkhYrZTTh6ulqiiJooA10RTZGESEYg.-DcSssHCfPUBsTU9kENb8_cYGq3vwCe0y-9zykIAbV0g.PNG/028.png?type=w1600)  

-&gt; 데브옵스를 보다 효율적으로 구현하기 위해 마이크로서비스 아키텍처 이용  

효율적인 데브옵스 구현을 위한 방안 제언  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDNfMjQ2/MDAxNzQzNjA2NTA2NTEx.DG7oc3n2oH6LqANagGnM2TDkTLHkQdDpiz9_KbUS7asg.hAyrrhXAR5TPQpYESaX4LMV10ErSXAsHIYiePIhRx7kg.PNG/029.png?type=w1600)  

-&gt; 스케일이 커짐에 따라 단계적으로 마이크로서비스 아키텍처로 변화  

### 데이터베이스 사딩(Sharding)가. 샤딩의 개념 및 분할방법나. 샤딩과 파티셔닝 (Partitioning)의 차이점다. 샤딩 적용 시 고려사항

**[리드]**  

테이블 수평분할 분산처리, 샤딩  

**[개념]**  

물리적으로 다른 데이터베이스에 데이터를 수평 분할 방식으로 분산 저장하고 조회하는 방법  

**[상세설명 및 해결방안]**  

테이블 수평분할 분산처리, 샤딩의 개념 및 분할방법 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjQw/MDAxNzQ0MTc3NTcxNTA1.BpE5Ykn96Wh-dMfgm9bMWg6xi8hPG5TOc1ZZMKT7UMgg.eqB4djDg-xAp4DijVay_SxZsqQlX-bSGi1FbgeV-Er0g.PNG/006.png?type=w1600)  

-&gt; 데이터 증가와 테이블의 대형화에 따라 단일DBMS의 성능저하를 방지하기 위해 샤드키 기준으로 물리적 수평 분할하는 기법  

비교기반 샤딩과 파티셔닝의 차이점 설명  

가. 목적/구조 관점의 샤딩과 파티셔닝의 차이점  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfNiAg/MDAxNzQ0MTc3NTA4MjYw.FrT--tYj5HLlAyVD6tEt61PpJfATBx6zBC75MQYV8Ocg.box01oC0ACXFlf0_Kk9yiBicHqoguY9F7_WBy11B_9og.PNG/004.png?type=w1600)  

-&gt; 여러개의 인스턴스에 분할저장과 하나의 인스턴스에서의 분할저장에서 차이점을 가짐  

나. 특징 관점의 샤딩과 파티셔닝의 차이점  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjM5/MDAxNzQ0MTc3NTQwOTEz.QqxdUmHfX9Stk4IuFUTxq8Sh6zGQtz-TkIaUvuVNH1kg.bTWcx7wFtiDquK-EXzprnuly68P7A7-RunyEsXjKNRog.PNG/005.png?type=w1600)  

-&gt; 테이블의 수평분할과 수평, 수직분할의 차이로 이해 분할된 스키마가 동일 형식으로 저장되는 샤딩과 상이 또는 동일 형식으로 저장되는 파티셔닝으로 분류됨  

대량의 분산처리, 샤딩 적용 시 고려사항 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjQ2/MDAxNzQ0MTc3NjA3NDAx.xbJDpSvJAE-ZImX4WlAsPwDl9yywhDuW7aDskkCMYrAg.3nuxqPqPP66IhDHabflQjQQGzAP8Ju4bSQ-V3AOcXrEg.PNG/007.png?type=w1600)  

-&gt; 데이터가 늘어남에 따라 분산처리 속도가 증가하여야 하며 기본적으로 데이터가 균등분배를 할 수 있도록 샤딩구성을 해야 함  

-&gt; 실무에서는 균등 분산과 온라인 scale-out, 처리량을 고려하여 업무에 적용하며 균등 분산의 방법으로 쉽게 구현 가능한 모듈러 연산 이용 노드 지정 저장이 사용됨  

### 과학기술정보통신부는 2024년 12월 [철통 인증 지침(제로트러스트 가이드라인) 2.0]을 발표가. 제로트러스트(Zero Trust) 정의 및 핵심 원칙나. 제로트러스트(Zero Trust) 보안 모델 구성요소다. 제로트러스트(Zero Trust) 성숙도 수준 4단계 특징 비교라. 제로트러스트(Zero Trust) 도입 절차

**[리드]**  

무신뢰 검증 보안모델, 제로트러스트(Zero Trust)  

**[개념]**  

기존의 경계 기반 보안과 달리, 접근 주체에 대하여 네트워크 혹은 물리적 위치만으로 신뢰를 부여하지 않는 사상  

**[상세설명 및 해결방안]**  

무신뢰 검증 보안모델, 제로트러스트(Zero Trust) 정의 및 핵심 원칙 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjQ0/MDAxNzQ0MTc3NzY2OTcx.y0ioGOp4i8HVdkElBgxhi0Lw3opZF5iutKoqoXdIgHsg.5K8oCYQ9yLg3m3mV47b_ELWFFW0yRrPrioaaBkMak1Yg.PNG/008.png?type=w1600)  

-&gt; 갈수록 고도화 되는 사이버 침해와 다양한 디지털 기술의 확산으로 2023년 7월 제로트러스트 가이드라인이 최초 수립되었으며, 최근에는 실제 기업에 적용 가능한 도입절차와 방법론, 수준 진단 모델 '4단계 성숙도 모형'이 정의된 제로트러스트 가이드라인 2.0이 발표되었음  

-&gt; 제로트러스트는 기존의 경계 기반 보안 모델과 달리, 네트워크 내부와 외부의 모든 사용자 및 장치를 잠재적인 위협으로 간주하고, 모든 접근에 대해 엄격한 검증을 요구함  

제로트러스트(Zero Trust) 보안 모델 구성요소 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjAw/MDAxNzQ0MTc3NzcxMDU0.uxV821bXmy_x7wzrhL8CMxj9rA0o0cEK-JcunDDWGhog.ea7lN-w9tEIFQA2UDh-Z0B9UaeSYrEfvK24hLXOC4nUg.PNG/009.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTA3/MDAxNzQ0MTc3ODgwMjU0.2ZZHRNdwxWdM3AIvhxO3PTWnUxdvUAAOBHvfqt6krccg.ZhYroSfuOAU0QLfcK9Uvf0sD9bdz8KK3bZAPYeLi5R0g.PNG/010.png?type=w1600)  

-&gt; 제어 영역(PDP)에서 정책을 결정하며 데이터 영역(PEP)에서는 접근통제 정책 실행과 모니터링을 수행함  

제로트러스트(Zero Trust) 성숙도 수준 4단계 특징 비교 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfODAg/MDAxNzQ0MTc3ODg3MDQy.mEuNKOzsk2v6vinK0ZBfUEzHGNem82DXRMKyuqiUOzsg.T3XtkcidzWv0-rhzWkAIZCXGl-Pdd_cSCry6PVlzuSsg.PNG/%EA%B7%B8%EB%A6%BC1.png?type=w1600)  

-&gt; 현재 수준을 진단·분석하거나 목표를 설정하고 검증하는 데 활용할 수 있도록 기존 3단계에서 4단계로 구체화된 ‘성숙도 모형’이 정의됨  

제로트러스트(Zero Trust) 도입 절차 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjIg/MDAxNzQ0MTc3OTIzNjI3.iC1Y-jFFCoMtvrCa1FlRp771uo5Jqk3IcGSg_-Kvmjgg.tuaNT2tiXvfGa-bQCd7wPwMEcYgbJ3Yu0yTxpqroQ8gg.PNG/011.png?type=w1600)  

-&gt; 기업에서는 단계별 고려사항, 조직의 역할, 단계별 이행안 수립을 위한 구체적 방법론을 고려한 도입 준비와 실제 운영·정착 필요  

### 데이터베이스 튜닝(Tunning)의 3단계와 튜닝의 기대효과

**[리드]**  

데이터베이스 성능 개선, 데이터베이스 튜닝(Tunning)  

**[개념]**  

DBMS 및 OS, 시스템, 어플리케이션의 이해를 바탕으로, 불합리한 요소를 찾아 제거/수정하여 성능을 개선하기 위한 일련의 작업  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjQ5/MDAxNzQ0MTc4MDQxODEz.A-nbyHYKoDKmbQ3eVtiRIznRHzm9uVRGvrZW8ZrNlLMg.-TjxgCCoCAyHSl5Y9RA6dHExsLLx8N9Ug7-oAjn5mN8g.PNG/012.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjA3/MDAxNzQ0MTc4MDUyMzUx.qh_CFzGyYEEisvIR2R02rk1PdBLJ9qOLQin8nIEa0D8g.qSqh5U3n3qwOJZWhGrXenLE0J_toTX2HWFFozr5e3-wg.PNG/013.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTkz/MDAxNzQ0MTc4MDUyOTQ0.tMJ0kNXj6JTkTx5B7XtmXx5-Qi9AvMPyDkbY03NOvrog.PvXzFMFzpUszP8zzaewcdBQj8MZON6VQrv0c3V3R5I4g.PNG/014.png?type=w1600)  

### ISA/IEC 62443

**[리드]**  

산업제어시스템 보안 표준, ISA/IEC 62443  

**[개념]**  

전자적으로 보안적인 산업용 자동화 및 제어 시스템(IACS)을 구현하기 위한 일련의 표준, 보고서 및 부속 문서들을 포함하는 국제 표준  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTkg/MDAxNzQ0MTc4Mjg0MjIw.IrkmaYmnYoDkILWE9XXA6XEhqX0smKQRPERyinWlXPUg.SstEa4StPCcwwnZfXWg372hmm4HPd7KbUmc2ZKZy-FYg.PNG/015.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTQz/MDAxNzQ0MTc4Mjg0MjYx.2G0ui-U-rTF17st_es1hrgVg6rDQpar3rd3Bl7YZQsYg.kf93zGu79vHdpQL2OuwZsY_vAY25nalATar4PyL0DQYg.PNG/016.png?type=w1600)  

### 멀티 클라우드와 하이브리드 클라우드 비교

**[리드]**  

유연성과 효율화 극대화, 멀티클라우드와 하이브리드 클라우드  

**[개념]**  

멀티클라우드 : 두 개 이상의 퍼블릭 클라우드 서비스 제공자 사용  

하이브리드 클라우드 : 퍼블릭 클라우드 + 프라이빗 클라우드 환경을 통합 운영  

**[상세설명 및 해결방안]**  

유연성과 효율화 극대화, 멀티클라우드와 하이브리드 클라우드 개념 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTI4/MDAxNzQ0MTc4Mzg1NzE4._F0ItqUsHstf0Iwo3OwWGeQwcXb1Qy6XaW92dh4-UHMg.WRaFwBWgl5MZyn6OGfGa0EFRUE0q07qI-PNpmhgcZk0g.PNG/017.png?type=w1600)  

- 멀티 클라우드와 하이브리드 클라우드는 여러개의 클라우드를 사용한다는 점은 동일하나 서로 다른 목적과 특징을 가지고 있음  

멀티클라우드와 하이브리드 클라우드 상세 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjcz/MDAxNzQ0MTc4NDQwNjc2.9RNpUTRMmDTDm3zIu5qZ-3pXN5D-zuOJXKTgXyH_te0g.9DrnEJOXIbRRg5pcXM0-pl146_S0m05qXxj-RxmrAXQg.PNG/018.png?type=w1600)  

멀티 클라우드 관리 기술 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjQz/MDAxNzQ0MTc4NDcwNzgx.9SzRS3GLjDnp0MeF0rf8VrSIG6zYtwBRymDx2uVv0Uwg.iQVc_J47BnG_RqNg-jlxoX8af2ZDnE0cn2bRQSvJJHsg.PNG/019.png?type=w1600)  

### 의사결정나무의 지니지수(Gini Index)와 엔트로피 지수(Entropy Index)

**[개념]**  

지니 지수 : 의사결정나무에서 불순도 측정을 위해, 데이터의 통계적 분산정도를 정량화하여 표현한 지수, 즉 지니계수가 높을수록 데이터가 분산됨  

엔트로피 지수 : 정보량의 기대값을 나타내어 의사결정나무의 무질서한 정도 및 불순도를 수치화한 지수  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTQg/MDAxNzQ0MTc4NTAwODM1.VANSFYx1X0KEhaX91pFDfJRGRthtRHfArXjJaMw7fykg.h8oggZ-EMWX4wR1ZOG9-zqXDaBUYiXgtaIpAykzO0Awg.PNG/020.png?type=w1600)  

지니지수와 엔트로피 지수 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTk4/MDAxNzQ0MTc4NTQ0NjU4.dFljkUQoZMdDbP0XZojWpRvSQKmoP_InrtueVcI4fW0g.EDla12u_iSmu_zhbOttJ34jUC5g-pI3BR1EQKL44cBAg.PNG/021.png?type=w1600)  

- 엔트로피 지수 범위는 0~1사이며, 0에 가까울수록 노드 내 데이터들이 동질적임을 의미 , 목표변수가 이산형인 분류나무의 경우 상위노드에서 가지분할을 수행할 때때, 분류변수와 분류 기준값의선택 방법으로 카이제곱 통계량 사용 가능  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTI5/MDAxNzQ0MTc4NTk2MTE3.8-r-YlhevuevK-aeuhn161GxMDLHgKspTdCU73CU-ZEg.qBA65wdxWOPE8SctG-t1lPD4haWq9be9I92vPFusnHog.PNG/022.png?type=w1600)  

### 선형 자료 구조인 스택, 큐, 리스트의 자료 입출력 원리

**[리드]**  

순차적 자료 나열, 선형 자료 구조  

**[개념]**  

스택 : 한쪽 끝에서만 데이터를 넣고 뺄 수 있는 제한적으로 접근할 수 있는 후입선출 (Last-In-First-Out) 형태의 자료구조  

큐 : FIFO (First in First out; 선입 선출)의 특징을 가지는 자료구조  

리스트 : 데이터를 일정한 순서로 나열한 자료구조  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjYg/MDAxNzQ0MTc4Njg2ODY3.DSYXzXaj1-n92H47eO4o8Y75AEkzBGsSTMDwC0FmGJUg.MfTgUmcBnrbgnvNysXloWMFfR2oMj0rx44PANfR3YfYg.PNG/023.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfOTUg/MDAxNzQ0MTc4NzAwNjY3.ewQD0UB54jb3E1Y8kHMYb_k6-UkgzMLS0LjfBmXwlCAg.kcuZcmQNS5MdF8dDptDuSuSuDeengJN-ZU0M5ZzIB00g.PNG/024.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfODAg/MDAxNzQ0MTc4NzAwODky.Ul2Td3MkdLoS1qijwCp71oCQlr335xn1UvMEG5MR-Kcg.QZJn5HsrN2cA7PXOE5OZeDDX5oAVm562iBakNZdelukg.PNG/025.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMTU4/MDAxNzQ0MTc4Nzg3MDE1.We-DCwubmAEedXvKHVFYHUaoVAQ38dwWsSwzMZS4eVog.TW-XAcXos-0PqxOozFETKGEh1Nl7ReNV_AuraVHj1Ccg.PNG/026.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfOTcg/MDAxNzQ0MTc4Nzg2OTcw.k7b5ABzvuaS3tdZW5KGkE00fVOIW62N_s7CwAqScdkQg.W94EijVfN4E9ePETgZG89sq5hkhFme1IKD8wxBUu2Fkg.PNG/027.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfNTAg/MDAxNzQ0MTc4ODU2NjIx.NZlLjMDR3V30_cHLbcE95HAsY3vfI3EUGiZUR1LquB0g.pjo_PEA7QhcdTMsbHvhI5xeKWjJ5IwD3ob_SUOxnedog.PNG/028.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MDlfMjcx/MDAxNzQ0MTc4ODU2Mjky.sqrvyhHOz0o6WuxKmFjOcRU8fRQKsZVMIBYHX6X6bdcg.71dtc6FFWsdREGi-IIA_io0KBbjR5Q0SJPMh5xx9x7og.PNG/029.png?type=w1600)  

### 암호화 기법가. 블록(Block) 및 스트림(Stream) 암호화 기법나. 워터마크(Watermark)

**[리드]**  

신뢰할 수 있는 디지털 비즈니스 환경 보장, 암호화 기법  

**[개념]**  

네트워크를 통해 전송되거나 저장 장치에 보관된 데이터를 인가되지 않은 제3자가 함부로 읽거나 수정할 수 없도록 보호하는 기술적 수단  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfNiAg/MDAxNzQ0MzgzMjk5NzUz.y-CZ-dKNgr2dp5k43e_NPBTRCUGmPckR7jLiwJkbCbkg.8i448KBuqIhUymiNrZ0MYqTdhCdqeIVA7CWE4vtWjtAg.PNG/030.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMjkg/MDAxNzQ0MzgzMjk5NzU1.ubEUpurwPlgYJkvJoouYv40TT0x5GGMFQi9QkxtQPhEg.QY26zfZ31DP54C8nXLtu7Kh_dfKx8ZP229y5l18uUDgg.PNG/031.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMTI5/MDAxNzQ0MzgzMjk5Nzg0.6UGT1-XUeP7QNCVzWSeSQZBAukT982FXxeNbBQRXoDgg.K6DxBJHwrLnw0iI-3fV6OS2pPn2YI__atbRZEMxZW88g.PNG/032.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfNzYg/MDAxNzQ0MzgzMjk5Nzc4.kZjhimVlMz0Qr9OVUYfDLLsi8WT7OcNXWgNGEVnYSv8g.EqbuG0sEK2Mt2diWa_es3fMMNhN7l46y9Rj-KEKN-eUg.PNG/033.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfNTcg/MDAxNzQ0MzgzMjk5Nzg5.mMsvMELxFUT4ItNWQ0JuQ9JZrkMl30p8sm1b-Vuv6EYg.jTWU_EH-mtZMRUbEQAMv6tkiJ7xxzyfck4SUGqD3ZLAg.PNG/034.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMjk1/MDAxNzQ0MzgzMjk5ODgy.LJ-RzE0TJrv7VlPhTCAtraeljhH0xDnMQir2myeXlCUg.z9eCit8Q4poMtuqKXHm3S2vRYE5GpZN4_9vayTczb2Ug.PNG/035.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMzIg/MDAxNzQ0MzgzMjk5ODk5.wUD2kzmhVQ8OwsjXZi3ZvFr2-kp42eedYcsKuptR6Usg.vcimVaoHxdh8xxiN3-oCmFPb1EoabCES0zUPLEnvL8wg.PNG/036.png?type=w1600)  

### IT 프로젝트를 성공적으로 수행하기 위해 요구사항의 체계적인 관리와 문서화가 매우 중요1) 소프트웨어(SW) 요구사항 품질 속성2) 요구사항 도출 기법3) 요구사항 개발 프로세스

**[리드]**  

IT 프로젝트의 성공적인 수행의 핵심, 요구사항  

**[개념]**  

프로젝트가 성공하기 위해 반드시 충족되어야 하는 조건이나 능력  

개발 대상과 범위, 방법에 대해 사용자와 개발자가 합의하는 과정  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMjMw/MDAxNzQ0MzgzNDQ1MzAw.V6n1nG7i8_TXBQAzJ5E8vu4CA5iuypTsvSz9ieDDfwUg.DMckYybe4Qusi9ZSc7VsBwclaizu3LkZsoCP4h4sMxYg.PNG/037.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMjkw/MDAxNzQ0MzgzNDQ1Mjkx.M0W6yI4-ui06JlyuTvCUaZ4DsD0TUeRWsEWnhk9VdA0g.ODWb2Jx9WQYsOewqyLXb7SFwfdOYYWdWfcjgftZ054Ag.PNG/038.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMTk4/MDAxNzQ0MzgzNDQ1Mjk2.at4eZXywI0NW8GocyNm1bB3VerQ3QLerzjq-hAfN3C8g.QMdRwyavGMf-TqcG9JjobFo0BCbARdmX_XfNYf9h76Qg.PNG/039.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMjI2/MDAxNzQ0MzgzNDQ1Mjk0.zZA1E-KM879DGHiy1KCEU2FDWRdwTbPkHJgSE8FReFYg.4Cm-8daOia78lUmnB_nRGbOFtW6vuWib9PHSGuBwqUgg.PNG/040.png?type=w1600)  

### 형상관리 개념과 형상관리 기준선(Baseline)

**[리드]**  

소프트웨어 품질의 핵심, 형상관리  

**[개념]**  

소프트웨어의 무결성 및 품질 보장을 위해 모든 형상 항목을 식별, 통제, 기록, 관리하는 활동  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMjc2/MDAxNzQ0MzgzNTU2OTU1.vcwNgLzqEVXmimTvPAzD-ckOAPX74t9RXe5-yiwObHkg.j4F4j4pQ3BoKPqPJruOJcCpk_vpBxtzgu90sroFpXc4g.PNG/041.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTFfMTQx/MDAxNzQ0MzgzNTU2OTQ1.NYFdoI6hLEaKHiXyJTQ6VP-nfAX7G_ClO_-_0tsGyRQg.n3mvi6qMqTReQeUAI-S1fsy6zIOnRgu-6FcGz2_6gr0g.PNG/042.png?type=w1600)  

- 형상관리의 일관성을 위해서 CCB와 공식적인 기준선을 활용  

### 운영체제(Operating System)태스크 우선순위 상속(Priority Inhreitance)

**[리드]**  

태스크의 우선순위을 통한 우선순위 역전 해결, 우선순위 상속  

**[개념]**  

낮은 태스크가 높은 태스크의 자원을 점유할 때 우선순위를 높은 태스크와 동일하게 상속시켜 역전 현상 해결 기법  

**[상세설명 및 해결방안]**  

태스크의 일관성 유지, 우선순위 상속의 절차 설명  

가. 우선순위 상속의 절차도  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTI3/MDAxNzQ0NTQ0MTMyNTE2.Cu6pZvZ2i0u7xeUxfw1gkUpywck1OdxBBX4rwNLiDNUg.cI4hSmE7niJKgyArPvSbPqwTZ1PvQm8MA0_esOYrg8Yg.PNG/013.png?type=w1600)  

나. 우선순위 상속의 상세 절차 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTUy/MDAxNzQ0NTQ0MTc0MTQx.EZZigoGFPWIbyz0hvZo2w_Z-Kg5Chkdxy_NHBFwDmVkg.5TA2rC2PyUJatuzmftFIi_QSTXvcP1T_80ShwfrS5Jsg.PNG/001.png?type=w1600)  

- 태스크의 우선순위를 변경시켜 태스크의 일관성 및 동기화를 유지  

- 우선순위 상속은 여러 자원 사용 불가능한 문제 및 데드락 발생 가능  

우선순위 상속의 데드락 문제 해결, 우선순위 올림  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTM0/MDAxNzQ0NTQ0MjM1OTYx.5fCjQmXzHYvodbvufuX_439LBk9FQytRqNfaD4mGCz4g.We-5mL6io766AOGIj7eYALuVgbdb72j3gT-IGSAschwg.PNG/002.png?type=w1600)  

- 우선순위 단점을 해결하기 위해 자원의 우선순위를 사용하는 우선순위 올림 사용 가능  

### 머신러닝(Machine Learning) 성능지표

**[리드]**  

머신러닝의 성능 평가, 머신러닝 성능지표  

**[개념]**  

머신러닝 모델의정확성을평가하여 얼마나 잘 작동하고 성능을 평가하는지표  

**[상세설명 및 해결방안]**  

머신러닝의 품질 검증, 머신러닝 성능지표의 유형 설명  

가. 머신러닝 분류별 성능지표 요약  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTQg/MDAxNzQ0NTQ0MzA2ODY2.NySRjb6pOaPMUoL7HvVaRGTxdiyfHOhJNlenmf20vz4g.LJBwkZc0Fjck22L5LuzkE63fb75m065-XoVOdBkYNVMg.PNG/003.png?type=w1600)  

나. 머신러닝 분류별 성능지표 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfOTEg/MDAxNzQ0NTQ0MzU4NDk3.Rbra2V1EAq6LAE3-lpEn8K4wMYb6x8PCuvu2ejxQ9BQg.Z2u5I9KhOZAtek4GtuDszNEYXKlOaOVUMJDKTWSSK6Ag.PNG/004.png?type=w1600)  

- 머신러닝을 기본으로 LLM의 특화된 지표를 함께 활용 가능  

머신러닝 성능지표를 활용한 LLM 성능 평가 방법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTQx/MDAxNzQ0NTQ0NDEwNTQz.JgNouZznWdSwl1xu4Z6CFnYgsF3YWfyZ-v2h9ODlEsEg.EcClZRjnOAGe87DbfSSP2sLgTOxWkhY0ILIshdTZz6gg.PNG/005.png?type=w1600)  

- LLM은 정밀도, 정확도 등의 평가기법과 혼잡도, BELU 등의 평가지표를 활용  

### TCP(Transmission Control Protocol)프로토콜의 3-way handshake와 4-way handshake

**[리드]**  

신뢰성 있는 TCP 연결, TCP 3-way handshake  

**[개념]**  

인터넷에서 데이터를 안전하게 주고받기 위해(TCP/IP 프로토콜), 데이터를 보내기 전 **송신자와 수신자 사이에 신뢰성 있는 연결을 설정하는 3단계 과정**  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjk2/MDAxNzQ0NTQ0NDcxNjMw.Z2zihEZswMROLxfWZKjq273_dqcr3794P7ho5_fKWvUg.kHsfT5bAN6st6wB9k1IcuWfIK8T92NDQPAnu_H-M_qog.PNG/006.png?type=w1600)  

- 3단계를 통해 연결을 수행하고 종료할 때는 4단계로 실행  

안전한 연결해제, Tcp 4-way handshake 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjcw/MDAxNzQ0NTQ0NTMwMzYz.qu5hGLVT-ASpded0bY6sZCrxt1I6YoBdpLEVOnmpLOIg.DMv9j_mRaNF0JQVo0GqrSavsWpYIsya1-I1RuQOi8Tcg.PNG/007.png?type=w1600)  

- TCP의 3-way와 4-way에서는 ACK, SYN, FIN의 Tcp Flag를 활용  

- TCP의 3-way와 4-way에서는 Half Open 등의 취약점 발생 가능  

TCP 3-way와 4-way의 단점 해결, SCTP  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjM3/MDAxNzQ0NTQ0NTc4MDQ0.406Up8dxByeHQ8WauVt82XgPU4QMu16cFri6PKHZFYYg.WzLkPuPgCFPoBcH_Dal6NKQqdSvV_PdQsTUlPIv53OEg.PNG/008.png?type=w1600)  

- SCTP 통해 TCP handshake 취약점 해결  

### 데이터베이스 트랜잭션 회복(Recovery) 기법가. REDO와 UNDO를 이용한 방법나. 체크포인트(Checkpoint)를 이용한 방법다. 그림자 페이징(Shadow paging)을 이용한 방법

**[리드]**  

트랙잭션 데이터의 무결성 보장, 트랜잭션 회복  

**[개념]**  

데이터베이스(DB) 운영 중 시스템 다운, 하드웨어 결함, 소프트웨어 오류 등으로 인해 장애가 발생했을 때, **데이터베이스를 장애가 발생하기 전의 일관성 있고 올바른(모순이 없는) 상태로 되돌리는 기술**  

**[상세설명 및 해결방안]**  

트랙잭션 데이터의 무결성 보장, 트랜잭션 회복의 중요성  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMzYg/MDAxNzQ0NTQ0NjMzMjI4.P7FqzYZNuea7p2oup_miSvJQ6PzR_CaabW3Akcdy5p8g.47mSVSswkp5D9qCy81hPF0borHGQCTDY5ye8gXsk1iAg.PNG/009.png?type=w1600)  

- 데이터베이스의 무결성 및 일관성을 위해 회복 기법을 활용  

Redo와 Undo를 이용한 회복기법 설명  

- 즉시갱신 : 완료 전 장애가 발생하면 Undo 수행, DB에 결과 즉시 반영  

- 지연갱신 : 장애 발생 시 Log 무시, Redo 수행, 로그에 기록 저장, DB에 한번에 반영  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjc0/MDAxNzQ0NTQ0Njc5NjUw._4lPQHvsEmXE9qMbme08v8FBlkETY5NmAPGD0LK1ZJsg.CuVk3nbO0X_MJ0JM5X5PuxsxgM9KLddPUoNH-RO_YC4g.PNG/010.png?type=w1600)  

- Redo와 Undo를 효과적으로 사용하는 체크 포인트를 이용한 회복기법 활용 가능  

체크포인트를 이용한 회복기법 설명  

- 장애 발생 시 가장 최근 검사점 이전의 트랜잭션은 회복을 미수행하고, 검사점 이후 작업만 회복을 수행하는 기법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjc2/MDAxNzQ0NTQ0NzM0NDYx.cjdtJClg2Zvt3S0XGKQw2Lr4Hhgpdbenmmd4IolG7-Yg.jJzDPhs-IL0-CuYlKjX8hTGbkIq0_Mo06Mx24RSilJ4g.PNG/011.png?type=w1600)  

- 동일한 데이터의 복사본을 활용하는 그림자 페이지 기법도 활용 가능  

동일한 복사본을 이용하는 그림자 페이징 회복기법 설명  

- 그림자 페이징은 현재 페이지와 그림자 페이지를 생성하고, 장애 발생 시 그림자 페이지를 이용하여 회복하는 기법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTMy/MDAxNzQ0NTQ0Nzg4Mzk5.JZWGyATRsY0SAS7J03ihWOsB_v23HeRHL6dZTwjhSRYg.9OP3d4g0_zlsjwPEVo6SUWof69dA-C73wcq0SDwaTCsg.PNG/012.png?type=w1600)  

- 그외 Aries 등의 회복 기법 활용 가능  

- 트랜잭션 회복 기법을 통해 트랜잭션 및 데이터의 무결성과 신롸성 등을 유지 가능  

- 빅데이터 및 NoSql에서는 트랜잭션 회복 기법에 샤딩 등의 기법을 통하여 일관성 유지 가능  

트랜잭션 회복 기법을 통한 기대효과  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTcg/MDAxNzQ0NTQ0ODM4Mjk0.-Mn5Ebf7vhXDXWWlY_aO4OUZnoEVFhBMffE4y9rpAj0g.bxvmd__p0V8LznGEJNy7NvbQDKEONBIFJoNAC1RWIdYg.PNG/013.png?type=w1600)  

- 최근 일부 MongoDB와 같은 NoSql에서도 트랜잭션이 지원되기 때문에 회복기법으로 일관성 유지는 더욱 중요해지고 있음.  

### VPN(Virtual Private Network)가. VPN의 개념 및 특징나. IPSec(Internet Protocol Security) VPN과 SSL(Secure Socket Layer) VPN다. VPN의 기술요소

**[리드]**  

재택 근무의 보안의 중심, VPN(Virtual Private Network)  

**[개념]**  

터널링 기법을 사용해 공중망에 접속해 있는 두 네트워크 사이의 연결을 마치 전용회선을 이용해 연결한 것과 같은 효과를 내는 가상 네트워크  

**[상세설명 및 해결방안]**  

재택 근무의 보안의 중심, VPN(Virtual Private Network)의 개념 및 특징  

가. 사설 네트워크의 전용 네트워크화, VPN의 개념  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTIg/MDAxNzQ0NTQ0OTI2NDAw.tCGDlgwVruzaiGxbZdBtqvhseI69s93p6ajyp59HRCAg.tHVot6HxL_LdmrfYwlyrdtyE9VseiDHix2WLpCu7144g.PNG/014.png?type=w1600)  

- VPN은 안전한 통신을 위한 암호호 등의 특징을 소유  

나. 보안성을 겸비한 VPN의 특징  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNzEg/MDAxNzQ0NTQ0OTY0MDYx.h9PiQvkaksa55M6Dims5ljVTxFq4Jd9MdbQ2RRm-_ckg.CPg9XIrDWydasHG1AdtQWyEEHNRrMJPUVN8Z3JlCrpAg.PNG/015.png?type=w1600)  

Layer-3의 IPSec을 활용, IPSec VPN과 Layer 4 이상의 SSL VPN 설명  

가. RFC 2401 기반, IPSec VPN 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfOTIg/MDAxNzQ0NTQ0OTkyNjYw.B0Slhp5-IkHLdjdH5KjbHQu4jiSw9cGulpte30gmKTMg.RWFZWa9lV7b8y3zycQ6Ccw_oyonMAuKJ9VhCeaUtrukg.PNG/016.png?type=w1600)  

- IPSec의 비용 등을 고려하여 SSL을 활용한 SSL VPN의 활용 증가  

나. RFC 2246 기반, SSL VPN 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjgz/MDAxNzQ0NTQ1MDMzNDIz.vMRF-QnjEXcjJBPyG2AxVvI7A69FxaGAVqdWW5uwrsgg.2LiLSVZwGpM_WPkzUYXdByTecG74MrIv0cfJdEDr4zIg.PNG/017.png?type=w1600)  

- 효과적으로 IPSec, SSL VPN을 운영하기 위해서는 암호화, 구현 방식 등 다양한 기술요소를 적용 및 활용  

안정적 VPN 운영을 위한 VPN의 기술요소 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNDcg/MDAxNzQ0NTQ1MDk0MjAy.l4_v3EzxSlvtOSQQ4zK0VrYHHXQfuHyytKlAgT8fuqEg.8Mw55x3SAob4xXaCttvBE8YXN1scg6JEzuoiV74cxywg.PNG/018.png?type=w1600)  

- 이러한 VPN을 이용하여 보안 강화, 업무 효율화 향상을 기대하지만 비용, 정책 등을 고려  

기업의 업무 효율 향상을 위한 VPN 도입 및 운영 시 고려사항  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTAw/MDAxNzQ0NTQ1MTU3Mjcz.hhPQ2P9AilUnSXI8Mu9-XGNkbS8QXah1-TOYZneDUY0g.K78ZsO0jh697Mbji1dvD4Pm4IH6RnOC-re2IM1Og2YUg.PNG/019.png?type=w1600)  

- 최근 보안 및 신뢰성을 위해 제로트러스트와 함께 적용  

### 인공지능 소프트웨어 품질 보증을 위한 테스트 기법가. 메타모픽 테스트 (Metamorphic Test)나. 뉴런 커버리지 테스트 (Neuron Coverage Test)다. 안전 반경 최대화 테스트

**[리드]**  

인공지능 소프트웨어의 품질 보증을 위한 테스트 기법  

**[개념]**  

규칙 기반이 아닌 데이터 학습 기반으로 동작하는 AI 시스템의 신뢰성, 안전성, 강인성(Robustness)을 검증하기 위한 일련의 특화된 기법들  

**[상세설명 및 해결방안]**  

인공지능 소프트웨어의 품질 보증을 위한 테스트 기법의 중요성  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTEx/MDAxNzQ0NTQ1MjYwMDU0.CHCtHAYeDXb2NAH5zTXyGA1w7eUt97tGGjGpFMxG4Usg.2Ds0mSpo9Eiw5h0L5mD7gT7Os4LRrg42zqIWKXQCVbUg.PNG/020.png?type=w1600)  

- 인공지능 소프트웨어는 비결정성, 테스트 오라클 문제로 인하여 메타모픽, 뉴런 등의 테스트 필요  

인공지능의 Big-Q 향상, 메타모픽 테스트와 뉴런 커버리지 테스트 설명  

가. 변성관계 활용 블랙박스 테스팅, 메타모픽 테스트 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjk0/MDAxNzQ0NTQ1MzA4Njg0.2ndeF6Z-Go_rOKrbtf-i-Pztw-iOUmWA9KfZA7O4eh8g.nDZFUjsmoEWOkoiWzLHcxoPK1LsoZGdMkLLWG-ehNeIg.PNG/001.png?type=w1600)  

- 신경망의 신뢰성 향상을 위한 뉴런 커버리지 등의 화이트박스 테스트 기법도 활용 필요  

나. 뉴런의 활성화 활용한 화이트박스 테스팅, 뉴런 커버리지 테스트 기법 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjIw/MDAxNzQ0NTQ1MzQ3NTE5.FPmueZcnOjvGnLGicFobn1nYxAt6pJ7yt43UA71n3tQg.XVYxSnyFuSGuDpBDnvUFV0-t7WYfQsuIW21QSrCWnqkg.PNG/002.png?type=w1600)  

- 메타모픽과 뉴런 커버리지 테스트를 넘어서 안전성을 위한 안전 반경 최대화 검증도 중요  

인공지능의 안전한 활용 검증, 안전 반경 최대화 테스트 설명  

- 인공지능은 안전한 상태에서 활용이 중요하기 때문에 언전 반경 확인이 매우 중요한 요소임  

가. 안전한 환경 확인, 안전 반경 최대화 테스트 개념 및 구성요소 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNzkg/MDAxNzQ0NTQ1Mzk1NDk4.qMA6D1V9iZVP05aUGhFH6Q-0MiOpnlPW_EGjWlbme6sg.UJGdznt22bX8gN0P1QdWyP3DAeMhWJDJFniXhwrByFog.PNG/003.png?type=w1600)  

나. 안전 반경 최대화 테스트 상세 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTI3/MDAxNzQ0NTQ1NDQzOTQy.UcTv7cGIvTZ4zX54fY-vqunR1klS-X-XJVyeyc1PUxkg.A-2Pm__EOAC792WeRRLNqDQ0qF0BtpZM1ODsyYTOAAQg.PNG/004.png?type=w1600)  

- 최근 인공지능의 활용이 증가하면서 품질 검증을 위한 다양한 테스트 기법 적용하여 신뢰성 향상 필요  

인공지능의 신뢰성 향상을 위한 인공지능 소프트웨어 품질 검증의 다양한 효과  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfOTcg/MDAxNzQ0NTQ1NDk3NDU2.4B189lsFx2OYHtSXeE7ZSXUxYlt6nrIdOaNcnnesITQg.XXTRmYIKDIyLwKzozVu72CobUamvCGgVNbfU8MuXNtEg.PNG/005.png?type=w1600)  

- 인공지능 소프트웨어 테스트를 통해 다양한 산업에서의 신뢰성 향상 및 고품질 서비스 제공 가능  

### 경험기반 테스트 기법

**[리드]**  

테스터의 경험적 지식 활용, 경험기반 테스트 기법  

**[개념]**  

테스트 설계자가 자신의 지식, 직관, 경험을 바탕으로 테스트 케이스를 도출하고 결함을 찾는 소프트웨어 테스트 기법  

- 형식적인 문서나 명세서보다는 테스터의 노하우와 감에 의존하는 방식으로, 특히 명세서가 부족하거나 시간이 제한된 상황에서 효과적으로 활용  

**[상세설명 및 해결방안]**  

특징  

- 형식적 절차보다는 경험에 의존  

- 테스터의 도메인 지식, 과거의 결함 경험, 직관 등을 적극 활용  

- 빠르게 결함을 찾는 데 유용  

- 문서화된 테스트 케이스가 없거나 불완전할 때 적합  

주요기법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjU5/MDAxNzQ0NTQ1NjU2Njc4.XL3-YXXoXnKhPWfEOFbni3ITFzfBz7sCdOW-refY5XYg.ccKCW6W9z9ZD9l3D4u6Yy0DoZrc53U2fw7h7nAlHYFEg.PNG/006.png?type=w1600)  

기법별 장단점  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNzMg/MDAxNzQ0NTQ1Njk0NDQ3.RWAA7JqG5vS59lPuhi5hclf_VxqcF626ypjeVBAhxMYg.Joq40iJvxbudv4OovJyKGOD5-AZZW8CDdH2OpK2yK5Ug.PNG/007.png?type=w1600)  

### BSC(Balanced Scorecard)와 OKR(Object Key Result) 비교

**[리드]**  

조직의 전략적 목표 달성과 성과 관리, BSC와 OKR  

**[개념]**  

(BSC) 재무의 관점(과거) 뿐만 아니라 고객의 관점(외부)과 내부 업무 프로세스의 관점(내부) 그리고 학습과 성장(미래) 관점이라는 4가지 관점에서 기업의 경영을 평가하려는 분석기법  
(OKR) 조직이나 개인이 도전적이고 명확한 목표(Objectives)를 설정하고, 이를 달성하기 위한 구체적이고 측정 가능한 핵심 결과(Key Results)를 정의하여 실행 중심의 성과관리를 유도하는 방식  

**[상세설명 및 해결방안]**  

특징 비교  

가. BSC (Balanced Scorecard)  

- 전략적 성과관리 도구  

- 재무, 고객, 내부 프로세스, 학습 및 성장의  

4가지 관점에서 조직 성과를 균형 있게 관리  

- 전략을 구체적인 KPI로 연결  

나. OKR (Objectives and Key Results)  

- 도전적 목표 중심의 실행 관리 도구  

- 명확한 목표(Objectives)와 측정 가능한 핵심 결과(Key Results)를 기반으로 설정  

- 민첩하고 유연한 실행 중심 성과 관리 방식  

상호보완적 활용 제언  

- (전사 전략 수립) BSC를 활용해 장기 전략과 각 부서의 전략 목표를 설정  

- (실행 도구로 OKR 도입) 각 부서나 팀은 BSC에서 도출한 전략 목표를 기반으로 분기별 OKR을 설정  

- (성과 관리 및 리뷰) BSC의 KPI와 OKR의 Key Results를 함께 추적하여 전략적 정렬과 실행 성과 모두를 관리  

### 다차원 색인구조(Multidimensional Index Structure)

**[리드]**  

다차원 데이터 검색 시간 복잡도 최소화, 다차원 색인 구조  

**[개념]**  

다차원 데이터를 효율적으로 저장하고 검색하기 위한 데이터베이스 또는 정보 검색 분야의 자료구조  
- 공간 데이터(예: 위치, 범위 검색), 시계열, 벡터, 이미지, AI 임베딩 등 다양한 응용에서 활용  

**[상세설명 및 해결방안]**  

필요성  

- 기존의 1차원 인덱스 구조(B-Tree, Hash 등)는 단일 키 기반 검색에는 강하지만, 다차원 쿼리(예: [x, y] 범위 내 모든 점)에는 비효율적  

유형  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTgw/MDAxNzQ0NTQ1ODI3MzUz.OgMG4najOh7u-pxRk577s4XQbDTUvo4oW9DlKJSox48g.c0HfBoEYub1m8I8IQl7xWi7Ah6ulWrRObn2QsKXFfG8g.PNG/008.png?type=w1600)  

선택 기준  

- 저차원(2~3D) -&gt; R-Tree, KD-Tree  

- 고차원(&gt;10D) -&gt; Ball Tree, LSH, VA-File  

- 정확도 필요 -&gt; KD-Tree, R-Tree  

### 통계학의 4가지 척도

**[리드]**  

수집 데이터 특성 수치화, 통계학의 4가지 척도  

**[개념]**  

사물이나 사람 등 대상의 특성을 통계상 수로 표현하기 위해 체계적으로 그 속성에 숫자를 부여한 기준  

**[상세설명 및 해결방안]**  

종류  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTU2/MDAxNzQ0NTQ1OTAzODMz.Ol9_yS7_3tSawPr7_mdpBxd3vUbFRm2am8eMNGiH6NIg._XGyTxabiHdKb2LvIGBJjApw-N1hGlkI6umz-eq1lkkg.PNG/009.png?type=w1600)  

척도의 활용  

- (평정척도(rating scales)) 평가자가 측정대상(주어진 현상, 인물 또는 사물)의 속성이 연속선상의 한 점에 위치한다는 전제에서 일정한 기준에 따라 대상을 평가하고 그 속성을 구별하는 척도  

- (리커드척도) 평정척도의 변형, 여러 문항의 개별 응답 점수를 합하여 척도 구성한다는 의미에서 총화평정척도(Summated Rating Scale)라고도 함  

### 트랜잭션 격리 수준(Transaction Isolation Level) 4가지를 사례 중심으로 설명

**[리드]**  

일관성 및 병행성 트레이드오프, 트랜잭션 격리 수준  

**[개념]**  

트랜잭션 실행 중 중간 연산 결과가 다른 트랜잭션으로 접근 불가하도록하는 고립성을 유지하기 위한 데이터를 허용하는 수준  
- Read Uncommitted, Read Committed, Repeatable Read, Serializable의 4가지 수준  

**[상세설명 및 해결방안]**  

격리수준 4가지 사례 들어 설명  

가. Read Uncommitted (읽기 미완료 허용) - 다른 트랜잭션에서 아직 커밋하지 않은 변경 내용을 읽을 수 있음  

1) 문제점: 더티 리드(Dirty Read) 발생 가능  

2) 사례: 트랜잭션 A: UPDATE 계좌 SET 잔액 = 잔액 - 100 WHERE 사용자 = '김씨' (아직 커밋하지 않음)  

트랜잭션 B: 김씨의 잔액을 조회했더니 100원이 빠진 상태가 보임  

그런데 트랜잭션 A가 롤백되면, B가 본 데이터는 실제로 존재하지 않는 값  

나. Read Committed (읽기 커밋만 허용) - 커밋된 데이터만 읽을 수 있음  

1) 문제점: 논리적 일관성이 부족할 수 있음, 반복 불가능한 읽기(Non-repeatable Read) 발생 가능  

2) 사례: 트랜잭션 A: 김씨의 잔액을 읽음 1000원  

트랜잭션 B: 김씨의 잔액을 900원으로 수정하고 커밋함  

트랜잭션 A가 다시 하씨의 잔액을 조회했더니 900원으로 바뀌어 있음  

다. Repeatable Read (반복 가능 읽기) - 같은 트랜잭션 내에서는 동일한 SELECT 결과가 항상 같음  

1) 문제점: 팬텀 리드(Phantom Read) 가능(행은 변하지 않지만, 새로운 행이 나타날 수 있음)  

2) 사례: 트랜잭션 A: "잔액이 1000원 이상인 사용자 목록"을 조회 김씨, 이씨  

트랜잭션 B: 새로운 사용자를 등록하면서 잔액을 1200원으로 설정하고 커밋  

트랜잭션 A가 다시 같은 조건으로 조회하면, 이전에 없던 새로운 행이 추가되어 있음 (팬텀 리드)  

라. Serializable (직렬화 가능) - 트랜잭션들이 마치 순차적으로 실행된 것처럼 완전한 격리 보장(가장 높은 정합성 보장, 모든 이상현상 방지)  

1) 문제점: 성능 저하, 동시성 낮음  

2) 사례: 트랜잭션 A: 잔액이 1000원 이상인 사용자 조회, 트랜잭션 B는 트랜잭션 A가 종료될 때까지 새로운 사용자 추가나 수정 불가  

그래서 트랜잭션 A가 조회한 사용자 목록은 항상 일관됨  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNTMg/MDAxNzQ0NTQ2MDA3MDc0.xXYQMT5J30fX4mVms7TdM0gV-OVataTkN13s8HAOyUkg.dkyO1ySpH9hsBzXZROFriDXWEdUkpEuteM44jqMOb_sg.PNG/010.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjg0/MDAxNzQ0NTQ2MDA3MDY2.8Tvt-It86zsIi27r3kTy3hxNcTBQbc0TLbYyeH-MAaMg.UR_ilH22Xhiy39j-MNMH7fmnf1l9Va5lv07uFNMoWisg.PNG/011.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjEz/MDAxNzQ0NTQ2MDU4ODEw.v-QPY-CYcPZzIW-nrEqZAlYh5rtiVt2L9lRBDE6AJ-Ug.-ON016-LLV0f1eldGJDigvK-U_1Q4qv1hCO80ZXnB4Mg.PNG/012.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjcy/MDAxNzQ0NTQ2MDU4ODA2.XmwBIAI16_HaLhz0V2SNlCq6OI0hMUGA8KlvBHvibDMg.d9fydLfQFIJ3PrGRMClnxjN9ynxMyL7nMPp7vQQe2Mog.PNG/013.png?type=w1600)  

### 스푸핑(Spoofing) 공격가. 스푸핑 공격의 개념나. ARP 스푸핑 공격 방법과 보안 대책다. IP 스푸핑 공격 방법과 보안 대책라. DNS 스푸핑 공격 방법과 보안 대책

**[리드]**  

보안 신뢰 체계 무력화, 스푸핑(Spoofing) 공격  

**[개념]**  

공격자가 신뢰할 수 있는 대상으로 위장하여 정보를 탈취하거나 시스템에 접근하는 사이버 공격 기법  
- 공격자가 자신의 신원을 숨기거나 다른 신뢰된 개체로 가장하여, 사용자나 시스템을 속이는 공격  
- 주로 인증되지 않은 접근, 정보 탈취, 피싱, 서비스 마비 등을 유도  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTQz/MDAxNzQ0NTQ2MTA3OTM4.sIg4wMDhNhcMjAXMJisAkkDLInbIrHDVQvpKErBN7Pkg.3mUFJoszCoAji7F7CM6t86sReNlUwfmHsJo-AOVa8O4g.PNG/014.png?type=w1600)  

ARP 스푸핑 공격 방법과 보안 대책  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjkg/MDAxNzQ0NTQ2MTk4NzQz.pl3AhFYrmLjRN6TsVb1bJ3vAFQuljTnfZQ_iAlLc5aQg.gVRVFoRhbZ1wJKmUi9p5sTv9_H4ywZUU3IyRqFRQgywg.PNG/015.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTkw/MDAxNzQ0NTQ2MTk4NzQ0.EIHNpTluUb04IiYTVaD6zle7kUEg-2pWzK9_EJdu5dQg.V7zocZvhoYmHW9Bl237UGxOT6z0geWf589TSu9rfv0Ag.PNG/017.png?type=w1600)  

- ARP 스푸핑은 공격자가 위조된 ARP 메시지를 네트워크에 보내 다른 장비를 속여, 트래픽을 가로채거나 중간자(MITM) 공격을 수행하는 기법  

IP 스푸핑 공격 방법과 보안 대책  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTYw/MDAxNzQ0NTQ2MjY4NjM2.tBZjNfB89DVf6e5N5DXZME7PC1Ckxl4H_pB8HJCoV48g.tWJVL2sMCxV-Z9OXxJ0s0DWG2LD1VEHf4KhbjuGKfyAg.PNG/018.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjUy/MDAxNzQ0NTQ2MjY4NjIz.8oQa2YKMk9mVefm_MdQsOeR0dcAsAhicmernF1Ko3pcg.WK7ePET6cyLnrIdXHOuGUD0fY8fGSqk824Sz_GqyFdsg.PNG/019.png?type=w1600)  

- 공격자가 자신의 IP 주소를 위조하여 신뢰받는 시스템이나 사용자처럼 위장해 공격을 수행하는 기법  

- 패킷의 출발지 IP 주소를 조작하여, 피해 시스템이 공격자를 신뢰된 대상으로 착각하도록 만듬  

### 가상머신(Virtual Machine)과 컨테이너(Container)에 대하여 구체적으로 설명하고, 차이점을 상세히 설명

**[리드]**  

인프라 자원의 효율성 극대화, 가상머신(Virtual Machine)과 컨테이너(Container)  

**[개념]**  

1) 가상머신: 가상화를 통하여 구현되는 복제된 컴퓨팅 환경  

2) 컨테이너: 모듈화되고 격리된 컴퓨팅 공간 또는 컴퓨팅 환경  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjA0/MDAxNzQ0NTQ2MzIzMzA1.-i74UYgjDoHiVFbFlJkgQrE6h76XJfSojDcDEtrnnJ8g.TugZEuU6v1suDCBNRYSdicYD0xik6e4zHSZIMJrQ0MAg.PNG/020.png?type=w1600)  

목적  

1) 가상머신  

- 하나의 하드웨어위에 동시에 여러 종류의 운영체제나 프로토콜을 실행  

- 하나의 하드웨어 자원을 여러 사용자에게 분할  

- 가상화를 통해 분할된 시스템 간 상호 간섭이 없는 독립성(Isolation)을 보장  

2) 컨테이너  

- 시스템 환경 의존성을 탈피하고 안정적으로 구동  

차이점 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjM0/MDAxNzQ0NTQ2Mzc3ODgz.fKQcrZDPpY4sJfBwDCPMm0hsL2cUiz5Sgl6H2wXlq7kg.fNVGiTVPgN8d0n5TVELKafkUvmk1_99AtAe2VuSbfaAg.PNG/021.png?type=w1600)  

### WBS(Work Breakdown Structure)

**[리드]**  

작업 분할 구조도, WBS(Work Breakdown Structure)  

**[개념]**  

100% rules, 3~5단계 수준  

산출물 → [범위 기준선, Scope Baseline]  

- 일정관리, 고객과 팀원간 의사소통의 수단 등에 어떻게 활용  

- 기준선의 명확화로 Gold-plating이나 Scope creep 방지  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTAz/MDAxNzQ0NTQ2NDI1MDcz.fW8pqgLa_oXWqnSWsDu6NdEb6LchVCnBdZ06kaIg7vgg.5Z-pmm-cucFhv1KJUo4WzG0paRCH2g1wK1aqCoudBGog.PNG/022.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTYg/MDAxNzQ0NTQ2NDI1MTIw.5iglbBzs6PVFFxKIlTJvrFaz6_nlmCPwwAVjQO4xATMg.piqht0_fc7nTozPMXdJN-9DyjHDICc0hnr0iV07diwwg.PNG/023.png?type=w1600)  

### 세마포어(Semaphore)

**[리드]**  

P/V 연산을 통한 상호배제, 세마포어  

**[개념]**  

멀티프로그래밍 환경에서 임계구역의 경쟁조건을 P, V연산통한 상호배제로 공유자원에 대한 할당과 반환을 제한하는 프로세스 동기화 기법  

**[상세설명 및 해결방안]**  

세마포어 동작 매커니즘  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfODkg/MDAxNzQ0NTQ2NTQyMjQ0.0pZ5b4WKimOwMb-gSSSIoFdM5tQRJrT99-t-H8wgB2sg.0zRob_ITEyvw46U4HkUuO8MNvaR1kaDl-3AuKU1UErwg.PNG/024.png?type=w1600)  

나. 세마포어의 P, V 연산 원리  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjI1/MDAxNzQ0NTQ2NTk3NDMw.40DRkhp4Tl_A7AmYBzPi49t_NApk7C5l3y8OkFKzPq4g.xHnptoghgbSMk7bweNf772gRleRfQfuAP62_mGtO4rwg.PNG/001.png?type=w1600)  

세마포어와 모니터 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTQ0/MDAxNzQ0NTQ2NjMzOTc1.qQLBA7Vo11VZBdShbGYSwIEOfe0ld6MnFC7KBK266IYg.CH0lxe6eH5RzS82qz9GsoZsDnnA9IypEV9F2ElbVyDog.PNG/002.png?type=w1600)  

### CMMI(Capability Maturity Model Integration)

**[리드]**  

여러 CMM 평가 모델을 통합한 SW 역량 성숙도 평가모델, CMMI  

**[개념]**  

제품 및 서비스의 개발과 유지보수, 획득 능력을 향상시키기 위해 카네기 멜론 대 소프트웨어 공학연구소(SEI)가 소프트웨어와 시스템 영역의 여러 역량 평가모델을 하나로 통합하고, 업무절차들을 체계화하는 만든 역량 성숙도 평가 모델  

(CMMI의 기능)  

- 프로세스 교준화의 기준과 방향을 제시, 조직 프로세스에 대한 측정 뿐 아니라 평가 지표로도 활용, 능력과 성숙도 평가, ISO 15504(SPICE)와 호환  

**[상세설명 및 해결방안]**  

CMMI 성숙도 5단계 및 CMMI 평가 방법  

가. CMMI 성숙도 5단계  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTc5/MDAxNzQ0NTQ2NzgxMDc1.VXe6R6gCTDYvmDhi8Ou1Du6mY3BHDyURUmK71Eh0TdIg.0iuUsoflMugh3UuHMCXUQipsfK_mAfctIFrTxKEldxIg.PNG/004.png?type=w1600)  

나. CMMI 평가 방법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfOTQg/MDAxNzQ0NTQ2Nzg2ODUy.tJxqf4ZG7dPFE85TznjEuhMHB5SSqOtPAq_GGU4n38kg.lHbJEydTzroqo-H4PR5Dhm-y8AdDaWyGpYrEC2LVggAg.PNG/005.png?type=w1600)  

평가 단계 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTY4/MDAxNzQ0NTQ2NzIzMjM1._gwEkM6lIel6fbAoV7LMZuRrUaOsJwobqPC6ug3proUg.bBs6MPiEajHJqnzl7DDqZq_IJAH789QACfR7JGLLYAsg.PNG/003.png?type=w1600)  

### BCP(Business Continuity Planning) 수립 시의 주요 지표와 DRS(Disaster Recovery System) 구축 시의 핵심 고려사항

**[리드]**  

기업 비즈니스 연속성을 위한 계획, BCP와 DRS  

**[개념]**  

BCP 개념 : 각종 재해, 장애, 재난으로부터 위기관리를 기반으로 재해복구, 업무복구 및 재개, 비상계획 등의 비즈니스 연속성을 보장하는 체계  

DRS 개념 : 재해복구계획의 원활한 수행을 지원하기 위하여 평상시에 확보하여 두는 인적, 물적 자원 및 이들에 대한 지속적인 관리 체계의 통합  

- 지난 22년 데이터센터 화재로 인한 카카오 서비스 먹통 사태와 같이 주요 서비스의 가용성 훼손 시 사회적, 경제적 피해 규모가 커짐에 따라 디지털 재난관리 강화를 위한 ‘디지털안전 3법’ 제정 등의 움직임 발생  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMzUg/MDAxNzQ0NTQ3MDA5ODIz.VwhHOMX_CvDCYmVWGD9JfMs0hhXqwvWlc8kxVd67EHUg.2y7oKhd1cylsLiDN2x_Bt_6bystohHOCoVayV4Me-TQg.PNG/006.png?type=w1600)  

BCP 수립 시의 주요 지표와 DRS 구축 시의 핵심 고려사항 설명  

가. BCP 수립 시의 주요지표 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjYg/MDAxNzQ0NTQ3MDk5MzI5.mm4SEUdB55bPrf8VmQWVpBOOxsa5WLdOhhs7TGg7Nwog.vWoZA2ndPPVGKCmL6Qywcp_aMPwdkUPNjm4qKpEzK74g.PNG/007.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTE2/MDAxNzQ0NTQ3MDk5MzMz.fNJRQwXprVAtPqz8cXAnDHxG5G9yyL4MXt9MEwFNTOog.tmByOopXbcF9W3QKPl-9oVDlCWzh1QTnr5HpBabx2BMg.PNG/008.png?type=w1600)  

- 업무영향분석(BIA) 단계에서 데이터 복구 목표 시점인 RPO와 업무 복구 목표 시간인 RTO 등의 핵심 지표를 도출  

나. DRS 구축 시의 핵심 고려사항 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNDEg/MDAxNzQ0NTQ3MTg5NTc4.KS_5s-4G7BO2uH8W0ud1XsuGrILVznswCpnkbeR05Ogg.nazXtJSZ9zZjI1K0TUIZv5oEv9CznT2QCupQ_Dc9RCkg.PNG/009.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjAg/MDAxNzQ0NTQ3MTg5NTY5.523MuqSDDFNOWp7hKVqZH-98V2q2nqaSY3r92mK25BIg.ZHrRPcbiaiPBbsV7UlblvrTBr8G_Z1py7Kic_VbXW18g.PNG/013.png?type=w1600)  

- 각 업체별 상황에 맞는 RPO, RTO를 산정하여 이에 따른 운영 형태, 복구 수준, 위치 선정 등을 함으로써 효과적인 TCO 절감 가능  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjAx/MDAxNzQ0NTQ3MjI1NTkx.UngN-pLxDTJv4t54PmVbXY9-_jIDo4IxPtULmR0NuZAg.q0epDThejo_x5I04mCUzy5tYliGBdIXdxv_tmVC5qZcg.PNG/014.png?type=w1600)  

### OSI 7 계층(Layer)에 대하여 계층별 다음 사항을 설명가. 기능나. 프로토콜 종류다. 데이터 종류라. 주요 장비

**[리드]**  

ISO7498, OSI 7 계층  

**[개념]**  

네트워크의 충돌 문제등의 완화를 위해 ISO에서 표준화된 네트워크 구조를 제시한 개방형 시스템 상호연결 국제표준 모델  
(계층 구분)  
- 상위 계층: - Application 계층, Presentation 계층, Session 계층 / - 데이터의 형식이나 세션 관리 등의 고수준 네트워크 기능 처리  
- 하위 계층: - Transport 계층, Network 계층, Data Link 계층, Physical 계층 / - 데이터 전송을 위한 하드웨어적, 기술적 세부 사항을 처리  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNjAg/MDAxNzQ0NTQ3Mjg1Njkx.ZR_aio_nv7OMAsrSF-q6ziAh1kY32hDkAkzka0cPkJ4g.wr4wkoh4FDto8qFQ84DM9VNzjKjrx1ovVYZjdPdhBesg.PNG/015.png?type=w1600)  

- 각 계층의 기능 및 프로토콜 분리로 계층간 상호 운용성 및 상호 독립성을 제공  

OSI7 7 계층의 기능 및 프로토콜 종류  

가. OSI 7 계층의 기능  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfNzIg/MDAxNzQ0NTQ3MzUyMDAy.eex7ISZQnCZYNhiascjfVjRCWZbj5wXyednBsE8_Hq8g.rzYryf2cTC3hhKUHZoyCcw1CMvuJ0HKq9Kg3EmwZJuog.PNG/016.png?type=w1600)  

나. OSI 7 계층의 프로토콜 종류  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTUw/MDAxNzQ0NTQ3Mzg3MjAy.H20eYrGmJLvpROLvz4FE3V713zM_LEe4VfFxhONRWuIg.Pi_kAzRF8laijZWaYpSEccNSIp9yszIJ1pjqn-yPcgIg.PNG/017.png?type=w1600)  

OSI 7 계층의 데이터 종류와 주요 장비  

가. OSI 7 계층의 데이터 종류  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjQ2/MDAxNzQ0NTQ3NDU3MDY4.E8B7ROS0CQP6yEJH5Qj1Od0ooek1JvL8egMUXB3nx1kg.hNt2yCR-3gxKT5afCQzNGr3BYZhoR_XPj0534T93kgkg.PNG/018.png?type=w1600)  

나. OSI 7 계층의 주요 장비  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMjk3/MDAxNzQ0NTQ3NDg5OTcw.4S5h0ovgUX7ihW86G2-oADgDARyw803657g3GjTGNn4g.sbgPxVww3UKr6QURFphPGIT1Atadzb5DCoFjtWd7U4Ug.PNG/019.png?type=w1600)  

Service Primitive  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTNfMTU5/MDAxNzQ0NTQ3NTI5ODYw.gy8tdeMkiVvUAi1vL5uVUaDZSWqMC_Wuj0w7aEuEz4Ag.Jp-vqspX3dTd_r-q0I_HT3EfZUZfuFUkNDx83PC0sNEg.PNG/020.png?type=w1600)  

- 데이터 전송 전 연결 설정 여부에 따라 연결형 서비스, 비연결형 서비스로 구분 가능  

### 최근 많은 범죄들이 지능화, 고도화 되면서 디지털 포렌식의 중요성이 증가하고 있다. 이러한 디지털 포렌식과 관련하여 아래 사항을 설명가. 디지털 포렌식의 개념나. 디지털 포렌식의 유형과 절차다. 디지털 포렌식 기술 및 활용분야

**[리드]**  

지능화, 고도화 된 범죄에 대한 법적 증거 확보, 디지털 포렌식  

**[개념]**  

컴퓨터를 이용하거나 활용해 이뤄지는 범죄 행위에 대한 법적 증거 자료 확보를 위해 컴퓨터 시스템, 네트워크 등 가상 공간의 자료가 법적 증거물로 법원에 제출될 수 있도록 확보하는 일련의 절차와 방법  
- 원칙: 정당성, 재현, 신속성, 연계 보관성(Chain of Custody), 무결성의 원칙  
- 과정의 명확성, 추적성, 무결성, 책임성이 있어야 정당성 확보  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMTcy/MDAxNzQ0NjM3MDk5ODE1.PyYE7EsTlZ7u5l5BLSk79kvDhkekOR8xgO77UxztLR0g.v9NEe5IKTDl3vx6Q_SCxoRs3KUVluJv8f6N4Hm3TSkYg.PNG/031.png?type=w1600)  

디지털 포렌식의 유형과 절차  

가. 디지털 포렌식의 유형  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMjEw/MDAxNzQ0NjM3MTgzMTU4.5k0NhZFbc2Ctrg_P_MQQtccHonXh0Jtvorjn61c1cTog.ubGvj14ZsN775BEaSUXoC4Lz6GSGkEo0ESEYa11I8fcg.PNG/001.png?type=w1600)  

나. 디지털 포렌식의 절차  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMjUy/MDAxNzQ0NjM3MjQ4OTM5.kIXA6NrBbmjJREkWQZifQn2Kqn-AWZrlB_uwl8pSoTAg.hpp5iPGiHS7-PcEM7QoxbE0yfdGN2PsswG6z3BKjPpog.PNG/002.png?type=w1600)  

- 디지털포렌식 절차에 맞춰 수집 및 분석, 제출해야 원칙 보장  

디지털 포렌식 수집 및 분석 기술  

가. 디지털 포렌식 수집기술  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMTE3/MDAxNzQ0NjM3MzA4MTE0.u-_7xkUs1Qs8QIiCMv_MUnjKFsjYI0kMD1OcP1cuPSEg.IhWSbTkD5MvFbK0O48Pq2EqpFeOwvpD716BbcrHbK0kg.PNG/003.png?type=w1600)  

나. 디지털 포렌식의 분석 기술  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMjMw/MDAxNzQ0NjM3NjI2MDQ4.GQhVu9bcEF4fJrDc7eGQKnMX5oT7kuWzAs3RxSUmdrsg.fC-TO6RQJ03nSBeONHwrT27C-9lPAG37Dgl7Qi_IGlsg.PNG/004.png?type=w1600)  

- 디지털 포렌식의 수집 및 분석 기술을 통해 각 분야에서는 범죄 조사, 데이터 분석, 보안 대응, 법적인 대응 등 다양한 목적에서 활용  

디지털 포렌식 활용분야  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMjI4/MDAxNzQ0NjM3NzI0NDcy.dx7JnZDOAmDWWZJzo6tDYaVf9swYdaUUWr_7g3E1Bo0g.JgnaK4YFYJkk0N04Pgi9Z9SPYsrHVBvVxI918aizgJ8g.PNG/006.png?type=w1600)  

- 최근 인공지능을 활용한 범죄가 증가하고 있어, 윤리적 준비와 더불어 디지털 포렌식 분야에서의 기술 주목  

### 리팩토링(Refactoring)가. 정의, 목적, 리팩토링 순서, 리팩토링 주요기법나. 코드스멜(Code Smell)의 정의와 특징다. 코드스멜의 종류를 3개 이상 기술하고 각각의 리팩토링 방법

**[리드]**  

내부 구조 개선 및 가독성 향상, 리팩토링(Refactoring)  

**[개념]**  

SW의 유지보수 및 개발 생산성을 향상하기 위해 외부로 보이는 동작의 변화 없이 내부 구조를 개선하는 기법  

**[상세설명 및 해결방안]**  

리펙토링의 정의, 목적, 리팩토링 순서, 리팩토링 주요기법 설명  

- 정의: SW의 유지보수 및 개발 생산성을 향상하기 위해 외부로 보이는 동작의 변화 없이 내부 구조를 개선하는 기법  

- 목적  

. 디자인 개선 : 설계의도와 구현 코드의 일관성 유지하기 위한 설계변경 용이  

. 이해도 향상 : 이해하기 쉬운 코드는 개발자 작업시간을 단축  

. 오류발견 용이성 확보 : 소스 구조를 명확히 함으로써 버그 원인 쉽게 발견  

. 개발 생산성 향상 : 좋은디자인 -&gt; 개발자 이해 향상 -&gt; 오류감소,개발 가속화  

- 순서  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMTA5/MDAxNzQ0NjM3Nzc3Mjc0.xOaKjvXxPfiw1FXW3iXW0fE4BzX6D9-F00cP-duzRT8g.7W5kKhzsKY_2f7wWUs6tzKQ6_Saok-SkctHNOiz5U9Qg.PNG/007.png?type=w1600)  

- 주요기법  

Extract Class/Method: 하나의 클래스에 다양한 Role 존재할 경우, 명확한 단위로 클래스/메소드 분리  

Push Down Method: 슈퍼 클래스의 메소드나 속성이 서브 클래스 일부에만 관련된 경우,해당 메소드나 속성을 서브클래스로 이동  

Move Method: 타 클래스와 결합도가 높은 메소드 해당 타클래스로 이동  

Move Attribute: 클래스의 속성을 다른 클래스가 더 많이 사용한는 경우,해당 클래스로 이동  

Self Encapsulated Field: Field 참조 시 정해진 규칙에 의해 접근,Public 접근제어를 Private으로 변경  

Decompose Condition: 복잡한 조건식을 작은 조건들로 분해  

코드스멜(Code Smell)의 정의와 특징 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfNzUg/MDAxNzQ0NjM3ODMwODUw.Urpvu5I-D17a6uWyKOOizdjju8_JB0CR9NIDXEnkc0Qg.4g5snGp73SpqTFwGYU6szhnDwz0p-mrx2c-he9oYeOUg.PNG/008.png?type=w1600)  

- 정의: Kent Beck에 의해 처음 제시되어 프로그램 가독성이 나쁘고 중복된 로직을 포함하는 등 코드품질을 저하시키는 요인(ex-길다, 많다, 겹쳐있다, 이름이 어색하다, 객체지향적이지 않다 등). 개발자가 이해하거나 유지보수하기 어려워 리팩토링의 대상이 되는 코드  

- 특징  

. 응용 프로그램 수준의 스멜: 중복 코드, 억지로 꾸민듯한 복잡성  

. 클래스 수준의 스멜: 커다란 클래스, 기능에 대한 욕심, 부적절한 관계, 거부된 유산, 게으른 클래스, 리터럴의 과도한 사용, 순환 복잡도, 다운캐스팅, 고아 변수 또는 컨스턴트 클래스  

. 메서드 수준의 스멜: 너무 많은 매개변수, 긴 메서드, 과도하게 긴 식별자, 과도하게 짧은 식별자, 과도한 데이터의 반환  

코드스멜의 종류 3개 이상 기술 및 리팩토링 방법 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMjkg/MDAxNzQ0NjM3ODkyOTQ2.POwNGnHXG1_yyHZWMlEybtcFB_7SRQ4m1m2cYgWC5r4g.W-cYIqnENiA3QvLtN8LOohTHumsNkpckPrHWHHy73TYg.PNG/009.png?type=w1600)  

- SW의 안전성, 신뢰성, 재사용성 확보위해 리팩토링이 필요하며, 리팩토링 지원도구의 적절한 활용이 필요하지만 무엇보다 전문가의 안정적인 설계와 code inspection 능력 필요  

### SOAP(Simple Object Access Protocol)와 REST(Representational State Transfer)를 비교 설명

**[리드]**  

OpenAPI 아키텍처, SOAP과 REST  

**[개념]**  

SOAP : 웹 서비스 간 데이터를 교환하는 XML 기반 프로토콜  

REST : HTTP 프로토콜을 기반으로 자원을 주고받는 아키텍처 스타일  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMjQg/MDAxNzQ0NjM3OTU1NTg0.Wi5sZQ45L2pbmOgziiUKQSL2pnje9qMxFtm-k7xo7uUg.YUagr_rFFDAm7gRhUcVN1M_POrNwtOO3NWdD5uYdBm8g.PNG/010.png?type=w1600)  

- SOAP은 엄격한 표준을 준수하므로 보안, 트랜잭션이 중요한 환경에서 사용, REST는 가볍고 빠른 모바일 API개발에 최적화되어있음  

SOAP과 REST 상세 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfMTk5/MDAxNzQ0NjM4MDIwMzY3.qwRe7AL4JUoAWgWpZL1P3bQZEJDIOBH6g5r76mOa5Owg.3AX8tT60wyXjpTVeXN5aA2lKQBS7zmYXLIxJFr8z_5Ag.PNG/011.png?type=w1600)  

- Open API 사용시 서비스 접근제어를 위해 OAuth2.0 기반으로 사용자 인증필요  

Open API 사용시 OAuth2.0 적용방안  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTRfNjkg/MDAxNzQ0NjM4Mjc2NDA5.WN-9a76_Tv0Lt-AuIEzDbMf34ic30TOyZ3B5pZbf7lMg.NbhacrR9kG9Q-4Wp1FRDD8yHHDzXbOCz9mBXDioGaDYg.PNG/012.png?type=w1600)  

- Open API 사용 환경에 따라 권한코드 부여, 클라이언트 자격증명, 디바이스 인증 등 인증방식 선택 필요  

### Canary Test

**[리드]**  

무중단 배포 위한 사전 테스트, Canary Test  

**[개념]**  

새로운 기능이나 업데이트를 일부 사용자 그룹에 먼저 적용하여 시스템의 안정성과 성능을 확인하는 테스트  

- 목적 : 변경 사항의 안정성 및 성능 검증  

--&gt; MSA 환경에서 Canary test는 무중단 배포와 안정적인 업데이트를 위해 필수과정임  

**[상세설명 및 해결방안]**  

Canary Test 절차 및 주요기법  

가. Canary Test 절차  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTk5/MDAxNzQ0NzI5OTAwODg2.IS8K8Xm-BzGoMrP7HoPS-wIn-i8UnoDkHXftqgUmaNog.H8sHiFGNSi641g4lrl9cohhPh_fXTuDuHGiG5SbSTncg.PNG/001.png?type=w1600)  

- Canary test 후 Canary 배포 또는 블루-그린 배포 진행하여 리스크를 최소화할 수 있음  

나. Canary Test 주요 기법  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTc4/MDAxNzQ0NzI5OTM1NjQx.IDILWS8xPZGWDZ-CSd247kaS4sUViKv-5HNYuG83Ztog.fuUaKRbrXvhlcBvwsUBY74X3Y7fquwr2PLTc6dsjGtIg.PNG/002.png?type=w1600)  

- Canary Test는 배포 전에 기능 안정성 검증 테스트에 중점을 두고, Canary 배포는 배포에 중점을 둠  

Canary Test 장점 및 단점  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfNDEg/MDAxNzQ0NzMwMDAwMTIz.0f3_YJbvoXwnk5Wqp81x73RIKk7mU7-kKwnoSjfL1iUg.z7dl2Q5kArmMcxEVBPPaWmm3pCzKsUBiw1viOvQJcVEg.PNG/003.png?type=w1600)  

- Canary Test는 배포 후 문제 발생 시 즉시 롤백이 가능하여 리스크 최소화하고, MSA 환경에 적합함  

Canary Test와 Canary 배포 비교  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMzMg/MDAxNzQ0NzMwMTA0Mzcx.jQvoMcMRhqxkIgGHcldsBoOBxtctQfptzyyWZKQ1ROAg.JFFvdxT6oUxXLfwkYCLcFlWf9sC-SyIJMPpGS14oERgg.PNG/004.png?type=w1600)  

### 소프트웨어사업 영향평가

**[리드]**  

민간투자형 SW사업 보호, 소프트웨어사업 영향평가  

**[개념]**  

공공기관이 SW사업을 추진할 경우 민간 시장에 미치는 영향을 사전에 분석해 결과를 과기정통부 장관에게 제출하게 하는 제도  
- 목적 : 공공 정보화 사업의 기획단계부터 민간시장에 미치는 부정적 영향을 평가  
- 근거 : 소프트웨어 진흥법43조 (공공 SW사업의 민간 시장 영향 분석)  
-→ 민간 소프트웨어 기업 경쟁력 확보를 위해, 2023년 10월 소프트웨어 영향평가제도 개정하여 발표함  

**[상세설명 및 해결방안]**  

소프트웨어사업 영향평가 상세 설명  

가. 소프트웨어사업 영향평가 대상기관 및 사업  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjAy/MDAxNzQ0NzMwOTQ0OTM2.6ou8_Qvw-3WQmRES0N5X6FK2BxCeZAKWK9RKc_DqD-8g.jUs42aqTS8XjaQqN3ID8tg91rXyzlPnRdrg5lQJS28Eg.PNG/005.png?type=w1600)  

- 상용 소프트웨어, 국가 안보 관련, 민간투자사업, 특정 목적 사업용인 경우는 제외함  

나. 소프트웨어사업 영향평가 항목  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTU1/MDAxNzQ0NzMxMDA2NDc4.JT5Yb5El7DQ3Mt7yNhWCVehe1UWclwxga0oRXvp-i9gg.JphDZUJCDtqJQdHrxGG4FZu6e7B0L8H7Ksm0ya65pSog.PNG/006.png?type=w1600)  

- 민간 소프트웨어와의 유사성, 민간 소프트웨어 시장 침해가능성과 소프트웨어사업의 필요성ㆍ공공성을 종합적으로 평가함  

소프트웨어사업 영향평가 시기  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTgx/MDAxNzQ0NzMxMDM0MzE4.T53L5xFXu28-7XF-zI1l8XBgmoBu3o4iZGE6TzeS0rcg.vxx2FZ1UU8cpSS6c2JFKQ63EMlmsD_FYXuZacd9zaE0g.PNG/007.png?type=w1600)  

- 각 단계별 영향평가 후 결과서 제출 및 침해 여부 없는 경우, 다음 해 지능정보화 예산 편성 시 반영함  

### NoSQL의 CAP(Consistency, Availability, Partition Tolerance)

**[리드]**  

분산 시스템의 DBMS 이론배경, NoSQL의 CAP 이론  

**[개념]**  

분산 데이터베이스가 갖춰야 할 일관성, 가용성, 파티션 허용성 3가지 특성 중 두가지 특성만 만족할 수 있다는 이론  

대용량 분산 데이터 저장소는 데이터 일관성(Consistency), 가용성(Availability), 단절내성(PartitionETolerance)을 모두 만족시키는 것이 불가능하므로 두 가지만 전략적으로 선택해야 한다는 이론 (DBMS 선정을 위한 이론적 배경)  

**[상세설명 및 해결방안]**  

CAP 이론의 요소  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfODYg/MDAxNzQ0NzMxMTQwMTk5.zdMItCBEEHlPQ_umyybODqLsSzQ6276w7UzlQyS1p6gg.czv5o4unrOura4dfKK_997a6IDRsBf3ZviK8pLkAvCsg.PNG/008.png?type=w1600)  

- 네트워크 파티션 상황에서 일관성(CP)와 가용성(AP) 둘 중 하나만 만족할 수 있음  

CAP 이론의 구성도 및 구성요소  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfNDEg/MDAxNzQ0NzMxMTg5ODcy.m6wgE_6AS9KQbPEmxWBW12zzAyGYxl0ZHD5yK77BYlEg.HOiCY2cBvv406r5jNik2EnGejusWNdHm6_FpzVP63_og.PNG/009.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjk5/MDAxNzQ0NzMxMTk2MzMw.j40QrO3cOFYRUumZHM2Qsky9KSuoMq3RD1B40d9QX14g.MQQWGwxc9IDTprB62g1VSqDnn7i2xKoGv6drM7E3umAg.PNG/010.png?type=w1600)  

- CAP이론은 파티션 허용성에 대한 명확한 정의 부족, 완벽한 CP 또는 AP시스템은 없다는 한계가 존재함  

CAP이론의 한계 극복, PACELC 이론  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMzAw/MDAxNzQ0NzMxMjY2ODMz.n21oljPgPDTjVrI06oLxMa0vEv292gxKNOufPD4m4hcg.eAcGDjfYVHxJPJS3DWkKKnNzeMN0WE8caT9ws2461Asg.PNG/011.png?type=w1600)  

- PACELC 이론은 CAP 이론의 단점을 보완하기 위해 네트워크 장애 상황과 정상 상황으로 나누어서 설명하는 이론  

- 장애 상황, 정상 상황에서 어떻게 동작하는 지에 따라 PC/EC, PC/EL, PA/EC, PA/EL로 분류 가능  

### 군집분석 기법인SOM(Self Organizing Map)가. SOM 정의 및 특징나. SOM 구성요소다. SOM과 신경망 분석기법의 차이점

**[리드]**  

자기조직화 지도 인공신경망 모델, SOM  

**[개념]**  

대뇌피질의 시각피질 학습 과정을 모델화 한 인공신경망으로, 자율학습에 의한 클러스터링을 수행하는 알고리즘 (Kohonen map 이라고도 함)  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfNzkg/MDAxNzQ0NzMxMzU1MTcx.FRHrca3xgeRoGl8el-yHCD7UJCT7nIVcMRUl7LrPl4Qg.Jv6q_IPSEJcIQdl9fdM2Pi56gpKIoLrxzkRJDwS0HiQg.PNG/012.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjU1/MDAxNzQ0NzMxMzU1MTkx.cph1IdS_3T8KvUJkg2a-KkgjKqqiLpRHNuToOX0hhUIg.bQWpNQjuJ6K96HkBEsI7wX_wuxEOUZoza4xpAZd7iikg.PNG/013.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjkz/MDAxNzQ0NzMxMzU1MjA2.8sAGAJqRVWoXF4sfGiSJHnfirmGmR0ozRWbRVXFeMzcg.IrA--p8HlD1IQ95F3ETgxxXOJQBPQjCmL1MQ1XhyFmYg.PNG/014.png?type=w1600)  

### 운영체제에서 발생할 수 있는 deadlock 현상가. deadlock의 개념나. deadlock과 starvation의 차이점다. deadlock이 발생하기 위한 조건 4가지라. deadlock 발생 시 처리 방안

**[리드]**  

프로세스의 점유 요청에 따른 무한 대기 문제, Deadlock  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjk2/MDAxNzQ0NzMxNDI4ODI1.zZaMExc5aMg3Gpz2u2ZMUGXbD5d21yojcjwbazG8Cpog.itZrzdv41ecpQ1IbaczQMXOFWToegOtLvKeZB8rvX8og.PNG/015.png?type=w1600)  

- 서로 점유하고 있는 자원을 요청하여 자원사용이 끝날 때까지 process 점유하여, 자원할당을 계속 대기하는 점에서 starvation과 동일  

deadlock과 starvation의 차이점 설명  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjMw/MDAxNzQ0NzMxNDkyMDU1.hxjT_4s2OgvroAhHVlBc4gBSIeHOgI7coJonwukXtiMg.W9vmQFIfIRLv-9V69FoZ0jtBbjtr31_qXQfG46Voec4g.PNG/016.png?type=w1600)  

- deadlock은 blocked 상태에서 절대 발생하지 않는 이벤트를 대기하고 있으므로, 해결하기 위해 4가지 발생 조건 중 하나 이상 부정 필요  

deadlock이 발생하기 위한 조건 4가지 및 처리 방안  

가. deadlock이 발생하기 위한 조건 4가지  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjE1/MDAxNzQ0NzMxNTU0MDk5.SqnywnQL6PYsbV5FsvaCA5Xo8p6SCMdVmsQebGCi2T8g.SGHLcQHn8wWkvOGB6ihPAM1YjfnYabA8GFpck74daTwg.PNG/017.png?type=w1600)  

- 상호 배제, 점유와 대기, 비선점, 환형 대기 조건이 동시에 발생 시 deadlock 상태가 되며, 이중 하나라도 부정 시 해결 가능  

나. deadlock 발생 시 처리 방안  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTUx/MDAxNzQ0NzMxNTg4ODAw.eH2iseJsxPmr3SKmjXZn4EgAKdJc1OYCCsN4FKE_Glog.rr5giFVFVupmPTQZDNU46xMFg0UH50P2_Rbvg_2VOIIg.PNG/018.png?type=w1600)  

- deadlock 발생 전 사전 처리가 효과적이며, 은행가 알고리즘을 사용함  

교착상태 회피 알고리즘, 은행가 알고리즘(Banker's Algorithm)  

- 정의 : 운영체제는 자원의 상태를 감시하고 사용자 프로세스는 사전에 자기작업에서 필요한 자원의 수를 제시하는 교착상태 회피 알고리즘  

- 안정 상태(Safe State) : 프로세스 별로 요청한 자원을 할당할 수 있고, 교착상태를 방지할 수 있는 상태  

- 불안정 상태 (Unsafe State) 교착상태가 발생할 수 있는 불안정 상태, 프로세스 별로 요청한 자원 할당 불가  

--&gt; 사용가능한 자원 수와, 프로세스 별 최대 요구 수를 고려하여 구현  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTcy/MDAxNzQ0NzMyMjczMTQx.rszUXhI3mUVLWN6LGlOiSCPCJfhq6mCBw_ITsQHgH6Ig.KtBX419BT3-R_qTij7Ty-duLiYES6M_9MM7nMV502VAg.PNG/019.png?type=w1600)  

### 영지식 증명(zero-knowledge proof)의 개념 및 등장배경, 충족조건, 원리, 블록체인 산업에서의 영지식 증명 활용사례에 대하여 설명

**[리드]**  

완전성, 건전성, 영지식성, 영지식 증명(zero-knowledge proof)  

**[개념]**  

사전적 : 거래 상대방에게 어떠한 정보도 제공하지 않은 채, 자신이 해당 정보를 가지고 있다는 사실을 증명하는 기술  

일반적 : 프라이버시 문제를 해결하는 암호학적 방법으로 사전 정의된 연산에 대해 비밀 입력 값은 공개하지 않으면서도 입출력 값의 관계에 해당하는 비밀 입력 값을 알고 있음을 증명하는 암호 기술  

**[상세설명 및 해결방안]**  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMjgw/MDAxNzQ0NzMyMzY5NTk4.nZrLOhZM6s6l9OCRHwtjgR6ZDUmUL64sn-u7EolTB3Yg.Bbk-HDLLEPvCGmtrD3pdFX-D9bs3grU9kpKk1ZjRccMg.PNG/020.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTgx/MDAxNzQ0NzMyMzY5NTY2.pcOee9giQTt5VWa_FaZXDHBlZk-dMKHIIpYq44jBrAIg.pve5D4vaVW16NIeJpnv3fcsiJawSA1zhg_80RLLt5AMg.PNG/021.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfODYg/MDAxNzQ0NzMyMzY5NTk3.qJTLcrL0dl4YqdhwUogKx8avW86ULKz78y1-hbLB9Csg.91GGrv-qtYlbQWxUz5XQtYQfqBvblba5w7g7RISvPBkg.PNG/022.png?type=w1600)  

![image](https://cafeptthumb-phinf.pstatic.net/MjAyNTA0MTZfMTQg/MDAxNzQ0NzMyMzY5NTcw.IcMYu641ZOu5up3k3h9Pz2mpiGhthair2fMZr3m3B0gg.idFqh84kNvfxe0TxAzdiaQ4aTfhtU_ILfk0W-9nNXc4g.PNG/023.png?type=w1600)  

