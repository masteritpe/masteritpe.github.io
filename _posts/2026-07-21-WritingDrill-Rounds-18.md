---
layout: post
title: "WritingDrill_Rounds_18"
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

### [3년치 기출, KPC 모의고사] 양자머신러닝(QML, Quantum Machine Learning)

**[정의]**  

- 양자컴퓨팅의 원리(중첩,얽힘,간섭)를 활용하여 머신러닝 알고리즘을 고도화하는 기술  

**[핵심/키워드]**  

&lt;기술요소&gt;  
* QSVM : 양자 커널과 특징맵을 활용한 고차원 데이터 분류  
* QRL : PQC 기반 정책·가치함수 근사를 통한 강화학습  
* QAOA : QUBO/Ising 기반 조합 최적화 알고리즘  

### [3년치 기출, KPC 모의고사] 소프트웨어 무중단 배포 방식

**[정의]**  

- 서비스가 중단되지 않은 상태로 새로운 버전을 사용자에게 배포하는 기술  

**[핵심/키워드]**  

&lt; 유형 &gt;  
* Rollingk Deployment , Blue-Greenk Deployment , Canaryk Deployment  
* 리버스 프록시와 로드밸런싱 기술을 활용해 무중단 배포 구현 가능  

### [3년치 기출, KPC 모의고사] 중심극한정리

**[정의]**  

- 모집단으로부터 추출된 표본의 크기n이 충분히 크다면(30이상)  표본 평균들이 이루는 분포는 정규분포에 수렴한다는 원리  

**[핵심/키워드]**  

&lt; 특징 &gt;  
* 정규 분포 근사화 , 추론의 강화 , 표본 크기의 영향 , 표본 추출 유연성 , 실험의 재현성  

### [3년치 기출, KPC 모의고사] ADAS(Advanced Driver Assistance System)

**[정의]**  

- 운전자가 차를 안전하게 운전하여 목적지까지 무사히 도착할 수 있도록 돕는 기술  

**[핵심/키워드]**  

&lt;기술요소 및 특징 &gt;  
* 카메라, LiDAR, Radar  
* 단일 센서 위주 구성, 사고 예방 및 편의 제공, 사고 시 사람 책임, Fail-Safe  
* 자율 주행 단계 0~2단계  

### [3년치 기출, KPC 모의고사] 개인정보보호 강화를 위한 가명처리

**[정의]**  

- 개인정보의 안전한 활용 위해 개인정보의 일부를 삭제하거나 대체하여, 추가 정보 없이는 특정 개인을 식별할 수 없도록 만드는 과정  

**[핵심/키워드]**  

&lt;가명처리 기술&gt;  
삭제, 부분 삭제, 행항목삭제, 로컬삭제, 마스킹, 총계처리, 부분총계, 일반라운딩,  
 랜덤라운딩, 제어라운딩, 상하단코딩, 로컬일반화, 범위방법, 문자데이터범주화,  
양방향 암호화, 일방향 암호화, 순서보존 암호화, 형태보존 암호화  

### [3년치 기출, KPC 모의고사] AI 리스크

**[정의]**  

- 인공지능의 개발·활용·관리 전 과정에서 발생할 수 있는 잠재적 손실이나 부정적 결과  

-AI시스템의 개발·학습·배포·운영 과정에서 개인,B조직,B사회에 부정적 영향을 줄 수 있는 불확실성 또는 위험  

**[핵심/키워드]**  

&lt; AI 리스트 종류 &gt;  
* AI모델자체 : 모델탈취, 적대적 공격, 모델 포이즈닝, 과적합 취약성, 프롬프트 인젝션  
* AI 학습데이터 : 데이터 유출, 데이터 위변조, 데이터 포이즈닝, 편향데이터주입  
* AI 활용연계과정 : API 취약점 악용, 서비스거부공격(DOS/DDOS), 추론과정 민감정보 노출  

### [3년치 기출, KPC 모의고사] WBS

**[정의]**  

- 프로젝트 목표를 달성하기 위해 수행해야 할 전체 작업 범위를 산출물 중심으로 계층 구조로 세분화한 체계도  

**[핵심/키워드]**  

&lt;특징&gt;  
① 산출물 중심  ② 100% Rule준수  ③ MECE 원칙 적용  
④ 상세 수준은 프로젝트 복잡도와 관리 필요도에 따라 결정  

### [3년치 기출, KPC 모의고사] 대수의 법칙

**[정의]**  

- 동일한 확률분포에서 표본 수가 증가할수록 표본 평균이 모평균에 수렴함을 설명하는 확률 법칙  

**[핵심/키워드]**  

표본평균의 분포(Distribution), 정규분포라는 모양으로 수렴, 가설 검정 및 신뢰구간 산출  

### [3년치 기출, KPC 모의고사] 프로젝트 위험관리

**[정의]**  

- 프로젝트 목표에 영향을 줄 수 있는 불확실성을 식별·분석·대응·감시하는 체계적인 과정  

**[핵심/키워드]**  

* 위험 종류 :Scope Creep, 요구사항 모호성, Gold Plating, 일정 추정 오류, 선행 작업 지연, 예산 산정 누락, 핵심 인력 이탈, 설계 오류  
* 대응 전략 : 에스컬레이션 (escalate), 회피 (Avoid), 완화 (Mitigate), 전가(Transfer), 수용(Accept)  

### [3년치 기출, KPC 모의고사] 엣지(Edge) 컴퓨팅

**[정의]**  

- 데이터가 발생하는 현장 또는 사용자와 가까운 위치에서 데이터를 처리·분석하는 분산 컴퓨팅 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
* 단말·게이트웨이·로컬 서버 인근 처리  
* 초저지연 기반 실시간 처리 최적  
* 현장 데이터 선처리·필터링 중심  
* 부분 독립 운영 가능  
* 초기 투자 비용 필요 (Capex)  
* 현장 장비 구축 비용 증가  

### [3년치 기출, KPC 모의고사] 분산 데이터베이스

**[정의]**  

- 여러 개의 물리적으로 분산된 데이터 베이스가 네트워크를 통해 논리적으로 하나의 시스템처럼 동작하는 DBMS  

**[핵심/키워드]**  

&lt;목적&gt;  
① 데이터 분산 , ② 논리적 일관성 유지,  ③ 병렬 처리 , ④ 네트워크 의존성  
&lt;분산 투명성&gt;  
-위치 투명성, 분할 투명성 , 지역 투명성, 복제 투명성, 병행 투명성, 장애 투명성  

### [3년치 기출, KPC 모의고사] 과적합

**[정의]**  

- 학습 데이터에는 성능 좋지만 실제 데이터에 성능 떨어지는 현상  

**[핵심/키워드]**  

&lt; 원인 &gt;  
* 훈련 데이터 과하게 학습, 파라미터 개수 과다, 모델 복잡도 증가  
&lt; 해결방안 &gt;  
* 정규화(Regularization), 차원 축소, 교차 검증, EarlyCStopping, 모델 단순화, Dropout, 사전 학습 (Pre-trained)  

### [3년치 기출, KPC 모의고사] 과소적합

**[정의]**  

- 적정 수준의 학습을 하지 못해 실제 성능이 떨어지는 현상  

**[핵심/키워드]**  

&lt; 원인 &gt;  
* 학습 부족, 학습 데이터 부족, Feature 부족, 과도한 정규화  
&lt; 해결방안 &gt;  
* 학습 데이터 증가, 모델 복잡도 증가, Feature 추가, 정규화 완화, 알고리즘 변경  

### [3년치 기출, KPC 모의고사] 맥케이브 순환복잡도

**[정의]**  

- 프로그램의 제어 흐름(Flow Graph)에서 독립적인 실행 경로의 수를 정량적으로 평가하여 소프트웨어 코드의 논리적 복잡도를 측정하는 메트릭  

**[핵심/키워드]**  

&lt;계산 방법&gt;  
1.. 제어 흐름 그래프 생성  
1\. 노드(V),간선(E),영역(P)확인  
2\. 복잡도 수식 적용  
3\. 복잡도 분석 후 코드 최적화  
* 추가 2가지 산출 방식 : 폐쇄 영역 +1, 분기 노드 +1  
* 복잡도가 50 이상인 경우 매우복잡 프로그램으로 리팩토링 (모듈분할,재설계) 필요  

### [3년치 기출, KPC 모의고사] Wi-Fi 7

**[정의]**  

- 2.4GHz, 5GHz, 6GHz 3개의 주파수 대역을 활용하여 이전 세대(Wi-Fi6/6E) 보다 최대 4.8배 빠른 최대 46Gbps의 속도를 제공하는 차세대 무선 통신 표준(Extremely High Throughput(고 처리량))  

**[핵심/키워드]**  

*초고속 및 고용량 - 주파수 대역폭이 160MHz에서 320MHz로 2배 확장  
*4K QAM 기술 -데이터 압축률 높여 와이파이 6 대비 한번에 약 20%더 많은 데이터 전송  
* 다중 링크 작동(MLO)- 2.4GHz, 5GHz, 6GHz 등 여러 대역과 채널 동시사용  

>320MHz 고 대역폭,4096 QAM, MLO(다중 링크 동작) 제공  
Wi-Fi 7에서 신뢰성, 연결성을 향상한 Wi-Fi 8로 발전하고 있음  

802.11ax (wifi-6), 802.11be (wifi-7) , 802.11bn (wifi-8)  

### [3년치 기출, KPC 모의고사] CTEM(Continuous Threat Exposure Management)

**[정의]**  

- 보안 위협 사전 대응을 위해 조직의 중요 자산에 대한 취약점 및 위험을 지속적으로 식별, 측정 및 우선순위 지정/대응하는 보안 위협 관리 시스템  

**[핵심/키워드]**  

&lt; 주요 기술 요소 &gt;  
공격 표면 관리, 위협 인텔리전스, 취약점 관리, 위협 모델링 및 시뮬레이션, 보안 오케스트레이션, 자동화 및 대응, 지속적 보안 모니터링,취약점 및 위협 검증,  
위험 기반 의사결정  

### [3년치 기출, KPC 모의고사] 파인튜닝

**[정의]**  

- 전이학습의 일종으로, 기존 모델의 일부 또는 전체 가중치를 조정하여 새로운 데이터셋에 맞게 추가 학습하는 방법  

- 사전 학습된 인공지능 모델의 가중치를 새로운 데이터에 맞게 세밀하게  
조정하는 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
도메인 특화 최적화, 사전학습 모델 활용 , 일반화 성능 유지  

### [3년치 기출, KPC 모의고사] 데이터 레이크

**[정의]**  

- 다양한 형태(정형+비정형)의 원형데이터(Rawdata)들을 모은 저장소 집합  

**[핵심/키워드]**  

&lt; 특징 &gt;  
① 비용 효율적인 스토리지 ② 빅데이터에 대한 확장성③다양한 데이터 유형에 대한 유연성  
- Schema-on-Read, 다양한 데이터 유형 지원, 확장성 및 비용 효율성,  
 전체 데이터 수명 주기 포괄 설계  

### [3년치 기출, KPC 모의고사] 데이터 스웜프(Data Swamp)

**[정의]**  

- 체계적인 관리와 메타데이터 없이 무분별하게 데이터를 축적하기만 하여 활용할 수 없게 된 방대한 데이터 저장소  

**[핵심/키워드]**  

&lt; 원인 &gt;  
 ① 무분별한 수집 ② 거버넌스 부재 ③ 버전과 기준 혼란 ④ 조직간의 사일로 (silo)  
&lt; 재발방지방안 &gt;  
 ① 메타 데이터 확보, ② 카탈로그 구축 , ③데이터 거버넌스수립 ④ 수명주기 관리  
⑤ 데이터 품질 모니터링, ⑤ 접근통제 강화 ⑥ AI 특화관리체계  

### [3년치 기출, KPC 모의고사] 터보퀀트

**[정의]**  

- 구글이 개발한 벡터 양자화 (VQ, Vector Quantization)기반의 AI메모리 압축 기술  

'- KV Cache(Key-Value Cache)를 3~4bit 수준으로 압축하면서 정확도 저하를 최소화하는 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
2단계 압축 매커니즘, KV Cache 경량화, 메모리 효율개선, 응답속도 향상  

&lt;기술요소 &gt;  
(1) Random Rotation  
벡터를 무작위 회전시켜 좌표 분포를 균일하게 만듦  
각 차원을 독립적으로 양자화하기 쉽게 변환  
(2) Scalar Quantization  
각 좌표를 3~4bit 수준으로 압축  
Lloyd-Max 기반 최적 코드북을 활용하여 왜곡(MSE)을 최소화  
(3) QJL (Quantized Johnson-Lindenstrauss)  
양자화 과정에서 발생하는 내적(Inner Product) 오차를 보정  
Attention Score의 정확도를 유지  

### [3년치 기출, KPC 모의고사] 데이터 자산화

**[정의]**  

- 조직 내에 산재한 데이터를 단순 저장 정보가 아니라 경제적·전략적 가치를 창출하는 자산(Asset) 으로 관리·활용하는 활동  

**[핵심/키워드]**  

&lt;필요성&gt;  
데이터 거버넌스 및 관리 체계, 데이터 품질 및 정제 , 기술적 인프라 및 아키텍처, 가치 평가 및 비즈니스 모델  

&lt;구성요소 &gt;  
* 데이터 표준화 : 데이터 형식·용어·코드 표준 정의  
* 메타데이터 관리 : 데이터의 의미·출처·소유자 관리  
* 데이터 품질 관리 : 정확성, 완전성, 일관성 확보  
* 데이터 카탈로그 : 데이터 검색 및 공유 체계  
* 데이터 거버넌스 : 정책, 역할, 책임 정의  
* 보안·개인정보 보호  : 접근 통제, 암호화, 가명·익명 처리  

### [3년치 기출, KPC 모의고사] 다중 에이전트 시스템

**[정의]**  

- 여러 개의 자율적  에이전트가 상호 협력·경쟁·조정을 통해 공동의 목표를 달성하거나 복잡한 문제 해결 시스템  

**[핵심/키워드]**  

&lt; 특징 &gt;  
에이전트(독립 객체), 환경(물리/가상 공간), Coordinator/Manager (협력·경쟁·조정),통신(메시지 교환)  

### [3년치 기출, KPC 모의고사] 데이터 이상치 (Outlier)

**[정의]**  

- 전체 데이터 분포에서 다른 값들과 현저하게 차이가 나는 극단적인 데이터  

**[핵심/키워드]**  

&lt; 이상치 영향도 &gt;  
① 통계값 왜곡 ② AI,머신 러닝 성능 저하 ③잘못된 의사결정 유발 ④ 처리 성능 저하  
&lt; 이상치 처리 방안 &gt;  
 * 삭제 , 극단치 기준적용 , 대체 , 변환  

### [3년치 기출, KPC 모의고사] 데이터 편향 (Bias)

**[정의]**  

- 데이터 수집·표본·분석 과정에서 특정 방향으로 데이터가 치우쳐 공정하거나 객관적인 결과를 반영하지 못하는 현상  

**[핵심/키워드]**  

&lt; 편향 영향도 &gt;  
① 분석 결과 왜곡 ② AI 공정성 저하 ③ 일반화 성능 저하 ④ 신뢰성 저하 ⑤ 법적·윤리적 문제 발생 ⑥모델 드리프트 가속 ⑦ Hallucination=악화  
&lt; 편향 처리 방안 &gt;  
*  데이터 균형화 , 데이터 다양성 확보, 데이터 정제, 민감정보 제거  

### [3년치 기출, KPC 모의고사] 코드 스멜

**[정의]**  

- 잠재적 설계 문제를 암시하는 비효율적 코드 구조 및 패턴  

'- 프로그램이 현재는 정상적으로 동작하지만, 설계나 구현상 좋지 않은 징후(Bad Smell)가 있어 향후 유지보수성과 확장성을 저하시킬 가능성이 있는 코드의 특성  

**[핵심/키워드]**  

&lt;코드 스멜 유형 &gt;  
 긴 메소드 , 중복 코드, 너무 많은 인수, 큰 클래스  
&lt; 코드 스멜 해결방안 &gt;  
* 리팩토링 , 요구 검증 , 요구 추적성, 코드 설계 원칙 재확인, 형상관리, 아키텍처 변경  

### [3년치 기출, KPC 모의고사] 리팩토링

**[정의]**  

- 외부 기능 변화 없이 내부 코드 구조를 개선하여 유지보수성과 확장성을 향상시키는 활동  

**[핵심/키워드]**  

&lt; 리팩토링 유형 &gt;  
*  Extract,move Method , Extract Class, PushDown Field, InlineClass, Rename  
&lt; 리팩토링 효과 &gt;  
* 유지보수성 향상, 복잡도 감소, 응집도 향상, 확장성 강화, 테스트 용이성  

### [3년치 기출, KPC 모의고사] 빅데이터 분석기법 중 클러스터링

**[정의]**  

- 데이터의 유사성, 거리 기준으로 유사한 속성을 가진 데이터들을 몇 개의 그룹(군집)으로 묶는 기법  

**[핵심/키워드]**  

* 유사한 속성 기반,클러스터링 유형  
K-Means (K-평균) , DBSCAN , 계층적 군집화 , EM알고리즘  

### [3년치 기출, KPC 모의고사] 필터링

**[정의]**  

- 불필요한 정보를 제거하거나, 사용자의 관심·요구에 부합하는 정보만 추출하는 분석기법  

**[핵심/키워드]**  

* 주요기법  
노이즈 필터링 , 중복 데이터 필터링 , 결측치 필터링 , 이상치 필터링  

### [3년치 기출, KPC 모의고사] 뮤텍스

**[정의]**  

- 하나의 쓰레드 또는 프로세스만 임계영역에 진입할 수 있도록 상호배제를 보장하는 락(Lock)객체  

'- 하나의 스레드만 공유 자원에 접근하도록 보장하는 상호배제 락(Lock)  

**[핵심/키워드]**  

* 뮤텍스는 자원의 소유권 개념으로 동작  
초기화 → Lock() 호출 → Unlock() 호출  

### [3년치 기출, KPC 모의고사] 세마포어

**[정의]**  

-운영체제 자원을 경쟁적으로 사용하는 다중 프로세스 환경에서, 임계영역에서의 상호배제 또는 동기화를 위해 사용하는 도구  

'- 공유 자원에 접근 가능한 개수를 관리하는 카운터 기반 동기화 기법  

**[핵심/키워드]**  

* 공유자원 접근을 통한 동기화 기법, 세마포어 매커니즘  
→ 초기화 , P 연산 , V 연산  

### [3년치 기출, KPC 모의고사] 모니터 기법

**[정의]**  

-언어 수준에서 상호 배제와 조건 동기화를 제공하는 고수준 동기화 메커니즘  

**[핵심/키워드]**  

* 매커니즘  
초기화 → 진입부 함수 호출 → 조건 대기 → 조건 신호 → 진입부 종료 (락해제)  

* 객체 내부에서 자동 Lock 관리  
* Condition Variable을 이용한 대기/통지(wait, notify 등) 지원  

### [3년치 기출, KPC 모의고사] 가상 메모리 관리기법

**[정의]**  

보조 기억장치에 저장되어 있는 프로그램을 주기억 장치에 적재하여 한정된 물리적 메모리를 효율적으로 사용하기 위한 관리 기법  

**[핵심/키워드]**  

&lt; 가상메모리 단편화 유형 &gt;  
* 외부 단편화 (큰 프로세스를 적재하지 못하는 현상)  
* 내부 단편화 (블록 내부에서 사용되지 못하고 버려지는 현상)  
&lt; 가상메모리 관리 기법들 &gt;  
* 통합 , 압축 , 프레임 , 버디 알고리즘 , Slab Allocation  

### [3년치 기출, KPC 모의고사] CIDR 개념

**[정의]**  

IP주소를 효율적으로 할당, 라우팅 테이 블을 단순화하는 표현 방식  

**[핵심/키워드]**  

&lt; CIDR 유형 &gt;  
* 수퍼 네팅 (연속된 IP주소 범위를 하나의 큰 네트워크로 통합하는 기법 )  
* 서브 네팅 ( 주어진 IP8주소 범위를 여러 개의 작은 네트워크로 분할하는 기법 )  
* VLSM (서브넷을 서로 다른 크기로 가변 분할하는 기법 )  

### [3년치 기출, KPC 모의고사] MLOPS

**[정의]**  

머신러닝 모델의 개발,  학습, 배포, 운영, 모니터링, 재학습까지 전 생명주기를 자동화하고 관리하는 운영 체계  

**[핵심/키워드]**  

* 목표 (모델 재현성, 품질유지, 모델 drift 대응)  
&lt; 구성 요소 &gt;  
* Data Pipeline : 데이터 수집·전처리 자동화  
* Feature Store : 학습·추론용 특징값(Feature) 관리  
* Model Training : 모델 학습 및 하이퍼파라미터 튜닝  
* Model Registry : 모델 버전 및 메타데이터 관리  
* CI/CD Pipeline : 모델 자동 테스트·배포  
* Monitoring : 성능·지연시간·Drift 모니터링  
* Retraining : 성능 저하 시 자동 재학습  

### [3년치 기출, KPC 모의고사] 모델 drift

**[정의]**  

- 학습 시점의 데이터 분포나 입력-출력 관계가 운영 환경에서 변화하여, 모델의 예측 정확도와 성능이 지속적으로 저하되는 현상  

**[핵심/키워드]**  

&lt; 유형 &gt;  
- 데이터 드리프트 (입력 데이터(X)의 분포가 변하는 경우)  
- 개념 드리프트 (입력(X)과 정답(Y)의 관계 자체가 변하는 경우)  
- 레이블 드리프트 (정답(Y)의 분포가 변화하는 경우)  

### [3년치 기출, KPC 모의고사] Model DoS

**[정의]**  

-  공격자가 AI 모델에 의도적으로 복잡하거나 연산 비용이 높은 입력값을 전송하여, GPU/TPU 등 하드웨어 자원을 고갈시키거나 추론시간을 지연시켜 정상적인 서비스를 불가능하게 만드는 공격 기법  

**[핵심/키워드]**  

&lt; 공격유형 &gt;  
- 연산 과부하 : Sponge Examples  
- 입력 조작 : Input Flood  
- 알고리즘 : Algorithmic Complexity  

### [3년치 기출, KPC 모의고사] Self-Attention 매커니즘

**[정의]**  

-  입력 시퀀스 내의 각 단어가 다른 모든 단어와 맺는 관계(유사도)를계산하여, 문맥적 의미를 반영한 새로운 벡터 표현을 생성하는 메커니즘  

**[핵심/키워드]**  

&lt; 아키텍처 &gt;  
Query(Q) - 현재 시점의 단어가 궁금해하는 정보  
Key(K) - Query에 매칭되는 식별자  
Value(v) - 두 단어 간의 연관성(유사도)을 확률(0~1)로 표현한 가중치  

### [3년치 기출, KPC 모의고사] PET(Privacy Enhanced Technology)

**[정의]**  

-  개인정보와 민감한 데이터를 보호하기 위해 설계된 기술과 방법론으로, 데이터 유출을 방지하고, 안전한 데이터 처리 및 활용하게 하는 기술  

**[핵심/키워드]**  

&lt; PET 도구 &gt;  
차분 프라이버시, 합성 데이터 생성,  영지식 증명 , 동형 암호화 , 신원 기반 암호화, 안전한 다자간 연산, 신뢰 실행 환경, 연합 학습, 분산 분석  

### [3년치 기출, KPC 모의고사] ISO/IEC 42001:2023

**[정의]**  

- 조직이 AI를 개발, 제공, 사용 시 책임 있는 AI 운영을 위해 정책, 목표, 프로세스를 수립하고, 지속적 개선(PDCA) 하도록 요구하는 AI 경영시스템 표준  

**[핵심/키워드]**  

*AI기반 제품과 서비스 제공 조직 뿐 아니라 도입 사용하는 조직 포함  
&lt;구성요소 &gt;  
1장. 적용범위, 2장. 인용표준, 3장. 용어정의, 4장. 조직상황, 5장. 리더십,  
 6장. 기획, 7장. 지원, 8장. 운용, 9장. 성과평가, 10장. 개선  

### [3년치 기출, KPC 모의고사] 데드락(Deadlock)

**[정의]**  

- 멀티프로그래밍 시스템에서 두 개 이상의 프로세스가 서로 상대방의 자원을 요구하면서 기다리는 상태  

**[핵심/키워드]**  

&lt; 발생조건 &gt;  
* 상호배제 , 점유와 대기 , 비선점 , 환형대기  
&lt; 해결방법 &gt;  
* 예방, 회피 , 발견, 회복  

### [3년치 기출, KPC 모의고사] 모라벡의 역설(Moravec’s Paradox)

**[정의]**  

- 인간에게 쉬운 시각·운동 지능은 컴퓨터로 처리하기 어렵고, 인간에게 어려운 논리·연산은 컴퓨터로 처리하기 쉽다는 역설적 현상  

**[핵심/키워드]**  

* 발생원인 : 기호화의 난이도, 프레임 문제 , 폰노이만 구조, 상식의 저주, 연산 밀도 격차  
* 극복위한 AI 패러다임 변화  
- Embodied AI , VLA Model , World Model 활용  

### [3년치 기출, KPC 모의고사] SSD(Solid State Drive)

**[정의]**  

- 반도체 기반 비휘발성 메모리(NAND Flash)를 저장 매체로 사용하여 기계적 구동부 없이 데이터를 전자적으로 저장·처리하는 고속 저장장치  

**[핵심/키워드]**  

* 반도체 저장 방식, 랜덤 접근, 고속 I/O 처리, 컨트롤러 기반 처리  

### [3년치 기출, KPC 모의고사] 시스템 콜(System Call)

**[정의]**  

-  사용자 모드(User Mode)에서 실행 중인 응용 프로그램이 커널 모드의 운영체제 기능을 안전하게 요청하기 위한 공식적인 인터페이스  

**[핵심/키워드]**  

* 필요성 : 보안성 (직접 접근 차단),안정성 (시스템 오류 방지),추상화(HW 구현부 은닉)  
* 사용자 요청 (System Call 호출) → 커널 처리 (Trap 및 mode 전환) → 결과 반환 (User mode 복귀)  

### [3년치 기출, KPC 모의고사] 뉴로모픽 컴퓨팅

**[정의]**  

-  인간의 뇌 신경 구조와 작동 방식(뉴런 및 시냅스)을 모방하여, 하드웨어 수준에서 초저전력·고효율·병렬 데이터 처리를 구현하는 차세대 AI 반도체 기술  

**[핵심/키워드]**  

*특징  
대규모 병렬 처리, 메모리와 연산의 통합 처리, 스파이크 및 전기신호, 비동기식, 이벤트 기반 , 프로그래밍 기법으로 스파이킹 뉴럴 네트워크 (SNN)  

### [3년치 기출, KPC 모의고사] 베이즈 정리

**[정의]**  

-  사전적 확률을 구한 후 확률 영향을 미치는 변수의 확률을 반영하여 사후 확률을 구하는 방법으로, 확률 정확도를 높이고자 하는 주관적 확률 이론  

**[핵심/키워드]**  

&lt; 특징 &gt;  
① 사전확률과 사후확률 사이 관계를 조건부 확률 이용 계산  
② 불확실성(직접 관측으로는 쉽게 얻어낼 수 없는 현상) 추론에 용이  

### [3년치 기출, KPC 모의고사] 개발방법론 테일러링

**[정의]**  

-  불확실성 검증 위한 선도개발에 적합하게, 기 정의 된 개발방법론의 절차/기법/산출물 등을 재활용하여 계획을 수립하는 기법  

**[핵심/키워드]**  

&lt; 구성요소 &gt;  
프로세스 테일러링 , 작업단위 테일러링 , 요구사항 산출물 테일러링 , 설계 산출물 테일러링, 조직 테일러링 , QA 범위 테일러링 , 개발도구 테일러링  

### [3년치 기출, KPC 모의고사] 자기회귀모형 (AR)

**[정의]**  

-  현재값을 과거 관측값의 선형 결합으로 표현하는 시계열 모형  

**[핵심/키워드]**  

* 특징 : 정상성 가정 필요 , 자기상관 활용  
* 한계점 : ① 비정상적인 데이터에 적용 어려움 ② 과거 데이터에 의존적  
* 해결방안 : 차분 적용 (차분 적용 후 AR모델, ARIMA 모델 활용 가능  
*수식 : 현재값 = 상수 + 과거 p개 데이터의 가중합 + 백색잡음  

<img src="data:image/png;base64,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" alt="embedded_DR_47_Keys_img_1.png" style="max-width: 100%; height: auto; margin: 16px 0;" />

### [3년치 기출, KPC 모의고사] 이동평균모형 (MA)

**[정의]**  

-  현재값이 과거의 오차들의 선형 결합으로 표현되는 시계열 모형  

**[핵심/키워드]**  

* 특징 : 과거 예측의 오차 기반 , 정상성 필요  
* 한계점 : ① 과거 데이터 자체를 활용하지 않음 ② 장기예측 시 성능 저하  
* 해결방안 : ① AR과 결합 , ② 차분 적용  
*수식 : 현재값 = 평균 + 현재 오차 + 과거 q개 오차의 가중합  

<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAVcAAABfCAIAAADTdxOWAAAQAElEQVR4AexdB1wUx/efmb0Cd0fvVRA7IGJD7CVG0/62GEvEaCJqYvSnpto11qixxhpRERQbGnvsFcGGBVABAem9H+W4293/2wONKOBRRCM7n9k289p8582b2dkTiYpPPAI8Ag0bAYL4xCPAI9CwEeCjQMPuf771PAII8VGA94J3CgFMCFWaCMYY7uDyThn4XzamMtv5KFAZMnx5vSPAjX+CC2IeBNy8+yBdRQjJS0nPK5AjQnC9G9OQFPJRoCH19rvcVggBOPnBGe/Vm89G5GenhP+9fsnK+TP3BcblMrAoeJct/+/bxkeB/34fvgctwITCOZEnNqxbt/96rrVj5w4u9sqw/YsX+YdlFAp0CGLZ96CR724T+Cjw7vZNQ7EMw4IfF0Qd3rx8f6ig68QfP26pa2hs3b5LM2PH/h3sjfUphPggUC1nqC4xHwWqixhPX8cIwHof4+JQ/8OXnhjadu7bQQ/kK3LTQoJDSJOWTmamWhAE+CgAoLy5zEeBN4ctL1kTBAjGLKJDw4IT0/ScHdo11QUmNisvOiRUaebQzNRQCs8MHHx+cwjwUeDNYctL1gCB0s3/gtT43BzdRlbN7bmVAMrLiL0XmSTp2KaZriF4KK2BHJ6kFggAxrXg5ll5BGqJQOm+n7RxI0NjexGDaZWKVqZEBJ8+H6lq3rK5gVSEEL8SqAzjuirno0BdIcnLqRkCLMMglmoycNwQe0ncaa9Nfv6rFyzbdOYpY+3qZCzRRvz3gZrhWh0uPgpUBy2e9k0gwLIsI9TvOmbKz+O/7u/u2ryVW3NDIjJp62wrlcILA78UeBOgl5PJR4FycPAPbwMBlmVpWmja1LXzBz3bO7Vq1tJQl5a2a9dGT0eA+PeBeugRPgrUA8i8Cg0QoFmWKSxIeXjN12vNjnNPMooyopNylQyDCawHNOB/n0nedNv4KPCmEebla4YARpgpKcrLyVDoW/cY/M2oNubFJQoVDe8DWDMBPFWNEeCjQI2h4xnrFgGWYbWlVs69PaYuXrdx5WLPAV3sTAQYNgf5nwzVLdCvSuOjwKuY8CVvAwGWZYlArC2VSbSEFCUQiLUkWiKCMZS/DXMalE4+CjSo7n7XGwtDnmXKEnf/rttbx/a9LXF8FHhbyPN6eQTeFQT4KPCu9MR7aAfGhHrTiRB+87DWrsNHgVpDyAuoDAGWZWiaeSHRNK2qWaLV6QVRZbcsyyI+DFTWAZqW81FAU6R4umohQAgpSQk5vXLYaI9hw0Z9+eVodfYYPnzkF1+MqF4eNhK4hg8fNWLkqBEjPEaOLM2jho8YNeyb1WdvJiKK/MfcuFpI1gMxD189gNwQVWCMhWyBPCZo737/g/sO+h/w3++39/rTfMq0mYOljbW5tUbZwsbG0lKXKZInPQ69ef6w3/79e/btg+x34OBB/0MHDnr/4X/pblwRxrwf18bJePRqgx7PWykCDMMKTFp0+nzamDZSqYggIhRTuAA1bdt/3OwFc2bPnDlzhiZ5xoxfZ85dsGTpstVr1m722r51w+rfF0we/klrE6JkVCqKTTp+5fbdh3kI845caVe8voIH7/UY8RQ1QIBlGVZsZNtj9A+ThrjqUESpwmKtnJDzf18IDikxNrUwN7fUIFuYm1tY2ju6uHb5oN+nQz3Gen439efZ8xYsXLLk91njB7Q2lKDky2dvBIXkQhjgtwdq0E2lLHwUKMWBP9c9AgzNskKTpoOmThneyUabKlYgqfJRkN/qlTsvRSlAHQN7h+pNv+qcGJYYNXP9+Otpi5YtWzj7f5+3lIafuXj+RiqEgXfPl6GR/4lcf8jBu1vFX43KPvVg7r+geJWCj/D/CT+q2EiGYZBAz3noz1M9+tjrUyVFRKadEnTV988tp5KKEGwg4mp3L1sWOhhk0OL/pixasWRmP1VS5LXD0SqEyzypYlvKSst7Wf25f5n6d/NSTzBgjBhaWZQvl+fJ5fKCgtKcL8+XFxYoaIzBGRi6uLBQXvCsVi7Pz4PaIhVUvZvQ8VZpgABLM4hC1p9MmjK0v7MeKS5CMngvCDi6btOhiHwWE8J1vQZyXiFhaZpmEbEbOHnGpG56iYH+QZmcH1UlDnNzDKGzYx7evHTu7NXbUZn5iKLqaQS80oB3qaB+MCCEKOUp909779y5bdu27bt2efv6+uza+dfWLQfOXYmSQzVRFaTe8d/ns2P79l3eXtv+2uK1deNfe09cDc0iCEN6lzDjbakOAhAHWEQZ9f5+wtAPu5pTymKsrZ0RfnPfikV77+QyCPq+xnGe4QIB1fqLgS6OLtkh4cWoClfBhCKoJDvmxknfDauWzJ318/Sflm73v51ZiKga60fvSyL10RACOBfLk+6dO7Lf74D3htUL5s2bMWv2gkVr/9x+OuhBihJswKqipPtH/DYumD1r5rzfV63b5u3ls+9kwL24IuhZUi9WghVvI2PwT5iRMGD0NtRrolNtIcX1oibUr9DAIp5hkXG3KT9+M7hnc1xcjMTaiieRV7Yu33M/FfqX1GIccoFAv8OoiRNneLQVq3+hxL6iHwq4EKBIv7N/zWTPxRdlXX/2PXlqfj+5/9bFqw7F0qC/xm0D2Qih//q5XsYXdBUtNXEcPMtrl4/3rhXDrMyo7MwsXZdBM9esnDbOTZ+BZaPExHnwvEn97cz1TV2Gztu09+DRI35rfh3bx4IGJ4K1338d6Erthz2yEkWJimEqpXjrFQytBBNr0wksw7BY3HbIhKEDP3agikuwWKxKDLu2aenO25m5LCJULdrIsJS2RKIjE1caRykIMzmPj22b8ZtfeJvhU74a4m5rZN61i7N5cciV4/88YhDBuFLmWlj2n2GtlyjAoUEJZUYWtnaNmzkP+HKoa2MrjJIS5UUKYmIkE2GKILagIPLMwXuNP5uxZs1cj34ujR0cHBpZmuqLOeb39SDwppQeEbR53KYriUnF8PTuNRSMkj8KPvXn+G3BmYUMPNXQRBZCPRY7DRs3esiI1soilUAoYLLCL/01b935iGwl4gZqDSUjEE1DYirhpyDEZIQE7F6xLUzZZPzUQe72OtyQ15LqG8jiY+NuhEUgxMKKrBL2hlBcb1GA+9Ny3GscAN7ys17NGjURFDy+HHTpYgygjFFBxoO9i1dcFPcaN2bUR05GQthLhH7lcmV9C2z//YwxZorzUh4HPkwuKOA2t2rTJBD2LNdGzEu8IFKZkxn3KPBJjkIJg4UbQC+RaPrI0gzWsfvwu/Ffj+ipK+cW4jgv7qbPiu1BD9NpREgtRFduAgYPz4oKOrx565MCi4Fjh7W0gXmFBXqlikFEmauQp6Zp7mOARlkGCe9PBozqszGw7sVI0Lxv92Yt7MSqp9dC7tyIRijj9r4V80/muo2fNLGPs646trP1aVU1dGFCqRMpDxxMJVBMcA0cGRZCIolQQEgNeJ8ZjkE5BfP0swyP5e17RlizKxFQIolYUJPWlVcIcYCV2bYfPnHc0I46hSowV8AmBvstWnci9GkhJrWBoLyi508gUxl3+8phr7NyE+tug7qYigEYlvOu3JycwmykYthiBWwrAkPV+KshpsDissxBXDUHiPyvZMCkXk1lubgrsP6ot0sLe11V3P3H51at37hjuW+oxaBxE//P1ZDAKoDhOqlerdJMGSEUqypIfBgQEBaXL2cJKQMPAgPCuDgrU8HQiJt7NBP3nApDev5Q3RvwRooiiqTQs76bViyYPf+3xau2+1+NzCz12upKq4y+NhaWk8ltEIhMO/T3nDS+r2kxjWmGCFKu+69ec/B6fC7EgTJIy/HU4gHiSm7MrSsnj8cJ7Gw69m+tKwAFLAvDV5mYlJ4Rj7TElFhLUKWGUiRJSc7jS39vXbFkwew5i1as3XP5XpIKOp4CDVVy/ycqAZT6tZNlWBjkln17d2jV2hCl3T992PtIpMWg72d/1dkI3s/ULw21sKi0y6gaJPCMqvUSjFV5GTd3rfh94bIjD+PzYWQAD8YEFyXfPbV83u8r/G/kKFTwXLWcOqslnBeq4gP3rZ81afLPi9dt8jm4z2fLn8t+mTxx2i+z9gQkyxWEELCxzjTWhSB4i2e1DVt/OvGHrz5tzGKMaKG08IH/tk0HLkXJMYaNvLrQUioDGi8PD7kbeCnN0M6uz/AP9GXcgFf3UGFienZ8NjLSMTAxFampwS0RhjowSf3MnTBATOi8sINbF0yd/MP85Vt3+B7027lh2W8/Tpjw4+/rTz2Rc3Ef1HDEtT+wWn/t5VRXAqkuQ63pIQzAZG/u9ol7RzcTlJSAtY2bjZ/8kRVCLE1zK4WKNHC9oR7ZuKLaZ2UAoiIp5MbJ7V7e3t4+muYd23ceC3ycUAzczwRVdIWupnMzwk/7nAwIeJAqV3BOgxCGYVacdO/Ultmrth2+8VShYqEI1UMCf0GMIunRnm2++07eTBNau3/h+cO8RfPnzvh2UHdbZfTd8NS8EgaX4QXOzMFX/71dIRIMwxJDqy7fzPimZysRzSpVQllJ+CnvjX+dvZfOEOqZ0RXyVqMQRjRSRIVEPLqfgUSFqZHX/bx9dvv6+PjsgvPGw5dDkpDMQmZja4EQhtdQjAlFCIbASUFfI0hQwsqzH537a8ueo4HxRabt+309/df5i3+bOdWzj7UsK+x2pLwEmlKG8bMJqOwR+KuXKYoihNNPVY+vDqjfil9w3aytY0woKbSgKE8eH56jgjtUCX5AztBFGXEpWXK5CuNKqBDC0IOqjIj7l/b77du//8CBAwdfn/cf2Ld374Fzd2PSVNADqFLZCByDkefG37yaJFA26tmxkbk+hC0Y8gjRCWlPw+4KbI07dXKVacHeU8WhDBPqlYQQEgoEAuh6SiAQwtMrFFQlFoG/MPL8yJN/7I23GLJsz9G9W5f+OPmrz4d5TJiyYPOeAzs2bp7+sZ2uNgsDDmFMqfIzstKS0gtBGmRQVFHGlZpIUQQTsLBCEwGZiqRVVcaZhWW2LqN/mtDP2UKAlEpKxjw447dp7aFgiAOEoMqtrEpuuTqMMWKSo6OePMoksNnERl06cBC6e7//voOHt6/Ycvbq/QKqiZVZUwf1/5KMMKssjL9x2v/w2fsJWfC6hxEhRJkWcvvY1tPM8F+8jx3csXLed/CJY/jYyXOWbTtwyGvhojFtdCnMMDCrIUwx8vSUjNQsOY1xta3HmJCi1Ic3Tx46fP5RhorFpPoyUM0TqTlrzTgxoQhmssJOHb4Rnai0MKSyoiMDjx+LKma5plcgExOCVQVPr+9Y5nvhSVxVn9PAtxhZy09Gzfbbs3PHTq8dO7a9Pu/08vbx9V34VW9nHQa2LtkKDFAXcZ1SkJ9+73qouFi7o4udjgEgxyAoZtPjkx/fTTDUtWrb1kwM44StQAiGhY6iICcnOysrOyv7ec7Ly8/Mzs0tpovzc3Iy8/Nz/63KzsrKys7NkStBXAVOBUUquTI+IsSik2MLM0lBbnpKcnJKemZuYQl4iSeY2wAAEABJREFUsMyyhY2uSABv3WALAKhMuL53v5f3uThwLnAwdYteOkFLaJUiPzsnOzv7BQuz8/LzM3Pz5cV0UU52ZmZ+Xt6LtVmZObl5RSpQ8pK01z6yDA2f+U3dxyyc8n/tLbXpEgUlFcefP+e3ZdvldDkCO18r4rUEgFFuckJmbBSSObgNnLd313ZvH6+dO7d7+3ot+KZzUx1ErOzs2rWBpQCLMCG0Ij9418oly70uPslgMMYII1SclpaWlGDf3d1elJebnZacnJyakVtQTCOxgZ6Vg7WMgY5l4bUGY0InXPX18jl4LUo9nbzWuPIE0Ck4L/z8geVzVu4OTlQhDAXlKd7oE/jyG5VfXjjmQgAqenpt85w/H5p3+frHXwbaU/InSfdPHIlQFLOIvGwOxhAzkKIk9YLfrgv3YgsQjLLyIss9sSxDibV1DUxNTU00TqamBroSEaXerygn7cUHMEyZlRtxLwTGeSd3JwNdLcT931lQXJgQ+/huuL6OgWsLO5EQPId5kU99jwlhGUVGRFDg1bMXL168fPl5vhx4JTD4XnxRfNitm5cDrj0vh5vzFy5cDgqKyFLQMKxBrFrS8xMoEetKHJxaP7l40X/d78vnzZg6edLU39bsDnhaAoaxLMtNUAjgo8DGyFvnjh04EZ5HOIRfkcUJJYQwCnlq6NVrYOCFFyy8eD3o6t0HEfFFcXeCrl6+dvHSv8ZfvHjh9LVbwU9zwJgaDFsG3v+0xA5Dpn3fv0szCaNQCiRUwuVTRzbuvqvE0Gawm7OshgfmmsmmpKalxpVQ5mbN3TqZmxoZ6hsZGRka6RbGJsmTE5GNY5PW7s0QArCgCSJtkw5Dxv+48H/9nB0EiGEQi5COuZW1reXdQ9v2rF84f9ZPU6dOmf77vtMh2WAUAMyyQIIAY0APJVw+fvTc6YgcFawGEeK0I80TJ8e4cY9h02dNnfJRUzHBLOjXnL22lLWDunraYTBgVJQYtnfJ+rt2HQd+9a3nkPYu7q5EmZr25J/zkQXwqo1fsodhaFpVkJETfOu23N7UQcdABCXV01on1JxZmSmxwdfzRJRDeycjHQnnOwiK6ZTE+LAQkb6Ok2tLgUgAxbgSD8AYg7e8mqEcwVFRJRSjypOIpYwdjCJuHdnhs+fvM9euXTxz+XZwdBbMJM95GKVSRauig0MfF6QZtGhqS9MQ7DiXe05R7gZXaASMcIwRxhVUUlxdORHVeWBplqVk9oN+/d/gzp1M2GIlg4hEoiuVsghXR07FtNA5iszU3Mx4ZG6k27SJ2XMqNvtmYFR0FGrk1rJd21bQYwhhzNAKlcqo64Ahvd2a6ROm7IeSrExXaGCqFfy3z479R06ev3bl0j/XHoYkFyJIpTEA2MFFlcrM4IAnuWID80aNWIahuQgCJJplTChEK0tURs1bf/zFoNYGWpiFbtKMt26oAKq6EfQ6KZgCjylKCdk7f+phsePwcVM+ttMW2zRv26lvF6RKTonxP3M/rxgcmHomCBjYwszUx0EXT5/bf/J6pkiCEx6FhSelylmKqsRJMCaqooKstMSkaqTExLQsebEKvPyZ6leuBPTlpMffuxkvoIzdXGx0ZEDCIK44Pj7m8Z0cYx0zxxamSAQ+AcMMKstllqExpWXczN29e9/evXr36PE893Dv7t7O1UbbxqmjW48uXZ+Xw80Hffr0cHdvbiSm8Cs+AVgy+XFBh1Z4JXaZMW/n2eNHTpz859yVS/vWzxnkKGZYBiYpMI4tTg4LuRlw5MCpG3FZQoEy/e7d+wmFNIsJhgaVM5GhaaKlY+bcvWuvXr36vGBhr87u3du2bm6jbdvevXuPrr16/mt87159+nXt2M5OH/qM01hOoGYPDDflCW37Tps2uKuzXomg9SCPb2d84ShikLpGMyGVU7EMrVIqkZGulZX1cyo2/vLp0LBw5PJR774fOBDEYoxV8vjwy0f/PhWWmKciFLQHIYrCTMyd4/5bThqN3rzT5/ipEyf+OXP2wsWdP3h2M2UYhsWIc1GVIjM8MOjyab+/78XQNC54GhMaFScHX8f4ucaqb2ABrMqODTp37OSVW+msgLAac1Yttxq19RMFMKEIYjLjL/w51yuzxUCPsZ+0MhRzPx0watO2c78ehnRqztNDx27l55Ug9MwijLgAWZiXmBT/+M6DXLFdIwPMKPNLSuhnFC83ExNC5I9O+C4e+eWYsWPHff215+vz2HFjRnt4zPW+8CAfuBEofVkq9wzFBRnpUcHBWgLi7NhCKoU5n8EcdWZ04pOwKB0zaVvnZow878Hh0yHJKYUgCnN8Lx5EKNHV1dXXezHJZFJ9PZkMvllLoUoqlb1YCfc6upIKfquDAYC82MSbx/1wz/4ffdS/g5NjK0cnJyfn1i2bNDLVoQCHMu3FBdn5OU9CgqNSlLpmjUwFWXlFCsJyVqlP3M0LB6FEYAaofTHLpFKwUCKmtHT19PSlsvIm6uvqyF7zuf0FBRXclnp8SUxIWGyipJvnhJ+++6yJnpiFOFYBcfWKoIkisRQLtABFWzOTMmYVijhzODgy3GrIgI/7djeGAQ8j92Ggr/f5LFXC6XmLdp27noSg/wDj1NtXbwXcMB40YUBv1zaOrVo6OjkCxs1tLGG2xhgjyCxDK3IzMzPS7waFplK6ViaGkrycPBWtVoZfl0ACJhSOPrX75MX7EYkPT+36ZcU/KUgF6rFaQn2doLFvUBUHA6EoimCUEXNq47yt8U3HTJ8+rH0jLcTABMcgLHNq4tqvi56qMD/6lH9gcr4SYaDmMGAZhpIZW7Z0bd1YqJILHLt+2rt/r47NTY2lME9AD79qNvgOIzR3dvvUc6Knp+c348ZpkD2/8ZwwYdxA9+ZW8K7BogrlIgBJmZQW8yCgWMQQA0MdrN6dwOBB+ZEPQ+9EYGuLNl3bUHmpt3z3PUjKLhJhjF+RxLL0KwnaoFLRHBK0SqWCp1co6FfkIPAdxOanpsU+KnHs5WQjRRAuy/gYuC8ukj8NjSlSqhChZFbOrdvZ6KJiqVGrHoP+r3tHZ0dLMI6FpQJQvpxZ8OkyQf9egEgFTwzLgIUVmshUYCJwaZAxgb5GbNTepfO3BBoN/H7hjJFuRlqAU40l/quU5dpIWVoYGFlps6xQAJ0FlSydfs1nd8BD3V5jxn3Rw14CRXR8bOydixlNXFsZk8f3Hj1Oy1UigBgjOjMqNTNV2vaDRsYIIbAKYKAZmrMNxn3C41h4n2GJWGrRsq17IypPqWvu2u2joT3bODU2lwImmLw2UUCBiwL/CZdjvdaORvkxgXej02hwfgwH6Ky3DA7+xnTB6OeaWZIXffXw6h8nLj10Tth71Miu9lJYF6jB5JTLGts169ZOgovlCZf2XIjMliME+FEUhm7EIm2pnq5BcW4828S5c4tWDuZG+lKJEGpQhQkqRGYtXHsNGz7088+HfP75YA3ykKFfDBv6QbsmFjABcR1cgWCIYSgrIS3ifgpS0ii3mJaIgApK40/5bN26LahI39jEyU6iyAn1DzWzNtA1FyPYoAOSN5TBTCyVScRaWZfP34grAi1UWSIo+fLxrUuXnU0tUnKeLNYxNhQUZOdqE1vnLu4WJqYm+lIMHgYSgOstZy7cI5R5eetvS3amtB3w7cyJPSz1EQ17hnVjGBcGzJ3bNG6tl536KD2XE6rMPLd+ye5oo08n/zKuaytdzIDH0AK9Ri4fDOztUvLkRrK1fcvG9qZACvEU6xmISopjzp+NyIICXAoxoXDh4wMbN2/YHSgHD8ACSiQzttCTp+SzjRo7tXazMTEyMpBpYWV+Stjpbdu3bd68FVzklbx10+btO3dfiUkvYCg9pz6fftjRMDsuMQm17uJqhGGhydkOSusrcwOx7nVhAiOZpAT4rZ3l6TF2wsTvp8z0PhNwLz78xJoN559kFaNSgtxH1/b/MXH2hr+jChUl8sKYQ6t+/W7c2G+nbzwTGA+bxJjz14z4qHt3UgzbtLARc7Me59tV2ctyAbtGB1uZWM6MgsTE6NBoAclLizu7efby1b6+29cuXrD2WJSea7eu9mzUjf2rl/256bSiz4j2zc1liIW5oDJxtS8H10W6jew7ftI503ftDM9xP82aO2/unDlzZvz4/bjpK/fcKWns1EgiFsByBNpUeO/Ko2yhrkPLZqJSzQBq6c3bPRMKXK/w7tEVi1cEWPadMGNKf1s9BL1Xh1bBGBdadPt8yMc2VMCaGev/+nPJ1F/WXSf9pv08f3QvaylmaZZhGGxiZefSpSmKvHLspm6bzm4tm2qDDSzDEjPXTm07GoX98d3kb6f9OnvuvDmzZ8/++YcJnjN2hCRJmjtZw/ICAEaMIjvk5v1UPdumNpZ6wKrOGFNCbZlOaYLrS1lHR1cmk4opwrLCVt1bNzIquHXmzhOhc//+rbQQRm/UfdT2lT9BV5QvqMMnZaG8IC+7mBFZdfx47PdTJk0Y38VEQCuLlc8aSRcV5KbniWxa9P9+ypQpkyeP/9BeW1ScmVWgUKgAXwLGFaYnhTxO0nZyaaErFbKpsYmZKTn1vH0CVpQkJjwNvqMyMHP7aNwnzans9LjY+PikbNO+X0xbsXHFb5MG92hEZ6l0XL8a2a6RoZhlnjVQMzBhVENrNaNVU4F8rGPoOuCn6QM7GWSFXzqye5u3z57DZ2+Gpeh07OMx7ae+lhIh93aDUUn03cepWob2LZ3MUGFhbkJEggImWy6wqSVpegITNSXVhA4mVkznhRxdvnTRvmJnz1kzhrlYiCAEwAysCbumNIATa9blo4nfjx9ozcTExqWUSNwnzv5t6pBmOkKGBhw4QQQGM52ffO/86VCDdj07WajS07JTsqFDWIFZxz4jf570gUlJRMCZg95bfPb7n7h+/6nK9lPPbyYM6mjAQAhBiFWVxAbfSqYaNbN3MIHvXVlp8bE5rEDHtFn34UOHffnliBEjhr+SR4wa+cXnA91sDSXqES+/de1STDzl1svdVJH8JLlIpUTV7iKuLTU9wMVryloFH8uwAJF1X8+Z6w8e8PPe8deWjevX/rl5y+YNW3/t72SqBZUcgX7bfp7LDu719tq8fu3atevWbdiyw2eX3/6dP33W0x4znEsoM9Kjw5/IHDq42xpr5Qcev3IvPE4B64x6nNBAFZ2YEPsoMNXMpM24ZZs37/BaseB/U3/9fcOanwe52Zqadxo1f/1m7/WL5i/6toeFQATeBS5UBTgvVbE0U1JQomKqFTkYhmYE+nafzvpj++69uzavW7lq9ZoNXnsPH9w6Z9KHVrCspmkWgeUoPuRBFqvj5OJmjbLCQ8+dvJFJ04iQ6vkYo6JLCotVLPuS6TV7xASWAYVPLm/7fcFfTy1HzVr0XRcHHQQw1ExclVwcTnotPvWYt2nD4tkLV/+1fvbwTqYsA4vF520hGMHADzt77knTnh+4m2UE3njwOLoQE1gq0KyOXbfRy/18fXZ4/blqxep1G7bs3OZ1YBAAAAx/SURBVPf3vrXf9W2npxbBwahQZj26Gy1u0rS1YzNR7v3rNy7ejC8BbgZ0A1HVmUGgCBXcPXcjjtXt089dEnXjREB8Ic0Q6KMqW1anlW8mCpSaCDgwDMwizLPEqm9gM6y0nut5BgiY8klNRZeSlCiUeUWFRTpIHnnvzsVL6Vr6EnNzimWe92Ep2Zs8A0JZT+IigqP1TQw7tLIrAdVEIJGIiNpq6GS4QiOFQohbDK2OXRqbA3xEW9/SuZeLlUxGwZPGnEAIvgyqiYFVy66fjBgy6LMeLpb6YhaKSic5iAFgamGuPE+MVMr0yDtn74YlkKZNJAIBqoYmIBUZmjRu3aOloZYQwxNork2GEICV6ff2rVmz+Y7uiNmLf+nrqENYutTmmgmGlQXFJWhxBQI42QzDEi2xiHDoMHR57wEuVV5hXFo0Y2euFX7nXqKK0jIzo9QtZcEu4BVbOrp+MMRjUP/eHZvA7iVIgVDKqQJemMsLCvNVQiGVmRoWdiEgM402bmYKyCNuMcYRVX1gkJEbF50qxTJdZV7w3fvF9rYSgRZmy1tZtZDa1oKP11ZE5fyAJMswMM65GzhK716k5wpLS+GuLKufOSKAUmpi3a5bf3uUcPWy/7Hk9h+3a+Nii0AiV10/BwCkSohLeBwpMDVq0bqpCKYOMICBpDYXjIArPEGGG3isTgYmoUlTt/FbJna3suRWSNVhBlrQyNAgBK4shzTcsyzABlUw0rnFgF37Pm4t7fNCDh29nsqYDPBwk2ABUJbRcHSvOUC6tIVrv+82f+NqKOEi32voq6yG8YqZgpjj6/9cfzKl7Xe/zfyklYzbKmaq5Kq6ElO4OCMtDV7QaFQJJWACzeAy3L3cdHjW0tdv3bW3o1bh7eOBojb2jR1LfzuIuAQcHCPDeSVTlp5BrN4DFgst2/bt0tik8NHp3f9kmDh0GNIdVhvABoI5Aa85OFnGzTp27dAMPboV/DjLfkA3Q7EQZhTN2F8jXcNqcHINKeufjJvs9Jr0GbHYd+XEoZ4/TBvV07GRNmJgrVt/tkCoZhJiYkIf0MYGth2dTSh4i+Q6ru4swLBCpigCimooExxO7Z1wfVECy8I6hZa0Gbd6waw5cyd/5fH1l31tRFwEq7Z/lZpYcwvLzCKwGaZIubhhxcq9N8yGTV/ybWdDCoOV1banTB53AeSYlGvb1qxduvt+CUUgwdzKVWh8cF5mZNnRY6XX3K89Z/40xM3FWghl5fgBWgidDHcpbyxAjAQ6bUas2jJv0vjp/xs7fEjX5hzGmq0DQAfLgi6B69hJk+dvWuD5xbiv+lshqpaYgNhq5nc5CkBTWERpSXTNLG3MTIz1pDARs/W5UEIIAz656akZqfl2jZt07eiABBixDKrLpPYDGjysLoX+K4sS6xuZW1haG+vLtMW4ei8sz6SUmli74EcoGPH51zcuXbzhtHb/CQtnDGksoGAI1BxMDCsLCrHy6957Q6IjbTp3KNvbf2a15lfYbhZKdMwsrC1NjWRCgqvpY1gg1jUytTY3NzPUEQthvVQ+UrzeDpYSywzNLGysTPQlYvUC4/U8dUoBXl6n8upaGPgJxFsYI3CGl7Tq4ltbc1iGYaQtPp265oz/hvmDmxOGK6it0Hrlh6mGhkZwF7peV1EvthLGK0zRUX4rl286wX44bt6cse11hbCHWc3hViYSQyIEJn6EmHC/VSs3XMwwd+vTUQq9U8NIpQ5zDHQueBlcyvRoemE5cBlIwE3XaIPjmQDuWt8uzrXyXY8CnI0IsTXs3VLu2pxBs0DHpoVL17ZtmuhpMfD4NnqpNi0A3rdrNYQA8LL8gG2L//BNbDNwyuzvuplIETg8WKZRhkH/QiaEEMK9QOVHHfpt2g9z157A9k3b93GBT6OV/fZTIy2ck9Wib2uNMSegFvo1a2MlVNA/ldTwxWUIwFsaxHkG3Lbsw0VZOX/RAAHY9AAXy76ya878pYE2fb+d/evARuqf1hBK41Q67p+dMZMadtV/xawJnpPnrt/+T1SWVbf23dxaihG8qb2tUaQBEO80CXTRO23fu2Hc24zT7wYCNbOCUASjoodHf1+5fE+SVZ9BQ7uYsglxT6OfapJjY2KfRkfeDzh/9uTxk4d3e29dOX/R3Bk/T5v608y5C1eu3brvVFiugkE23ds6t7cXw7ZnzWzkuRDiowDvBW8IAUwozBTGBf61dNmWM+FFSJB8bu8fs378ddZczdKcOXM4QvVp7tx58+bNXTBn4bIVa/70OXopJJeWQKKUVNNebZ3cbQXorb0zviH06lUsHwXqFe6GowxjwspTQo7+sXSF7408hUrx6OIhX+5/qt3j67PbR8Pss3vv0YvXg+7cvRMaFZteIhAJhGIhl+FbnrJYUVKMm37Swal1YyGC14GGg22dt5SPAnUOKS+QQwBjli7IzMkuMvhw9MgxY8d+NWbsuLFjx40Zw53hpvp57GiP0R6jPEaV5i9He8DjxEmfurUwQywfBDjMa3zwUaDG0PGMVSEAG6rEuGW3iVu9vbx9vLZv/6s079hRdlP6WPPzjm07d3jt2jipT3tLFj6FVmUKX/c6BPgo8DqE+Pp3GgF+P6AOuoePAnUAIi+iEgRgpa7+Jc3rTrWoZ/gwUAn41Sjmo0A1wOJJeQTeSwT4KPBedus73Cj4eKD+6V9NTeR+RkhAQk35eb5XEeCjwKuY8CVvDAFMKEK4cYyoGujAhFAUgYQK8hUMzYCgGkjhWV5BgI8Cr0DCF7whBDAhOO+x/6qfxvyy6EgkC6OZYE1VYYIxpcrPiA8+4ffHgmm/7g7MKGQI0ZhfUz0Nk46PAg2z399OqzFGBalJqWnpcpG4Op4HiwA6K/JWwD/nAm7fCjrls/PAjch8JYsQHwVQXaTq9EVd6ONlNGAEYMzqOQ2a9NuaWf/rx/3JKEbzf1nMwrcARiAztmrq5GxvYKyvLeTXAXXnSXwUqDsseUmVIoAR90ZfmBoXnSIybdTMwZJS/60DjGGW594MqjiABrEMQxm3cOv2cd9uLrZWEhaxkBCf6goBPgrUFZK8nH8RKH8HQ52lmIyY4HtBZ4/67zty4nZqIcKwMEAMw/2fTKoq07MfBjKlf/FTSavjR3kN/FPtEOCjQO3w47lfiwAmmFYWhBzacfKxSkuZfPbw2rUnnsIagKWVWclxT2Oio2JioivN0Sk5BSUMUQcN2Ah4rTaeoAYI8FGgBqDxLNVAgBBEK5kngdkterdv5SCSZ+bQMkNdEMAoirPiY6Oio6KiYyAQVJCjIUBEJeYWKhiIJMDB5zeEAB8F3hCwvNgyBGAljwUiu8++HuxmL78e+JDoN+3lZgmVlLbMvm3nHj169erRvVf3ijLUde/VxsZYJqDpmv+VUlDF56oR4KNA1fjwtVUhoGkdRelZm2gp7l24Fs2YOH/Y3YIglkGEiLS0tLW1JXBUnrWEFO+kmgJdQzoe4BoCx7NpjgDG3FagPOhYULzEpl0XFzYp4sbDzJK0mGPzx4wa8smggYOHDq4gfz5g4NDBX8w6cC26iBACIiDDriJ3Rty19AbxqdYI8FGg1hDyAl6DAMbceM26d+Z2plG7Ln1sFLGhl+4USwRSg6ZdP/ls0NBBgwcNHFRRHjJ4wKAB3Zpb6wvgwyCm1D861pFIxARjkZZMRwx6KYr3YIChlpnHsJYA8uwaIoBLlEUivexbJy9cvRVn4N5EKtQxbPnB0GGjxowe7fGlRwV51OjRozy+7O/S2FiEMZZHnP977beTJi9ccig0Jub4xl8mT5q+zDcgOhU+N3BRRkMzeLIKEOCjQAWg8EUvIVC7R5aBqZzVdRr67ZjP3FroGNs1d+3pqsfAtqGmf1eA5QwgFEWJRAYOzoP+98vPn3cy19MWCgiF+QjAgVO7g48CtcOP59YEAQYSMu00etSI8b9O/bz/h+1MaLpafx0E+KVNen72/drVK5atWrl08aLlK3+H/OPITvamLKP5D5E1MbYB0pAG2Ga+yW8FAZpmGAyfBhhuEVB9C1hYODAvJ66s+qJ4jpcQ4KPAS4Dwj28OAe7FgDtqrIFjLnfUWBLP+CICfBR4EY2Gfs+3v2EiwEeBhtnvfKt5BP5FgI8C/2LB3/EINEwE+CjQMPudbzWPwL8I8FHgXywazh3fUh6BFxHgo8CLaPD3PAINEQE+CjTEXufbzCPwIgJ8FHgRDf6eR6AhIsBHgfe51/m28QhoggAfBTRBiafhEXifEeCjwPvcu3zbeAQ0QYCPApqgxNPwCLzPCPw/AAAA//+QZ3YNAAAABklEQVQDAIcYoDErAKv3AAAAAElFTkSuQmCC" alt="embedded_DR_48_Keys_img_1.png" style="max-width: 100%; height: auto; margin: 16px 0;" />

### [3년치 기출, KPC 모의고사] 데이터 관측가능성(Data Observability)

**[정의]**  

-  데이터 파이프라인 전반에서 데이터의 상태·품질·이상 징후를 지속적으로 관찰·이해·문제 원인을 추적할 수 있는 능력  

**[핵심/키워드]**  

&lt; 기술요소&gt;  
* AI/ML&기반 자동화된 이상 탐지  
* Lineage 매핑, 실시간 알림(Alert)  
* 메타데이터 수집  
* 프로파일링  
* 데이터 거버넌스  

### [3년치 기출, KPC 모의고사] 정보모델링의 참조 무결성

**[정의]**  

-  외래 키(Foreign Key)가 참조하는 기본 키(Primary Key)의 값이 항상 유효하도록 보장하는 규칙  

**[핵심/키워드]**  

&lt; 유형 &gt;  
* 입력 참조 무결성 : 의존, 자동, 기본, 지정  
* 수정 참조 무결성 : 제한, 연쇄  
* 삭제 참조 무결성 : 제한, 연쇄 , 기본, 지정  

### [3년치 기출, KPC 모의고사] TTPs(Tactics,Techniques and Procedures)

**[정의]**  

위협 행위자 또는 위협 행위자 그룹의 패턴, 활동 및 방법을 의미하며, 사이버 범죄자의 공격 수행 방식  

**[핵심/키워드]**  

&lt;요소&gt;  
* Tactics (전술) : 공격 단계에서의 목표/의도  
* Techniques (기법) : 전술을 달성하기 위한 방법  
* Procedures (절차) : 특정 공격자가 수행한 구체적인 실행 절차  

### [3년치 기출, KPC 모의고사] 은행가 알고리즘

**[정의]**  

운영체제가 자원의 상태를 감시하는 상태에서 프로세스가 필요 자원을 요청할 때 사전에 안전 여부를 검증하는 교착상태 회피 기법  

**[핵심/키워드]**  

&lt;자료 구조&gt;  
Available – 사용 가능한 자원의 양  
Max – 각 프로세스가 최대 요청할 수 있는 자원의 양  
Allocation . 현재 각 프로세스에 할당된 자원의 양  
Need . 프로세스가 실행을 끝내기 위해 추가로 필요한 자원  

### [3년치 기출, KPC 모의고사] 프롬프트 인젝션(Prompt Injection)

**[정의]**  

악의적 또는 조작된 입력을 통해 LLM의 지시문·정책·제약을 우회하거나 변경하여 비의도적 출력을 유도하는 보안 취약점  

**[핵심/키워드]**  

&lt; 유형 &gt;  
* 직접 인젝션, 간접 인젝션, 탈옥  
&lt; 절차 &gt;  
1\. 프롬프트 인젝션 삽입  
2\. 사용자 검색  
3\. 데이터 조회  
4\. 시스템 프롬프트 구성  
5\. 인젝션된 결과 전달  
&lt; 대응 &gt;  
* 입력값 검증, 권한 최소화, 시스템 프롬프트 강화, 보안 업데이트, 보안 가드레일  
&lt; 연관 &gt;  
* OWASP LLM TOP 10  

### [3년치 기출, KPC 모의고사] 선택 정렬(Selection Sort)

**[정의]**  

전체 원소중에서 가장 작은 원소를 찾아서 첫번째 원소와 자리를 바꿈  

**[핵심/키워드]**  

&lt;특징&gt;  
*가장 작은 값을 선택하여 앞에서부터 하나씩 확정해 나가는 정렬 방식  

### [3년치 기출, KPC 모의고사] 삽입 정렬(Insertion Sort)

**[정의]**  

현재 값을 그보다 앞에 있는 정렬된 부분과 비교하여, 알맞은 위치에 삽입해가며 정렬하는 알고리즘  

**[핵심/키워드]**  

&lt; 특징 &gt;  
* 정렬된 앞쪽 비교, 제자리 정렬, 안정 정렬  
&lt; 복잡도 &gt;  
* 최선 O (n), 최악, 평균 O (n의 제곱)  

### [3년치 기출, KPC 모의고사] SRP(Single Responsibility Principle)

**[정의]**  

SRP ( 단일책임 원칙)  
- 객체(클래스)는 하나의 책임(기능)만 가져야 하며, 변경되어야 하는 이유도 하나뿐이어야 한다  

**[핵심/키워드]**  

&lt;장점&gt;  
* 높은 응집도(High Cohesion) 확보  
* 낮은 결합도(Low Coupling) 실현  
* 유지보수 및 테스트 용이  
&lt;적용 사례&gt;  
* MVC에서 Controller, Service, Repository 분리  
* MSA에서 서비스별 책임 분리  
* 클린 아키텍처의 계층별 역할 분리  

### [3년치 기출, KPC 모의고사] DIP(Dependency Inversion Principle)

**[정의]**  

DIP(의존성 역전 원칙)  
-  고수준 모듈(비즈니스 로직)이 저수준 모듈(구현 클래스)에 직접 의존하지 않고,  
둘 다 추상화(인터페이스, 추상 클래스)에 의존하도록 설계하는 객체지향 설계 원칙  

**[핵심/키워드]**  

&lt;장점&gt;  
* 결합도(Coupling) 감소  
* 유연한 구현 교체  
* 확장성 향상(OCP 지원)  
* 단위 테스트(Mock 객체 활용) 용이  
&lt;적용 사례&gt;  
* 인터페이스 기반 설계 적용  
* DI(Dependency Injection) 프레임워크(Spring) 활용  
* Mock 객체를 이용한 테스트 자동화  

### [3년치 기출, KPC 모의고사] IT감사 가이드라인(2025.02)의 IT 내부통제 체계

**[정의]**  

금융회사의 IT내부통제 체계 강화 및 IT감사 업무의 체계적 수행을 위해 금융감독원이 마련한 권고 기준  

&lt; IT 내부통제 체계 &gt;  
다층적 통제를 통해 통제 부실 방지 및 책임성 강화위한 3단계 유기적 구조 체제  

**[핵심/키워드]**  

&lt; 3단계 유기적 구조 &gt;  
① IT조직의 자체통제  
② IT자체감사  
③ 감사조직의 IT감사  

### [3년치 기출, KPC 모의고사] OWASP Top 10 for Agentic Applications 2026

**[정의]**  

- 자율적으로 계획, 도구를 사용하고, 메모리를 활용하며, 다른 에이전트와 협업하는 Agentic AI 시스템의 보안 위험을 정리한 프레임워크  

**[핵심/키워드]**  

&lt;전체 목록 &gt;  
1  ASI01 Agent Goal Hijack 에이전트 목표/의사결정 경로 탈취  
2  ASI02 Tool Misuse and Exploitation  정당한 도구의 악의적 사용  
3  ASI03 Identity and Privilege Abuse  동적 신뢰/위임을 악용한 권한 상승  
4  ASI04  Agentic Supply Chain Vulnerabilities 서드파티 에이전트 컴포넌트의 악성/변조  
5  ASI05  Unexpected Code Execution (RCE)  에이전트 코드 생성/실행 경로 악용  
6  ASI06  Memory & Context Poisoning 저장/검색된 컨텍스트 오염  
7  ASI07  Insecure Inter-Agent Communication  에이전트 간 통신의 인증/무결성 부재  
8  ASI08  Cascading Failures 단일 장애의 시스템 전체 전파  
9  ASI09  Human-Agent Trust Exploitation  인간의 에이전트 신뢰를 악용  
10 ASI10 Rogue Agents 악성/손상된 에이전트의 범위 이탈  

### [3년치 기출, KPC 모의고사] PS-Satcomm

**[정의]**  

- 기존 PS-LTE를 저궤도  위성통신과 결합하여, 재난·재해 상황에서도 끊김 없는 공공안전 통신을 제공하기 위한 차세대 재난안전통신망  

**[핵심/키워드]**  

&lt;주요 기술 요소 &gt;  
* LEO Satellite : 저지연 위성통신 제공  
* D2C (Direct-to-Cell) : 스마트폰이 기지국 없이 위성과 직접 통신  
* Network Slicing : 재난 발생 시 구조 통신에 우선 대역폭 할당  
* Multi-Orbit : LEO·MEO·GEO 연계로 통신 연속성 확보  
* 05G-Advanced / 6G NTN : 비지상망(Non-Terrestrial Network) 기반 서비스  
* KASS/GPS 연계 : 구조 대상자의 정밀 위치 제공  

### [3년치 기출, KPC 모의고사] PS-LTE

**[정의]**  

- LTE 기술을 기반으로 경찰·소방·해양경찰·군·지자체 등 재난 대응 기관이 하나의 통합망에서 음성·영상·데이터를 실시간으로 공유할 수 있도록 구축된 국가 재난안전통신망  

**[핵심/키워드]**  

&lt;특징&gt;  
* 기관 간 상호운용성 : 경찰, 소방, 해경, 군, 지방자치 등  
* Mission Critical 서비스 :  
* LTE 광대역  
* 우선순위(QoS) 적용 : 재난에 우선 적용  

### [3년치 기출, KPC 모의고사] 기술부채(Technical Debt)

**[정의]**  

- 단기적인 개발 일정이나 비용 절감을 위해 최적의 설계나 구현 대신 임시방편의 해결책을 선택함으로써, 향후 유지보수·확장·품질 개선 시 추가적인 비용과 노력이 발생하는 상태  

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
* Data Debt 데이터 품질 저하, 편향, 불균형  
* Model Debt 모델 노후화, Drift, 과적합  
* Feature Debt Feature 중복, 관리 어려움  

### [3년치 기출, KPC 모의고사]  AI 레드팀(AI Red Team)

**[정의]**  

&lt;정의&gt;  
- 인공지능 시스템(특히 LLM,생성형 AI등)에 대해 의도적 공격·취약성 검증을 수행하는 전문팀  
- 사이버보안에서의 ‘레드팀(공격 모의팀)’ 개념을 AI시스템 검증에 확장 적용한 것  

- 조직측면 : 인공지능(AI)시스템의 보안과 윤리적 취약점 점검,실전 환경에서 테스트하기 위해 구성된 조직  
- 활동측면 : AI시스템의 편향,보안 문제 등을 발견하기 위해 공격자 입장에서 의도적으로 시스템을 테스트하는 활동  

**[핵심/키워드]**  

&lt;주요 역할&gt;  
- 취약점 탐색 :프롬프트 주입, 데이터 오염  
- 윤리적 문제 및 편향성 점검 :편향 응답 확인, 개인정보 유출 확인  
- 신뢰성 및 안전성 강화 :발견 문제 방어전략 수립  
- 공격 시나리오 모의 실험 :AI기반 공격 시나리오 시뮬레이션  

- AI블루팀 : AI시스템과 네트워크를 사이버 위협으로부터 방어 하는 역할  
- AI퍼플팀 : 레드팀과 블루팀의 협력을 촉진 하고 통합하는 역할&lt;실행 단계&gt;  
– 목표 정의: 평가 대상(모델·데이터·API·운영환경)과 검증 목표(보안·안전·신뢰·규제)를 명확화  

– 공격 시나리오 설계: 프롬프트 인젝션, 탈옥, 데이터 중독, 적대적 입력, 모델 추론·오남용 등 공격 벡터 정의  

– 테스트 세트 구축: 공격 유형별 테스트 케이스·프롬프트·자동화 스크립트 구성  

– 공격 실행: 수동·자동 공격 수행, 탐지·차단 여부 및 로그 수집  

– 영향 분석: 성공 여부, 영향 범위, 재현성, 위험도 평가  

– 재검증 및 개선: 블루팀 대응 적용 후 재테스트, 잔존 리스크 식별 및 개선사항 도출  

### [3년치 기출, KPC 모의고사] PWA(Progressive Web App)

**[정의]**  

- 웹  기술(HTML, CSS, JavaScript)을 기반으로 개발하면서도 네이티브 앱(App)과 유사한 사용자 경험(UX)을 제공하는 웹 애플리케이션  

**[핵심/키워드]**  

&lt;구성요소&gt;  
(1) Service Worker  
* 백그라운드에서 실행되는 JavaScript  
* 캐시(Cache) 관리  
* 오프라인 지원  
* 백그라운드 동기화  
* 푸시 알림 제공  
(2) Web App Manifest  
* 앱 이름 , 아이콘 , 시작 URL , 화면 방향 , 테마 색상  
(3) HTTPS  
* Service Worker는 HTTPS 환경에서만 동작  
* 데이터 위·변조 방지  

### [3년치 기출, KPC 모의고사] 가상메모리 단편화

**[정의]**  

- 메모리 할당과 해제가 반복되면서 사용 가능한 메모리 공간이 비효율적으로 분산되어 메모리 활용률이 저하되는 현상  

**[핵심/키워드]**  

&lt;유형&gt;  
* 내부 단편화 (Internal Fragmentation)  
고정 크기의 메모리 블록을 할당할 때, 실제 필요한 크기보다 크게 할당되어 블록 내부에 사용되지 않는 공간이 발생하는 현상  
-→ 발생환경 : 페이징(Paging)  , 고정 크기 블록 할당  
-→ 해결방안 : 페이지 크기 최적화, 가변 페이지(Huge Page 등) 활용  
* 외부 단편화 (External Fragmentation)  
메모리 할당과 해제가 반복되면서 빈 공간이 여러 곳에 흩어져, 총 여유 공간은 충분하지만 연속된 큰 공간이 없어 메모리를 할당하지 못하는 현상  
-→ 발생환경 : 세그멘테이션(Segmentation) , 가변 크기 메모리 할당  
-→ 해결방안 : 메모리 압축(Compaction), 페이징 사용, Buddy System  

### [3년치 기출, KPC 모의고사] 모델 전도 공격(Model Inversion Attack)

**[정의]**  

- 머신러닝 모델의 출력이나 파라미터를 이용하여, 모델이 학습했던 개인정보, 이미지, 텍스트 등을 역으로 추정해내는 공격 기법  

**[핵심/키워드]**  

*주요기법  
이미지 데이터 : 출력기반, 최적화 기반, Feature Inversion , GAN 및 Diffusion 기반  
텍스트 / 일반데이터 : 파라미터 기반, Query-efficient  
생체정보/ 임베딩데이터 : Embedding Reconstruction , Gradient&기반 , Hybrid&방식  

### [3년치 기출, KPC 모의고사] ISP

**[정의]**  

- 정보기술이 경영전략의 수립과 실행을 지원할 수 있도록 통합 정보시스템 구축을 위한 마스터플랜을 마련하고,장기적 관점에서 정보시스템의 발전 청사진(To-Be모델)을 제시하는 활동  

**[핵심/키워드]**  

환경분석 → 현황분석 (AS-IS) → 미래모형 설계 → 실행계획 수립  

### [3년치 기출, KPC 모의고사] GPU

**[정의]**  

- 컴퓨터 모니터에 픽셀(화소)로 투영되는 그래픽 처리를 위해 FLOPs(부동 소수점 연산)기반 병렬 처리 특화 처리 장치  

**[핵심/키워드]**  

&lt;구성 요소 &gt;  
* Streaming Multiprocessor(SM) : 다수의 연산 코어를 관리하는 실행 단위  
* CUDA Core / Stream Processor : 범용 병렬 연산 수행  
* Tensor Core : AI 행렬 연산(FP16, BF16, INT8 등) 가속  
* RT Core : 실시간 Ray Tracing 연산  
* HBM/GDDR : 고대역폭 메모리 제공  

### [3년치 기출, KPC 모의고사] TPU

**[정의]**  

- Google이 딥러닝 연산을 가속하기 위해 개발한, 행렬곱과 벡터연산(텐서연산)을 초고속 수행하도록 설계된 특수 목적형 하드웨어  

**[핵심/키워드]**  

&lt;주요 구성 요소&gt;  
* MXU(Matrix Multiply Unit) : 대규모 행렬 곱셈 전담 연산 장치  
* Vector Unit : 벡터 연산 수행  
* Scalar Unit : 제어 및 일반 연산 수행  
* HBM : 고대역폭 메모리  
* Interconnect : TPU Pod 내 TPU 간 연결  

### [3년치 기출, KPC 모의고사] 재공학

**[정의]**  

- 기존 시스템을 널리 사용되는 프로그래밍 표준에 맞추거나 타 하드웨어에서 사용할 수 있도록 변환하는 기법  

**[핵심/키워드]**  

&lt;현대적 재공학&gt;  
* 최근에는 단순 구조 개선에서 디지털 전환(DX) 중심의 재공학으로 발전  
→ 클라우드 전환  
→ MSA 전환  
→ AI 기반 재공학  
* AI 기반 재공학은 LLM을 활용한 코드 분석, 자동 문서화, 테스트 케이스 생성, 코드 변환을 통해 레거시 시스템의 클라우드 네이티브 전환과 디지털 혁신 지원  

### [3년치 기출, KPC 모의고사] 역공학

**[정의]**  

- 이미 구현된 소프트웨어의 개발 단계를 역으로 분석하여 처음의 문서나 내부 구조,동작 원리,소스 코드 등의 자료를 얻어내는 기법  

**[핵심/키워드]**  

&lt;주요 기술&gt;  
* 소스코드 분석 : 코드 구조, 함수, 클래스 분석  
* 정적 분석(Static Analysis) : 실행 없이 코드 분석  
* 동적 분석(Dynamic Analysis)	: 실행 중 동작 분석  
* 디컴파일(Decompiler) : 실행 파일 → 고급 언어 복원  
* 디스어셈블(Disassembler) : 기계어 → 어셈블리 코드 변환  
* 모델 추출 : UML, ERD 등 설계 산출물 생성  

### [3년치 기출, KPC 모의고사] 로우코드

**[정의]**  

- 최소한의 코딩지식만으로 코딩이 가능하도록 작업 간소화하여 개발 업무의 접근성을 확대하고, 업무 효율을 높이는 개발방식  

**[핵심/키워드]**  

&lt;기술 요소&gt;  
* Visual Modeling : Drag & Drop 기반 화면·프로세스 설계  
* Workflow Engine : 업무 프로세스(BPM) 자동화  
* Component Library : UI 및 기능 컴포넌트 재사용  
* API Integration : REST/OpenAPI 등을 통한 외부 시스템 연계  
* Custom Code : 복잡한 비즈니스 로직 확장  
* DevOps 연계 : CI/CD 기반 자동 배포  

### [3년치 기출, KPC 모의고사] 공격 표면(Attack Surface)

**[정의]**  

- IT 환경에서 공격자가 접근·탐색·악용할 수 있는 모든 노출 지점(자산·경로·정보)의 총합  

**[핵심/키워드]**  

&lt;공격 표면과 벡터 비교 &gt;  
* 공격 표면 (Attack Surface) : 공격 가능한 모든 대상·진입점  
* 공격 벡터(Attack Vector) : 실제 공격에 사용되는 경로·기법  
&lt;사례&gt;  
* 웹 서버, API, VPN, AI 모델  

### [3년치 기출, KPC 모의고사] 공격 벡터(Attack Vector)

**[정의]**  

- 공격자가 공격 표면을 활용하여 침투 또는 권한 획득을 수행하는 구체적인 공격 경로와 수단(방법)  

**[핵심/키워드]**  

&lt;사례&gt;  
피싱, SQL Injection, RCE, Prompt Injection  
&lt;주요 공격벡터&gt;  
* 네트워크 : DDoS, MITM, DNS Spoofing  
* 웹 : SQL Injection, XSS, CSRF, SSRF  
* 인증 : Brute Force, Credential Stuffing, Pass-the-Hash  

### [3년치 기출, KPC 모의고사] 측면 이동(Lateral Movement)

**[정의]**  

- 지능형 위협 공격(APT)과정 중 공격자가 조직 내 최초 시스템 해킹에 성공 후 내부망에서 사용되는 계정 정보를 획득하여 내부망의 시스템으로 이동하는 방식  

**[핵심/키워드]**  

* MITRE ATT&CK에서는 Lateral Movement를 독립 전술(Tactic)로 정의  
&lt;공격 기법&gt;  
* Remote Services : RDP, SSH, SMB 이용  
* Remote Desktop Protocol : 원격 데스크톱 악용  
* PsExec : Windows 원격 실행 도구 악용  
* SMB/Windows Admin Shares : 공유 폴더를 통한 이동  
* SSH : 리눅스 서버 간 이동  

### [3년치 기출, KPC 모의고사] 단방향 해시함수

**[정의]**  

- 입력데이터를 고정된 길이의 해시값(Hash&Value)으로 변환하는 단방향 함수  

**[핵심/키워드]**  

&lt;암호학적 특징&gt;  
* 역상 저항성 : 해시값으로 원문을 찾기 어려움  
* 제2 역상 저항성 : 같은 해시를 만드는 다른 입력을 찾기 어려움  
* 충돌 저항성 : 서로 다른 두 입력이 동일한 해시를 만들기 어려움  

### [3년치 기출, KPC 모의고사] 키스트레칭

**[정의]**  

- 해시 함수를 수천에서 수만 번 반복하여 암호화된 데이터(다이제스트)를 생성하는 보안 기술  

**[핵심/키워드]**  

① 입력: 사용자의 비밀번호와 솔트(Salt)를 결합  
② 해싱: 결합된 값을 해시 함수에 넣고, 그 결과값을 다시 해시 함수의 입력값으로 사용하는 과정을 수천 번 이상 반복  
③ 최종 저장: 수많은 반복 끝에 도출된 최종 해시값(Stretched&Key)을 데이터베이스에 저장  

### [3년치 기출, KPC 모의고사] 자율 최적화(Self-Optimization)

**[정의]**  

- 네트워크가 실시간으로 수집되는 빅데이터를 AI모델로 분석하여,사람의 개입 없이 스스로 자원 할당,파라미터 조정,장애 복구 등을 수행하는 기술  

**[핵심/키워드]**  

&lt; 기능&gt;  
* Self-Configuring	자동 구성 및 설정  
* Self-Healing	장애 자동 감지 및 복구  
* Self-Optimizing	성능·자원 자동 최적화  
* Self-Protecting	위협 탐지 및 보안 강화  

### [3년치 기출, KPC 모의고사] AI-RAN

**[정의]**  

- 무선 접속망(RAN)전 영역 AI 내재화. 무선 자원 전체 종단 간(End-to-End) 제어하고 지능적 최적화 차세대 무선 접속망 기술  

**[핵심/키워드]**  

&lt;기술 요소&gt;  
* AI/ML : 트래픽 예측, 장애 예측, 자원 최적화  
* GPU/NPU : AI 추론 및 학습 가속  
* vRAN / Cloud RAN : RAN 기능의 가상화 및 클라우드화  
* Open RAN : 개방형 인터페이스 기반 RAN  
* RIC(RAN Intelligent Controller) : AI 기반 RAN 제어  
* Edge Computing : 저지연 AI 서비스 제공  

### [3년치 기출, KPC 모의고사] 오류 검출

**[정의]**  

- 데이터 수신측에서 오류가 있음을 검출만 하는 기법  

**[핵심/키워드]**  

CRC, Checksum, Parity Bit  

### [3년치 기출, KPC 모의고사] 오류 정정

**[정의]**  

- 오류 검출 후 자체적으로 수정까지 하는 기법  

**[핵심/키워드]**  

- 전진 오류 수정(FEC)  
- 후진 오류 수정(BEC): ARQ  

### [3년치 기출, KPC 모의고사] 정지-대기(Stop-and-Wait) ARQ

**[정의]**  

- 하나의 프레임 전송 후 ACK 수신 시 다음 프레임을 전송하는 방식  
- 한번에 한 개의 프레임만 전송하고 ACK 미전송 시 재전송하는 방식  

**[핵심/키워드]**  

① 데이터 1에 대한 ACK&수신 후 데이터 2 전송(한 개씩 전송)  
② 데이터 3에 대한 NAK&수신 시 3 재전송  
. 에러가 없을 경우 송신측에게 ACK 전송  
. 에러가 있는 경우 NAK를 전송하여 재전송 유도  
. 하나 보내고 하나 확인 후 다시 전송  

### [3년치 기출, KPC 모의고사] Go-Back-N ARQ

**[정의]**  

송신측에서 프레임을 연속 송신하고, 수신측은 오류 발생 시 NAK와 오류 프레임번호 송신, 송신측은 오류 프레임부터 재전송하는 방식  

**[핵심/키워드]**  

-전송 효율 높음 (프레임 연속 전송으로, 채널 이용률 향상)  
- 오류 프레임부터 재전송 (오류 발생 시 이후 프레임 모두 재전송)  

### [3년치 기출, KPC 모의고사] 랜섬웨어

**[정의]**  

ransom(몸값)과 ware(제품)의 합성어,컴퓨터에 저장된 파일들을 암호화하여 사용자가 읽을 수 없는 문자들로 바꿔버린 후, 암호화를 풀어주는(복호화) 대가로 금전(몸값)을 요구하는 악성프로그램  

**[핵심/키워드]**  

&lt;주요 공격 기법&gt;  
* 파일 암호화  
* 데이터 탈취  
* 이중 갈취  
&lt;주요 공격 경로 &gt;  
* 피싱 메일 , 취약점 공격 , 공급망 공격 , 악성 광고  

### [3년치 기출, KPC 모의고사] RaaS

**[정의]**  

랜섬웨어의 변형으로, 랜섬웨어를 제작 및 배포하려는 사람을 위해 고안된 일종의 주문 제작 대행 서비스  

**[핵심/키워드]**  

&lt; 최신 RaaS 동향 &gt;  
* Double Extortion : 암호화 + 데이터 유출 협박  
* Triple Extortion : 고객·협력사까지 협박  
* Initial Access Broker(IAB)와 연계하여 침투 경로 구매  
* AI 활용 : 피싱 이메일 생성, 악성코드 난독화 자동화  
* 공급망 공격 : 협력업체를 통한 대규모 감염  

### [3년치 기출, KPC 모의고사] B-Tree

**[정의]**  

- 데이터를 정렬된 상태로 저장하면서, 검색, 삽입,  삭제를 모두 빠르게 처리할 수 있도록 설계된 트리 구조  

**[핵심/키워드]**  

&lt;특징&gt;  
* 다중 분기 구조 (한 노드가 여러 키와 자식 가짐)  
* 균형 유지 (모든 리프 노드가 같은 깊이로 유지됨)  
* 정렬 유지 (항상 키 값이 오름차순 정렬 상태 유지)  
* 빠른 탐색 (루트부터 리프까지 log(n)단계로 탐색)  
* 효율적 디스크 접근 (한 노드에 여러 키 저장 →I/O최소화)  

### [3년치 기출, KPC 모의고사] B+Tree

**[정의]**  

- B-트리를 확장한 인덱스 구조로,  내부 노드에는 키만, 리프 노드에만 실제 데이터(또는 포인터)를 저장하는 균형 다진 검색 트리  

**[핵심/키워드]**  

&lt;특징&gt;  
* 정렬된 리프 노드 연결 (범위 검색에 유리)  
* 내부 노드는 탐색 전용 (데이터는 리프에만 존재)  
* 균형 트리 유지 (모든 리프 노드는 동일한 깊이)  
* 빠른 범위/순차 검색 (리프 노드 연결로 전체 탐색 최적화)  
* 낮은 트리 높이 (다진 구조로 검색 경로 짧음)  

### [3년치 기출, KPC 모의고사] 태스크 우선순위 상속(Priority Inheritance)

**[정의]**  

- 우선순위 역전 방지 위해, 공유 자원을 점유한 낮은 우선순위 태스크가 높은 우선순위 태스크의 우선순위를 일시적으로 상속받아 먼저 실행되도록 하는 동기화 기법  

**[핵심/키워드]**  

&lt; 장점 &gt;  
* 우선순위 역전 해결  
* 실시간 응답성 향상  
* Deadline 충족 가능성 증가  
&lt; 단점 &gt;  
* 구현 복잡성 증가  
* 여러 개의 Mutex를 사용할 경우 관리가 어려움  
* Deadlock 자체는 해결하지 못함  

### [3년치 기출, KPC 모의고사] 정적 SQL(Static SQL)

**[정의]**  

- SQL 문이 프로그램 작성(컴파일) 시점에 미리 정의되고 검증되는 SQL 방식  

**[핵심/키워드]**  

&lt;장점&gt;  
* 실행 속도 향상 (Parse 및 Optimize 과정 최소화)  
* 문법 오류를 컴파일 시 발견  
* 실행 계획 재사용  
* SQL Injection 방지에 유리  
* 프로그램 안정성 향상  
&lt;단점&gt;  
*SQL 구조 변경이 어려움  
* 다양한 조건을 처리하기 위한 유연성 부족  
* 프로그램 수정 후 재컴파일 필요  

### [3년치 기출, KPC 모의고사] 동적 SQL(Dynamic SQL)

**[정의]**  

-  프로그램 실행(Runtime) 시점에 SQL 문을 동적으로 생성하고 실행하는 SQL 처리 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
* 실행 시 SQL 생성 : Runtime에 SQL 구성  
* 높은 유연성 : 조건, 컬럼, 테이블 변경 가능  
* 복잡한 검색 지원 : 다양한 조회 화면 구현  
* 성능 부담 : Parse 및 최적화 비용 발생  
* 보안 관리 필요 : SQL Injection 대응 필수  

