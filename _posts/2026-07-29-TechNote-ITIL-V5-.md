---
layout: post
title: "TechNote(ITIL V5)"
date: 2026-07-29
categories: technote
tags: [technote]
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

### [경영컨설팅(MA)] ITIL V5

**[상세 내용]**  

**ITIL V5의 등장 배경과 핵심 변화**  

2019년 발표된 ITIL V4는 업무 프로세스의 디지털 전환과 클라우드 중심 환경에 대응하기 위해 기존 ITIL V3를 대폭 재정비한 버전이었습니다. 그리고 7년 만인 올해 ITIL V5가 등장했습니다. 그동안 AI 기술의 급격한 발전과 디지털 제품 중심 운영 모델 확산으로 인해, ITIL V4만으로는 최신 환경을 충분히 설명하기 어려워졌기 때문입니다. 기존 ITIL의 강점을 유지하면서 AI 기반·디지털 제품 중심 환경에 맞춰 발전된 새로운 ITIL V5에 대해 알아보겠습니다.  

**1. AI 시대의 도래로 인한 요구 변화**  

AI는 더 이상 단순한 분석 도구가 아니라 **의사결정 과정의 핵심 구성 요소**가 되었습니다. 서비스 수요를 자동으로 계산하고, 운영 리스크를 AI가 실시간으로 평가하는 등 이제 조직은 “사람이 판단하고 AI가 보조하는 구조”에서 “AI가 판단하고 사람이 검증하는” 구조로 이동하고 있습니다.  

AI와 자동화는 운영 모델 자체를 바꾸고 있습니다. ITIL V4는 자동화를 강조했지만, AI가 운영을 주도하는 수준의 자동화를 전제로 설계된 프레임워크가 아니었습니다. AI 시대의 AIOps는 사람이 운영하는 시스템에서 **AI가 운영하고 사람이 감독하는 시스템**으로의 변화를 끌어냈습니다.  

AI가 의사결정에 관여하는 순간, 조직은 아래와 같은 새로운 책임을 가지게 됩니다.  

- ㆍAI가 왜 그런 결정을 내렸는지 설명할 수 있어야 함  
- ㆍ데이터 편향을 관리해야 함  
- ㆍAI 모델의 오작동·오판에 대한 통제 체계 필요  
- ㆍ규제 준수(개인정보보호법, 자동화된 의사결정 규제 등)  

ITIL V5는 이 **AI 거버넌스**를 핵심 구성 요소로 포함하고 있습니다.  

AI는 서비스 자체의 구조가 바뀌는 데에도 큰 영향을 주었습니다. 이제 서비스 설계와 운영은 더 이상 단순한 IT 서비스 관리가 아니라, AI 모델 관리, 데이터 관리, 서비스 관리가 **하나로 결합된 형태**로 나타나고 있습니다.  

ITIL V4는 AI 시대가 불러온 새로운 AI 중심 의사결정 체계, AI 주도적 자동화 체계, AI 거버넌스, 그리고 AI 기반 라이프사이클을 설명하는 데 구조적 한계를 가지고 있었습니다. ITIL V4는 클라우드와 디지털 전화 중심의 시대를 반영했지만, 기업들이 AI를 통해 업무 전반을 재편하는 시대로 인해 새로운 지침인 ITIL V5가 등장하게 되었습니다.  

**2. 제품 중심(Product-centric) 운영 모델 확산**  

ITIL V4는 서비스 중심(Service-centric) 모델이 기반인 서비스 가치 시스템(SVS)을 중심으로 작성됐습니다. 하지만 오늘날의 경영 환경은 **서비스와 제품을 통합해 하나의 디지털 경험을 제공**하는 방향으로 나아가고 있습니다.  

ㆍ디지털 제품의 라이프사이클 관리  

- ㆍ제품과 서비스의 통합 운영  
- ㆍ고객 경험 중심의 가치 흐름 관리  

이러한 변화에 맞춰 ITIL V5는 제품과 서비스를 하나의 엔드-투-엔드 라이프사이클로 통합해 관리할 것을 제시합니다.  

![image](https://steg.co.kr/upload/editor/1dd211a2d77333c569727effa5c66754_d16cd.png)

발견 → 기획 → 획득 → 구축 → 전환 → 운영 → 조달 → 지원 8단계로 구성된 라이프사이클은 제품과 서비스가 하나의 가치 제공 체계 안에서 어떻게 움직이는지 설명하고 있습니다.  

**3. 복잡성 증가와 민첩성 요구**  

ITIL V4도 당연히 민첩성을 강조했습니다. 하지만, AI 기반 환경에서는 더 높은 수준의 적응력과 실험 기반 운영이 필요합니다. ITIL V5는 이러한 요구를 반영해 예측이 불가능한 환경에서 프로세스를 유연하게 조합하고 변화시킬 수 있는 **복잡성-네이티브** 프레임워크로 설계되었습니다.  

오늘날의 조직은 불확실하고 변동이 크며 복잡하고 모호한(VUCA) 환경에 직면해 있습니다. ITIL V5는 이러한 환경을 전제로 예측할 수 있는 계획 중심이 아니라, 실험·학습·적응이 기본인 전략을 제시하고 있습니다.  

ITIL V5는 AI·자동화·디지털 제품 중심 운영이 기본값입니다. 이는 ITIL V5가 복잡한 시스템을 단순화하기보다는 복잡성을 관리하고 활용하는 능력에 더 초점을 맞추고 있다는 것을 보여줍니다.  

ITIL V4가 실천(practices)을 명확하게 규정하고 있었다면, ITIL V5는 그 실천과 가치 흐름(value chain)을 유연하게 적용하고 있습니다. ITIL V5의 복잡성-네이티브 프레임워크에서는 고정된 프로세스가 아니라, 상황에 맞게 민첩하게 프로세스를 조합하고 변화시키는 능력이 중요해졌습니다.  

![image](https://steg.co.kr/upload/editor/ITILV4V5_734bb.png)

**4. ITIL 4 → ITIL 5: 진화의 핵심 요약**  

&nbsp;ITIL V4에서 ITIL V5로의 변화는 위와 같이 요약할 수 있습니다. 이러한 변화는 ITIL V5의 새로운 교육 커리큘럼에서도 확인됩니다. 가치 사슬(Value Chain) 모델은 단순해졌으며, 방대했던 34개의 실천(Practices) 사례들은 새로운 8단계 라이프사이클로 설명이 가능해졌습니다.  

ITIL V5는 AI로 인해 예측 불가능해진 업무 환경, 그리고 제품·서비스를 통합하여 운영하는 시대상을 반영하고 있습니다. 급격하게 변화하는 현시대에 더 민첩하게 대응할 수 있는 ITSM의 초석이 되리라 기대합니다.  

