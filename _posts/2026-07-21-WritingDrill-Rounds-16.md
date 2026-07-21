---
layout: post
title: "WritingDrill_Rounds_16"
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

### [신기술, BigUp모의고사/합숙] AI Native Development Platform

**[정의]**  

생성형 AI(GenerativeAI)를 사용하여, 소프트웨어를 이전보다 빠르고 쉽게 개발할 수 있도록 바이브코딩 및 AI 에이전트를 지원하는 소프트웨어 개발 플랫폼  

**[핵심/키워드]**  

* 가트너 2026, DevOps → AI 기반 자동화  
 * AI를 기본 아키텍처로 설계, SDLC 전반에 AI 내재  

&lt;구성&gt;  
 1) AI 모델 계층 : LLM, 도메인 특화 모델(코드 생성, 분석, 리팩토링)  
 2) 개발 자동화 : AI 코드 어시스턴트, AI 테스트 자동화(코드 생성, 품질, 결함 예측)  
 3) 운영 기술 : AIOps, CI/CD 엔진(로그 분석, 장애 예측, 성능 최적화, 자동 배포)  
 4) 데이터 영역 : 데이터레이크·데이터하우스, 지식그래프·벡터DB(의미 기반 검색)  
 5) 확장 기술 : 에이전트 프레임워크(개발·운영 작업 수행, 워크플로 자동화)  

&lt;도구&gt;  
 1) 클라우드 기반 (Google Vertext AI, Amazone SageMaker, MS Azure AI)  
 2) 개발자 도구 (GitHub Copilot)  
 3) AI Agent 개발 플랫폼 (Mind Studio)  
 4) AI 앱 생성 플랫폼 (Natively)  

### [신기술, BigUp모의고사/합숙] 컨피덴셜 컴퓨팅(Confidential Computing)

**[정의]**  

신뢰 실행 환경(TEE)기반으로 사용 중(in-use)인 상태의 데이터까지 보호하는 컴퓨팅 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
 - TEE 기반 보안, 개인정보보호, 데이터 사용중 암호화  

<구성(기술)>
 1) 신뢰실행환경 (TEE)  
  - Intel(SGX, TDX), AMD (SEV-SNP), ARM (Trustzone), AWS (Nitro))  
 2) 실행증명 (무결성확인)  
  - 측정부팅, 어테스테이션  
 3) 주변장치 (하드웨어칩) :  GPU, NIC, FPGA  
 4) 시스템 SW (프로그래밍 모델) : Enclave  
 5) 응용암호화 : 완전동형, SMPC(안전한 다자간 연산)  

&lt;TEE&gt;  
 - 하드웨어 기반 격리(측정부팅), 원격 증명(PCR)  

### [신기술, BigUp모의고사/합숙] 도메인 특화 언어모델 (DSLM, Domain-Specific Language Model)

**[정의]**  

특정 산업의 데이터로 학습하여 고정밀·고신뢰 예측이 가능한 특화 LLM  

**[핵심/키워드]**  

&lt;특징&gt;  
 - DSLM 학습데이터셋, 골든 데이터셋  

&lt;기술&gt;  
 1) 데이터 : 도메인 전용 데이터셋, 데이터 정제 및 라벨링  
 2) 모델학습 : 파인 튜닝(Fine-tuning), From Scratch 학습  
 3) 지식확장 : RAG (Retrieval-Augmented Generation), 벡터 데이터베이스  
 4) 지식구조화 : 지식 그래프(KG)  
 5) 입력최적화 : 프롬프트 엔지니어링, 인컨텍스트 러닝(ICL)  
 6) 추론 제어 : 룰 기반 제어  
 7) 안전성 : 도메인 안전 가드레일  
 8) 평가 :  도메인 특화 평가 지표  
 9) 운영 : 지속적 학습(MLOps/LLMOps)  
 10) 보안/거버넌스 : 접근통제, 감사가능성  

### [신기술, BigUp모의고사/합숙] 선제적 사이버 보안(Proactive Cyber Security)

**[정의]**  

위협 발생 이전 단계에서 위험을 식별·예측·차단하는 사전 예방중심 보안접근 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 사전예방 중심, 자동위협 차단·기만기술 적용, 위협 사냥 (Threat Hunting)  

&lt;기술요소&gt;  
 1) 공격표면관리(ASM) : 외부공격 표면식별, 노출 자산 지속 스캔  
 2) 위협인텔리전스 AI : IOC, TTP, 위협예측 모델  
 3) 행동 모니터링 : UEBA, 행위기반 이상탐지  
 4) 이상탐지 : 비지도학습 기반 탐지, 시계열 이상탐지  
 5) AISecOps : SOAR, SIEM  

### [신기술, BigUp모의고사/합숙] PMBOK 8th edition

**[정의]**  

PMBok 7th의 원칙 중심 철학과 이전 버전의 실무적 프로세스 구조를 결합, 프로젝트 관리를 효과적으로 수행하기 위한 지침서  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 7th의 가치 중심 + 이전의 프로세스 중심 실무 적용, 가치 전달(Value Delivery)  
 - 6 원칙, 7 성과 도메인, 40개 프로세스, 5가지 초점영역  

&lt;6원칙&gt;  
 1) 전체적 관점, 2) 가치중심, 3) 품질내재화, 4) 책임감 리더십,  
 5) 지속가능성 통합, 6) 권한있는 문화  

&lt;7성과도메인&gt;  
 1) 거버넌스 (governance), 2) 범위 (scope), 3) 일정 (schedule), 4) 재무 (finance),  
 5) 이해관계자 (stakeholder), 6) 자원 (resources), 7) 위험 (risk)  

&lt;5 초점영역&gt;  
 1) 착수, 2) 계획, 3) 실행, 4) 감시/통제, 5) 종료  

### [신기술, BigUp모의고사/합숙] CAST(Causal Analysis based on System Theory)

**[정의]**  

STAMP 이론 기반, 시스템 전체 관점에서, 사고가 발생한 후 근본적 원인을 분석하여 사고의 재발을 방지하기 위한 기법  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 사고 원인 분석 (발생한 사고의 근본 원인 분석, 재발 방지)  
 - 다양한 원인 포함(조직 구조·행동·안전 문화 등), 안전제약조건, 확증편향회피  

&lt;동작 절차&gt;  
 1) 기본정보 수집, 2) 제어구조 모델링, 3) 컴포넌트 분석,  
 4) 제어 구조 결합 식별, 5) 개선 프로그램 생성  

### [신기술, BigUp모의고사/합숙] 에이전트 커머스(Agent Commerce)

**[정의]**  

사용자의 의도를 파악한 AI Agent가 상품 탐색, 금액 비교, 최종 결제와 배송 확인까지 자율적으로 수행하는 새로운 상거래 모델  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 의도기반(Intent-based) 자동실행  

&lt;작동원리&gt;  
 1) 자연어 명령, 2) 의도해석 및 탐색, 3) Catalog API 연동, 4) 보안토큰, 5) 결제/승인  

&lt;아키텍처 기술요소&gt;  
 1) AI 엔진 : LLM 의도해석, 자동결제 (플래닝, 툴)  
 2) 데이터인프라 : 상품 메타데이터, Catalog / Inventory API  
 3) 협업구조 : A2A 통신, MCP 프로토콜  
 4) 결제/신뢰(보안) : SPT, AP2  
 5) 신원/권한 (거버넌스) : KYA, 디지털 자격증명  

### [신기술, BigUp모의고사/합숙] 오픈워싱(Open Washing)

**[정의]**  

오픈(Open)이라는 용어를 사용하지만 실질적인 개방요건(코드·표준·권한)을 충족하지 않는 행위  

**[핵심/키워드]**  

&lt;특징&gt;  
 - Open+Washing, 개방성 위장  

&lt;전형적패턴&gt;  
 - API만 공개, 내부 로직 비공개, 소스 공개하되 비자유 라이선스  

&lt;대응방안&gt;  
 - OSI(Open Source Initiative)기준, 라이선스 검토(MIT, GPL 등)  
 - SBOM기반 라이선스 관리,  OSPO조직 운영  

### [신기술, BigUp모의고사/합숙] 데이터센터 네트워킹

**[정의]**  

데이터 센터 내 서버·스토리지·가속기(GPU/NPU)간 고속·저지연 통신을 제공하는 인프라 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 초대규모, 초저지연, Leaf-Spine, East-West 트래픽  
 * 고대역폭, Scale-Out  

&lt;기술요소&gt;  
 1) GPU Interconnect : NVLink, NVL72, UALink  
 2) 서버간 패브릭 : InfiniBand, Ultra Ethernet  
 3) 메모리 접근기술 : RDMA, RoCE, InfiniBand RDMA  
 4) 광통신 연결 : Silicon Photonics (실리콘포토닉스)  

### [신기술, BigUp모의고사/합숙] Wi-Fi 8/IEEE 802.11bn

**[정의]**  

Wi-Fi 7에 비해 초고신뢰성 (UHR), 안정적인 연결, 더 강력한 커버리지, 혼잡한 네트워크에서도 원활한 로밍을 위한 차세대 Wi-Fi 표준  

**[핵심/키워드]**  

&lt;특징&gt;  
 - IEEE 802.11bn, UHR, Seamless, 25% 이상 성능 개선, 신뢰성, 안전성  

&lt;사양&gt;  
 - 주파수 (2.4GHz, 5GHz, 6GHz), 대역폭 (320MHz),  
 - 최대속도 (23Gbps), 변조 (4096QAM)  
 - 안테나 (16x16 MIMO)  

&lt;주요기능&gt;  
 - Cross Layer (DSO, NPCA)  
 - MAC Layer (MAPC, ELA)  
 - PHY layer (DRU, ELR, UEQM),  
 - 다중협업 (CO-BF, CO-SR, CO-RTWT, CO-CR)  

### [신기술, BigUp모의고사/합숙] LPU(Language Processing Unit)

**[정의]**  

대규모 언어모델(LLM)의 추론 성능을 극대화하기 위해 설계된 아키텍처  

**[핵심/키워드]**  

&lt;특징&gt;  
 - TSP (Tensor Streaming Processor), SRAM 중심 설계,  
 - 결정론적아키텍처 (Deterministic Architecture)  

&lt;주요구성&gt;  
 1) 처리장치 - TSP, MXM, SXM, MEM, VXM, SIMD  
 2) 저장장치 - On-Chip SRAM  
 3) 통신장치 - C2C Interconnect, Deterministic Network  
 4) 제어장치 - Software Defined Scheduler, Synchronous Data Flow  

&lt;기능&gt;  
 - LLM 추론 가속, 지연시간 최소  

&lt;적용&gt;  
 - Groq LPU (On-Chip SRAM, 정적, 결정론적, SW 주도 준동기화)  
 - HyperAccel LPU (LPDDR, 다이렉트 스트리밍, 거대단일코더, HW 자율 ESL)  

### [신기술, BigUp모의고사/합숙] 공동 패키징 광학(CPO, Co-Packaged Optics)

**[정의]**  

AI 연산칩(GPU, ASIC 등)과 광학소자를 하나의 패키지 기판 위에 직접 통합하는 차세대 반도체 패키징 기술  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 광 신호 전송, 동일 패키지 사용, 저전력, 초고대역폭, 저지연, 고집적화  

&lt;연결 대상&gt;  
 - 칩↔칩, 칩↔스위치, 스위치↔스위치  

<구성 / 기술요소>
 1) 스위치 ASIC : SerDes, Digital PHY  
 2) 광학엔진 : SiPh (실리콘 포토닉스), InP (인듐인)  
 3) 광변조기 :  MZM (마하-젠더), MRM (마이크로링)  
 4) 광수신기 : TIA (트랜스 임피던스), GePD (게르마늄 포토다이오드)  
 5) 파장 다중화부 : DWDM, CWDM  
 6) 레이저광원 : DFB Laser (분산 피드백), CW Laser (연속파)  
 7) 패키징 기판  
  - Interposer (인터포저), Co-Packaging (공동 패키징), EMIB (고밀도연결)  
 8) 광결합부 - Fiber (광섬유), Grating (회결격자)  

### [신기술, BigUp모의고사/합숙] UCIe3.0(Universal Chiplet Interconnect Express 3.0)

**[정의]**  

칩렛간 통신속도를 비약적으로 높이고(최대 2배), 복잡한 멀티-칩 시스템을 위한 관리 및 테스트 기능을 강화한 차세대 개방형 칩렛 상호연결 표준  

**[핵심/키워드]**  

* 초당 64GT, 부가채널 거리 10mm  

 1) 프로토콜 계층 : 연속 전송 프로토콜, 스트리밍 프로토콜 확장  
 2) 어댑터 계층 : 오류 검출 및 재전송 매커니즘  
 3) 물리 계층 : 고속 신호 처리, 런타임 재보정, 사이드밴드 거리 확장  

&lt;기술요소&gt;  
 1) 성능 및 전력효율 : 데이터 속도 2배, 런타임 재보정, L2 유휴 최적화  
 2) 시스템관리 및 신뢰성 : 우선순위 측대역 패킷, 빠른 스로틀 및 긴급종료  
 3) 설계유연성 : 확장된 측대역 도달거리, 연속 전송 프로토콜, 고신뢰 인코딩  

 1) 고속스로틀링  
  - open drain 양방향 핀, Thermal zone, 내부 fail-safe  
  - 작동방식 : 미리 협상 수준 속도 스로틀링  
 2) 비상 셧다운  
  - off package driver, 와이어 연결, 최대온도 도달  
  - 작동방식 : 셧다운 신호 외부전원 전달  

### [신기술, BigUp모의고사/합숙] NPU(Neural Processing Unit)

**[정의]**  

딥러닝 연산 (특히 신경망 추론)을 효율적으로 수행하기 위해 설계된 AI 전용 프로세서  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 행렬,벡터 연산 최적화 : CNN, Transformer, 핵심 연산 고속 처리  
 - 고효율, 저전력 : 전력 제약 환경에서도 AI 실행  
 - 전용 MAC (Multiply-Accumulate) 배열 : 대규모 병렬 Multiply-Add 연산  

&lt;기술요소&gt;  
 1) 제어부 : Instruction Scheduler, Control Logic  
 2) 메모리계층 : Unified Cache System, DMA Controller  
 3) 텐서 : Tensor Processing Core, MAC Array  
 4) 벡터 연산 : Vector Processing Unit  
 5) 전용함수 : Activation Fuction Accelerator, Pooling Operation Accelerator  
 6) 데이터 전처리 : Quantization Unit, Reorder Unit  

### [신기술, BigUp모의고사/합숙] SASE(Secure Access Service Edge)

**[정의]**  

네트워크와 보안 기능을 클라우드에서 통합 제공하는 아키텍처 모델  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 클라우드 통합(네트워크+보안), 위치무관 보호·엣지 적용,  
 - 제로 트러스트 기반, 멀티환경 유연성  

&lt;구성&gt;  
 1) 네트워크 보안 (Network Security as a Service) (=SSE)  
  - CASB, SWG, FWaaS, ZTNA, VPN  
 2) 네트워크 (Network as a Service)  
  - SD-WAN, CDN, Carrier, Bandwidth Aggregation, Networking Vendors  

### [신기술, BigUp모의고사/합숙] CI(Connecting Information)

**[정의]**  

개인 식별정보를 직접 사용하지 않고, 이를 일방향 해시(Hash) 처리하여 생성한 개인 고유 식별값  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 불가역성 (원본 주민번호 복원 불가), 고유성(동일인 항상 동일한 CI 값)  
 - 연계성(서로 다른 기관 동일인 식별), 표준길이(88byte), 개인정보에 해당  

&lt;생성&gt;  
 1) 입력값, 2) 해시함수 적용, 3) CI 출력  

&lt;발급&gt;  
 1) 회원 가입 요청, 2) 본인확인 요청, 3) 본인확인 완료,  
 4) 본인확인 결과, 5) 회원관리 완료  

&lt;보안위험성&gt;  
 - 식별수단 (공통식별자, 악용시나리오), 피해확장 (2차피해, 마스터 키)  

&lt;해결&gt;  
 - C12 전환, 유효기간 설정, 제로 트러스트, 분리 보관  

&lt;CI와 DI 비교&gt;  
 - CI : 연계정보(기관 간 식별)  
 - DI : 중복가입확인정보(사이트 내 중복 확인)  

### [신기술, BigUp모의고사/합숙] Purdue 모델

**[정의]**  

PERA기반,  enterprise 영역과 manufacturing(제조) 영역으로 나누고, IDMZ를 사용한 IT와 OT의 이중 분리 구조의 보안 참조모델  

**[핵심/키워드]**  

* PERA, ISA-99  

&lt;Level&gt;  
 * 6단계 구성  
  - Level 4~5 - Enterprise 영역(IT영역)  
  - 두영역 사이에 IDMZ  
  - Level 0~3 - Manufacturing 영역(OT영역)  

&lt;OT 보안 6원칙 연계&gt;  
 - 레벨5 : 엔터프라이즈 NW (IT영역), 원칙 2 (Biz 이해), 원칙 4 (NW 분리)  
 - 레벨4 : 이메일, 인터넷, 물류 NW, 원칙 2 (Biz 이해), 원칙 5 (안전한 공급망)  
 - IDMZ : 방화벽, 리버스 프록시,, 원칙 4 (NW 분리), 원칙 5 (안전한 공급망)  
 - 레벨3 : 사이트 운영 (OT영역), 원칙 2 (Biz 이해), 원칙 5 (안전한 공급망)  
 - 레벨2 : 구역 감독 통제 , 원칙 1 (안전 최우선), 원칙 6 (인적 보안)  
 - 레벨1 : 기본제어-배치,분산,드라이브, 원칙 3 (데이터 보호), 원칙 6 (인적 보안)  
 - 레벨0 : 드라이브, 엑츄에이터, 로봇, 원칙 4 (NW분리), 원칙 5 (안전한 공급망)  

### [신기술, BigUp모의고사/합숙] HNDL(Harvest Now, Decrypt Later) 공격

**[정의]**  

공격자가 암호화된 데이터를 수집 및 저장한 뒤,나중에 양자 기술이 충분히 발전하면 이를 해독하려는 공격 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 현재 데이터 수집 (Harvest Now), 나중에 해독 공격 (Decrypt Later)  
 - 모스카 (Mosca)의 부등식 (X+Y>Z) 원리  

&lt;동작과정&gt;  
 1) 수집 (HarvestNow) : 현재 상태(Present)  
 2) 대기 및 보관(Storage) : 과도기(Interim)  
 3) 해독(Decrypt) : 미래(Future)  

&lt;대응방안&gt;  
 - 양자내성암호화 (PQC)  
 - 하이브리드 암호화 아키텍처  
 - 암호 민첩성  
 - 대칭키 암호화 키 길이 강화  
 - PKI 고도화 : Crypto-Agility 확보. PQC 기반 HSM/KMS 가속화  

&lt;유사&gt;  
 * SNDL (Store Now, Decrypt Later - 선 저장 후 해독)  
 * 사후 해독 공격 (Retrospective Decryption)  

### [신기술, BigUp모의고사/합숙] AI 해킹

**[정의]**  

성능저하, 정보유출, 오작동 유도를 목적으로 인공지능 모델·데이터·서비스를 목표로 한 공격  

**[핵심/키워드]**  

* OWASP Top 10 for LLM / Agent, ATLAS (위협 프레임워크)  

&lt;공격목표&gt;  
 - 모델 무력화, 정보 유출  

&lt;주요 공격유형&gt;  
 - 데이터 포이즈닝, 모델 도용/추출, 모델 인버전, 프롬프트 인젝션, 탈옥  

&lt;주요취약점&gt;  
 - 데이터 파이프라인 신뢰 부족, 검증/모니터링 미흡, 권한 관리 취약  

<공격도구,기법>
 - API 정보 노출, 자동화 쿼리/스크립트 공격, 합성 데이터, 적대적 패턴 최적화  

&lt;대응방안&gt;  
 - 데이터 무결성 확보, 모델 안전성 강화, 운영/접근통제  
 - AI레드팀, AI정렬, 거버넌스/검증체계  

### [신기술, BigUp모의고사/합숙] 랜섬웨어 다중갈취(Multi-Extortion)

**[정의]**  

랜섬웨어 공격자가 단순 암호화를 넘어, 데이터 탈취··제3자 압박 등 복수의 협박 수단을 결합하여 피해 조직의 지불 압력을 극대화하는 복합형 협박 전술  

**[핵심/키워드]**  

&lt;유형&gt;  
 - Double Extortion : 데이터 암호화 + 유출 협박, 2중 갈취  
 - Triple  Extortion : Double + DDoS, 3중 갈취 방식  
 - Quadruple Extortion : Triple + 공급망•파트너•규제기관까지 확장, 4단계 이상  

<대응방안 : 예방적 관점>
 - 접근 통제 및 계정 보안 : 다중 요소 인증(MFA), 최소 권한 원칙  
 - 취약점 및 패치 관리 : 정기적인 패치, 취약점 스캐닝  
 - 데이터 백업 : 3-2-1 백업 전략, 어어갭, 불변 스토리지  
 - 데이터 유출 방지 : DLP 솔루션 적용  
 - 탐지 및 격리 : EDR/XDR 구축  

<대응방안 : 사후 대응 관점〉
 - 복구 능력 확보 : 사이버 복원력 강화  
 - 운영적 위협 대응 : DDOS 방어 체계, 공급망 체계 강화  
 - 몸값 지불 정책 : 지불 거부 원칙, 전문가 협의  
 - 법률 및 평판 리스크 관리 : 법률 자문, 대외 커뮤니케이션  

### [신기술, BigUp모의고사/합숙] 데이터 랭글링(Data Wrangling)

**[정의]**  

분석·머신러닝·시각화 등의 목적에 맞게 원시 데이터(Raw Data)를 정제하고 구조화하는 일련의 전처리 과정  

**[핵심/키워드]**  

* AI Ready Data로 만드는 필수 전처리  

&lt;절차&gt;  
 1) 데이터 탐색, 2) 데이터 구조화, 3) 데이터 정제,  
 4) 데이터 확장/통합, 5) 검증/품질 평가, 6) 출력/배포  

&lt;도구&gt;  
 - 쿼리/DB : MySQL, PostgreSQL  
 - 데이터 처리(파이썬) : Pandas, NumPy  
 - 전처리/머신러닝(ML) : Scikit-learn  
 - 데이터 모델링/변환 : dbt (Data Build Tool)  
 - ETL/ELT : Apache NiFi, Talend, Trifacta  
 - 데이터 프로파일링 : Pandas Profiling (ydata-profiling)  

&lt;데이터 랭글링 vs ETL vs ELT&gt;  
 * 랭글링 : 탐색적 정제·분석 중심,  
 * ETL : 정형화 이동 프로세스,  
 * ELT : 클라우드 기반 이동 후 변환  

&lt;데이터 랭글링 vs 데이터 먼징 vs 데이터 전처리&gt;  
 * 랭글링 : 정제, 구조화 전체과정  
 * 먼징 : 초기 데이터 정제  
 * 전처리 : 데이터 준비과정  

### [신기술, BigUp모의고사/합숙] 러닝라이트(Learn right)

**[정의]**  

창작자가 저작물이 AI 학습에 사용될 경우 이를 허용 또는 거부하거나 보상을 요구하도록 지원하는 지적재산권  

**[핵심/키워드]**  

* AI 학습 데이터 권리 공백을 보완 대안, AI 저작권  

&lt;필요성&gt;  
 - AI 학습 데이터 활용 급증, 기존 저작권 제도의 한계  
 - 창작자의 선택권/보상 요구 증가  

&lt;주요내용&gt;  
 - 공정이용, 라이선스 필요, 옵트인 등록 시스템, 기여자 보상  

&lt;기존 6대 러닝라이트 저작권&gt;  
 1) 복제권 (Reproduction Right)  
 2) 2차적 저작물 작성권 (Derivative Works Right)  
 3) 배포권 (Distribution Right)  
 4) 공연권 (Public Performance Right)  
 5) 전시권 (Public Display Right)  
 6) 디지털 음성 전송권 (Digital Audio Transmission Right)  
 7) AI 학습 허용/거부권 → 현재 논의 중인 제7의 배타적 권리  

&lt;유사용어&gt;  
 * TDM (Text and Data Mining) exception / right (EU)  

### [신기술, BigUp모의고사/합숙] 오픈소스 AI

**[정의]**  

데이터 정보·코드 정보·매개변수 정보를 모두 공개하고 사용·연구·수정·공유의 4가지 자유를 보장하는 AI  

**[핵심/키워드]**  

<오픈소스AI 조건 (4대 자유)>
 - 사용 (Use) : 상업적/비상업적 제한 없음  
 - 연구 (Study) : 투명성 보장  
 - 수정 (Modify) : 커스터마이징 자유  
 - 공유 (Share) : 재배포 자유  

&lt;필수 공개 항목&gt;  
 - 데이터 정보 : 학습 데이터 관련 정보 (승인조건)  
 - 코드 : 전체 소스코드 (라이선스)  
 - 매개 변수 : 모델 가중치 및 설정 (승인조건)  

&lt;유형&gt;  
 - AI 시스템 : AI 시스템 전체 적용  
 - AI 모델 : 모델 구조, 모델 매개 변수(가중치 포함) 등 독립적  
 - AI Weight : 매개변수 집합 적용  

&lt;오픈소스 AI vs 오픈웨이트&gt;  
 * 오픈소스 AI : 가중치, 전체 코드 공개  
 * 오픈웨이트 : 훈련코드, 데이터셋 미공개  

### [신기술, BigUp모의고사/합숙] 전방 배치 엔지니어(FDE, Forward Deployed Engineer)

**[정의]**  

고객 현장(Customer Site)에 직접 배치되어 비즈니스 요구사항을 분석, AI·LLM·데이터·클라우드 기술을 활용, 맞춤형 솔루션을 설계·구현·운영하는 고객 밀착형 AI 엔지니어  

**[핵심/키워드]**  

&lt;주요역량&gt;  
 - AI / Cloud : 클라우드 환경이해, 아키텍처 설계  
 - Domain : 업무 이해, 비즈니스 요구해석  
 - AI Apps Dev : 애플리케이션 개발, API 연계  
 - Full Stack Data Science : 전과정 수행, E2E 데이터 파이프라인  
 - Communication Skill : 원활한 소통, 브릿지 역할  

&lt;주요 역할&gt;  
 - 현장 문제 발굴 및 업무 프로세스 분석, 데이터 연결 및 AI 솔루션 구현  
 - 현장 적용·검증 및 조직 확산  

&lt;주요 산출물&gt;  
 - AI 적용 과제 및 요구사항 정의서, 개선된 업무 프로세스 ,  
 - 현장 적용 AI 서비스·에이전트, 운영·확산 계획 및 성과지표  

&lt;FDE 핵심 수행영역&gt;  
 - 고객 이해 : Business Analysis, 도메인 지식, 업무 프로세스 분석, 요구사항·KPI 정의  
 - AI 솔루션 구현 : LLM, AI Agent, Prompt·Context Engineering, 모델 최적화  
 - 데이터 활용 : RAG, Vector DB, 데이터 파이프라인, Knowledge Graph  
 - 시스템 통합 : API, MSA, MCP, 이벤트 기반 연계, 기존 시스템 통합  
 - 운영 최적화 : MLOps, LLMOps, AIOps, 모니터링, 성능·비용 최적화  
 - 보안·거버넌스 : IAM, Guardrail, 개인정보 보호, 모델·데이터 품질 관리  
 - 현장 적용·확산 : PoC·MVP 개발, 사용자 검증, 변화관리, 교육 및 확산  

### [신기술, BigUp모의고사/합숙] 로봇 파운데이션 모델(Robotic Foundation Model)

**[정의]**  

로봇의 지각, 계획, 조작 등 다양한 도메인 전반에서 활용이 가능한 범용 로봇제어 아키텍처  

**[핵심/키워드]**  

* 사전 학습 모델, 범용  

&lt;주요기술&gt;  
 - 데이터/학습 : 멀티모달 데이터, Pre training, Fine-tuning, RLHF  
 - 인지/이해 : 멀티모달 인식, NLU, 시맨택 매핑, VLA (Vision Language Action)  
 - 계획/추론 : 행동계획, 논리/물리 추론, 시스템2 (추론)  
 - 제어/실행 : 강화학습, 모션 제어, 디지털 트윈, 시뮬레이션, 시스템1 (제어)  
 - 시스템 아키텍처 : 트랜스포머, Diffusion, 모델 압축, On Device, 엣지 AI  
 - 응용/확장 : Guardian / Embodied Agent, 텔레오퍼레이션  

&lt;활용&gt;  
 - RX (로봇 트랜스포메이션), 피지컬 AI, Embodied AI, HRI  

### [신기술, BigUp모의고사/합숙] 옴니모달(Omni-Modal) AI

**[정의]**  

텍스트·이미지·음성·영상·행동 등 모든 모달 데이터를 하나의 통합 모델에서 학습·이해·생성하는 AI 구조  

**[핵심/키워드]**  

* 단일모델-모든 모달통합 (공유잠재공간)  

&lt;특징&gt;  
 - 단일 Transformer, 공통 토큰화(Tokenization), Sequence-to-Sequence  
 - Interleaved 데이터, 일체형 구조  

&lt;핵심 기술&gt;  
 - 공통 토큰화 : 동일한 토큰 단위  
 - 모달 정렬(Alignment) : 동일한 임베딩 공간 정렬  
 - 크로스 모달 학습 :  
     Matching(의미적 일치), Translating(모달 변환), Referencing(참조)  
 - 생성 : Multimodal Generation, Diffusion Models, VLMO  
 - 맥락/추론 : 종합적 모달 정보 이해  
 - 통합 : 인코드-디코더 통합  
 - Cross Attention : 정보 교차  

&lt;사례&gt;  
 - Gemini Omni, GPT 5.5, NVIDIA Cosmos 3  

&lt;멀티모달 vs 옴니모달&gt;  
 - 멀티모달 : 모달별 분리 인코더 → 융합 모듈 → 출력  
 - 옴니모달 : 공통 토큰화 → 공유 잠재공간 → 단일 Transformer → 멀티모달  

### [신기술, BigUp모의고사/합숙] Re-ranking 알고리즘

**[정의]**  

초기 검색 결과를 다시 평가하여 더 정확한 순서로 재정렬하는 알고리즘  

**[핵심/키워드]**  

* 1차 결과를 관련성(Relevance)과 일관성(Consistency) 기준 Re-Ranking  
* 2단계 후 처리 (Post-processing)  

&lt;단계&gt;  
  1단계 (Recall 중심),  2단계 (Precision 중심)  

&lt;주요 알고리즘&gt;  
 1) Cross-Encoder : 쿼리와 문서를 하나의 입력 처리  
  - Cross-Encoder, MonoBERT  
 2) Embedding : 쿼리와 문서를 독립적 임베딩 벡터 변환  
  - Bi-Encoder  
 3) Late Interaction : 쿼리 토큰과 문서 토큰 간 MaxSim 연산  
  - ColBERT  
 4) Learning to Rank (Pointwise) : 각 문서를 독립적으로 점수화  
  - MART, GBRank  
 5) Learning to Rank (Pairwise) : 두 문서의 상대적 순서 비교  
  - RankNet, LambdaRank  
 6) Learning to Rank(Listwise) : 문서 리스트 전체의 순서 고려  
  - ListNet, ListMLE, LambdaMART  

&lt;동향&gt;  
 - 추론(Reasoning) 주입, LLM-as-Reranker, Hybrid  

### [신기술, BigUp모의고사/합숙] SEO(Search Engine Optimization)

**[정의]**  

검색엔진에서 웹사이트나 콘텐츠가 자연 검색 결과의 상위에 노출되도록 만드는 모든 기술과 전략  

**[핵심/키워드]**  

&lt;구성요소&gt;  
 - 온 페이지(On-page) : 키워드, 제목 태그, 메타 설명, 콘텐츠 품질  
 - 오프 페이지(Off-page) : 백링크, 소셜 신호, 브랜드 언급  
 - 기술(Technical) : 사이트 속도, 모바일 최적화, 보안(HTTPS), 구조화 데이터  
 - 사용자 경험(UX) : 직관적 내비게이션, 빠른 로딩,명확한 정보 제공  

&lt;기술요소&gt;  
 - 사이트 최적화 : XML사이트맵, CDN, Cache  
 - 보안요소 : HTTPS, SSL/TLS  
 - TAG활용 : Title, Meta description, H1~H6 헤딩, ALT태그  
 - 크롤링 관리 : Robots.txt, Canonical태그, Noindex 태그  
 - 로그분석 : Google Search Console, ELK  
 - 국제SEO : hreflang 태그, Lazy Loading  
 - 멀티미디어 : Alt속성, WebP포맷, 자막  

&lt;SEO vs AEO vs GEO&gt;  
 * SEO : 검색순위 상승, 키워드 중심, 웹페이지  
 * AEO : 페이지 내 답변, 구조 데이터 중심, 질문-답변  
 * GEO : 신최출처, 요약, 문맥, 청크, 임베딩  

&lt;동향&gt;  
 - E-E-A-T 강화, Zero-Click 증가  

### [신기술, BigUp모의고사/합숙] 에이전트 군집(Swarm) 코딩

**[정의]**  

여러 개의 자율적인 AI에이전트가 협력하여 복잡한 소프트웨어 개발 프로젝트를 수행하는 개발 방법론  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 자율성, 컨텍스트 이해, 분산제어, 협업 및 조정  

&lt;구성요소&gt;  
 - 에이전트 (Agent) : 자율성, 목표 지향성, 환경 인지  
 - Hand-off : 에이전트 간 제어권이나 작업을 위임  
 - 통신 메커니즘 : 메시지 큐,API호출  
 - Coordination : 전체 군집의 행동, 작업할당  
 - Environment : 코드베이스,버전 관리 시스템(Git),개발 도구(IDE)  

&lt;기술요소&gt;  
 - 멀티에이전트 프레임워크 : AutoGen, LangChain /LlamaIndex, OpenGPTs/CrewAI  
 - 지식베이스 : VectorDB, RAG 시스템  
 - LLM : ChatGPT, GPT-5, Claude  
 - 버전관리 : Git, GitHub, GitLab  

### [신기술, BigUp모의고사/합숙] ISO/IEC 42119

**[정의]**  

ISO/IEC/IEEE 29119를 기반으로 인공지능(AI) 시스템의 테스팅 및 품질 검증 절차를 규정하는 국제 표준 시리즈  

**[핵심/키워드]**  

* ISO/IEC/IEEE 29119 기반  

&lt;주요 파트&gt;  
 1) ISO/IEC TS 42119-2 (AI 시스템 테스트 개요) : 프레임워크와 위험 기반 접근 방식  
 2) ISO/IEC AWI TS 42119-7 (AI 레드팀 테스팅)  
  - AI 시스템의 취약점을 공격 및 검증 레드팀 평가 수행  

 * 특징 : 공격자 관점, AI고유 취약점, 사전 예방적, 반복 및 개선  
 * 테스트절차 : 1) 범위/목표, 2) 위협 모델링 시나리오, 3) 공격, 4) 결과 추적, 5) 개선  
 * 테스트기법  
  - 입력조작 : 프롬프트주입, 탈옥, 모델회피  
  - 데이터공격 : 학습데이터오염, 모델추출, 민감정보 유출  
  - 시스템 통합 : 과도한 권한/위임, 편향/공정성  
 * 구성원 : 리더/PM, AI 레드팀 전문가, 보안 테스트 전문가, AI 엔지니어,  
               AI 법률 전문가, 도메인 전문가  
 * 연계 : CVD / VDP 연계 가능  

### [신기술, BigUp모의고사/합숙] 소버린 클라우드(Sovereign Cloud)

**[정의]**  

현지 법률과 규정을 준수하여 데이터 접근이 이루어지도록 설계하고 구축된 클라우드 컴퓨팅 아키텍처  

**[핵심/키워드]**  

&lt;소버린 클라우드 기능&gt;  
 1) 데이터 소유권 강화 : 데이터 관리 및 제어 강화  
 2) 강화된 보안 : 기존 클라우드 대비 보안 향상  
 3) 높은 서비스 가용성 : 안정적 서비스 제공  
 4) 국가/조직의 특정요구 충족 : 컴플라이언스 준수  

&lt;소버린 클라우드 구축 절차&gt;  
 1\. 사전준비 : 주권 정책 정의, 주권확보 전략수립,  주권 확보 준비  
 2\. 구현 : 주권 아키텍처 수립, 클라우드 데이터 통제  
 3\. 운영 : 클라우드 주권 관리, 주권 생태계 최적화  

&lt;국내사례&gt;  
 - 클라우드 보안 인증제(CSAP)와 민관협력형 모델(PPP)존재  

&lt;활용&gt;  
 - 소버린 AI 연계, 자립형 AI 생태계  

### [신기술, BigUp모의고사/합숙] 양자컴퓨터 오류

**[정의]**  

극도로 미세한 큐비트(Qubit)가 외부 환경(열·전자기파)과의 상호작용으로 인해 디코히어런스(결어긋남)를 일으키며 데이터가 손실되는 현상  

**[핵심/키워드]**  

&lt;원인&gt;  
 - 결어긋남, 게이트 오류, 상태전환 오류, 측정오류, 누화 오류  

&lt;양자 오류의 처리 기법&gt;  
 1) 오류 억제 (Error Suppression) : 오류 발생 자체를 줄이는 방법  
  - 동적 디커플링, 최적 제어 펄스, 양자 피드백 제어  
  - 누화(=간섭) 억제(Crosstalk Suppression)  
 2) 오류 완화 (Error Mitigation) : 발생한 오류의 영향을 사후 보정하는 방법  
  - 제로 노이즈 외삽 (ZNE, Zero Noise Extrapolation)  
  - 확률적 오류 제거 (PEC, Probabilistic Error Cancellation)  
  - 측정 오류 보정, 누화 모델링(Crosstalk Modeling)  
 3) 오류 정정 (Error Correction, QEC) : 오류를 실시간 검출·정정하는 방법  
  - Shor Code, Steane Code, Surface Code, Color Code  
 4) 결함 허용 양자 컴퓨팅 (FTQC)으로의 전환  

<양자 오류 정정(QEC) 절차>
 ① 논리 큐비트 준비 ② 오류 발생 ③ 신드롬 측정 ④ 디코딩 ⑤ 오류 정정  

&lt;ancilla&gt;  
 - 데이터 큐비트를 직접 측정하지 않고, 오류 정보만 읽기 위해 사용하는 임시 큐비트  

### [신기술, BigUp모의고사/합숙] 데이터 메시(Data Mesh)

**[정의]**  

중앙 집중형 데이터 레이크의 한계를 극복하기 위해, 도메인 중심의 분산형 데이터 관리 방식(탈중앙화)을 적용하는 데이터 아키텍처 패러다임  

**[핵심/키워드]**  

* 탈중앙, 분산형, 도메인 중심  

&lt;데이터 메시 4원칙&gt;  
 1) 도메인 소유권(Domain Ownership),  
 2) 데이터 제품화(Data as a Product),  
 3) 셀프서비스 플랫폼(Self-Serve Data Platform),  
 4) 연합형 계산 거버넌스(Federated Computational Governance)  

&lt;구성요소&gt;  
 - 아키텍처 : Domain, 셀프세비스 플랫폼, 분산 거버넌스  
 - 도메인 : 운영 데이터, 분석 데이터, 데디터 제품  

&lt;주요솔루션&gt;  
 - 카탈로그 : Data Catalog, Glue, Dataplex, Unity Catalog  
 - 쿼리 페더레이션 : BigQuery, Lakehouse Federation  
 - 데이터 스트리밍 : Kafka, Dataflow, Kinesis  
 - IaC (Infrastructure as Code) : Terraform, Cloud Formation, Ansible  
 - 생성형 AI (Generative AI)  

### [신기술, BigUp모의고사/합숙] AI 리터러시(Literacy)

**[정의]**  

개인이 AI 기술을 비판적으로 평가할 수 있게 해주는 일련의 역량으로서, AI와 효과적으로 의사소통하고 협업하며 온라인, 가정 및 직장에서 AI를 도구로 사용하는 역량  

**[핵심/키워드]**  

&lt;필요 역량&gt;  
 - AI 기본 개념 이해 (기계학습, 딥러닝 등)  
 - AI 윤리와 책임 (편향, 투명성, 프라이버시 등)  
 - AI 활용 역량 (도구 사용, 문제 해결 능력)  
 - 비판적 사고력 (AI 결과 해석 및 한계 이해)  

&lt;강화방안&gt;  
 - 정책연구, 커리큘럼 개발, 디지털 취약층 교육, 교육자 대상 교육  
 - 국제협력, 민관산학연 협력  

### [신기술, BigUp모의고사/합숙] AI TRiSM(Trust, Risk, Security Management)

**[정의]**  

AI 부작용을 최소화하고, 방안으로 인공지능의 신뢰성, 위험성, 그리고 보안관리를 강조하는 프레임워크  

**[핵심/키워드]**  

* 가트너 2023 / 2024  
* 인공지능 신뢰, 인공지능 위험성, 인공지능 보안  

&lt;주요목적&gt;  
 - 거버넌스, 신뢰성, 공정성, 안전성, 데이터 보호  

<5가지 기본 요소 (5 Core Elements)>
 - 설명 가능성 (Explainability) : 기능의 투명성과 이해 가능성 확보  
 - 모델옵스 (ModelOps) : AI 모델의 자동화된 운영 및 배포  
 - 데이터 이상 탐지 (Data Anomaly Detection) : 비정상 데이터 식별 및 감지  
 - 적대적 공격 대응력 (Adversarial Attack Resistance) : 적대적 학습 공격 방어  
 - 데이터 보호 (Data Protection) : 개인정보 및 민감 데이터 보호  

<시스템 요소 (System Components)>
 - AI 시스템 (AI System) : AI 모델을 포함한 실행 환경  
 - 에이전트 (Agent) : 워크플로우 기능을 수행하는 단위 실행체  

&lt;주요계층&gt;  
 - AI 거버넌스(AI Governance) : AI 자산 관리, 신뢰 구축  
 - AI 런타임 검사 및 실행 (AI Runtime Inspection and Enforcement) :  
      거버넌스 정책과의 트랜잭션 정렬  
 - 정보 거버넌스(Information Governance) : 데이터의 전체 라이프사이클  
 - 인프라 및 스택(Infrastructure and Stack) : 하드웨어 및 소프트웨어 환경, 배포 환경  

### [신기술, BigUp모의고사/합숙] 결측치(Missing Value) 처리 기법

**[정의]**  

학습 모델의 편향, 과적합 방지를 위해 측정 누락된 Data를 처리하는 매커니즘  

**[핵심/키워드]**  

&lt;결측치 유형&gt;  
 - MCAR (완전 무작위), MAR (무작위), MNAR (비무작위 결측)  

&lt;처리 기법&gt;  
 1\. 제거법 : 단일값 삭제, 목록삭제, 행 제거, 열 제거  
 2\. 단일 대체법 : 평균, 중앙값, 최빈값, 이전/이후 단순확률 대치  
  - 단순확률 (핫덱, 콜드덱, 혼합)  
 3\. 다중 대체법 : 단일 대체 여러번, MICE  
 4\. 모델 기반 대체 : KNN (근접), 회귀 (Regression)  
 5\. 머신러닝 알고리즘 내부 자체 : XGBoost, LightGBM, CatBoost  

### [신기술, BigUp모의고사/합숙] 패스키(PassKey)

**[정의]**  

비밀번호 기반 인증 방식의 보안 취약점 해소를 위해 WebAuthn기술 표준의 공개키 방식을 적용한 FIDO 기반 무비밀번호 인증기술  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 비밀번호 불필요, 서비스별 고유성, 비정상 인증 방지, 피싱방지  

&lt; 기술요소 &gt;  
 - FIDO2 : Passkey의 기반 기술, WebAuthN, CTAP  
 - WebAuthN : 브라우저와 서버 간 인증, W3C 표준 API  
 - CTAP : 인증 장치와 클라이언트 간 통신 프로토콜  
 - FDO : IoT 장치의 클라우드 관리 플랫폼 온보딩  
 - 공개키/개인키 : 디바이스와 서버에 저장, 상호인증 수행  
 - OAuth2 : 자원 소유자 자격증명 승인 방식  
 - 암호학적 난수 : 예측 불가능한 챌린지 생성  
 - 생체인식 : 사용자 본인 여부를 확인  
 - 보안 장치 내 인증자 : 개인키 저장/연산하는 물리적 보안 모듈  

&lt;등록&gt;  
 1) 공객키 - 개인키 생성, 2) 공개키 서버 저장  

&lt;인증&gt;  
 1) 서버의 챌린지 요청, 2) 개인키 서명 / 전송, 3) 공개키 검증  

&lt;유형&gt;  
 1) 동기화형 패스키 (Synced Passkey) : 클라우드 키체인, 여러 기기 공유  
 2) 기기 종속형 패스키 (Device-bound) : 특정 물리적 하드웨어 내부 저장  

&lt;사례&gt;  
 - Apple/Google Passkey  

### [신기술, BigUp모의고사/합숙] 서비스 가치 시스템(SVS, Service Value System)

**[정의]**  

서비스 통한 가치 창출 달성하는데 필요한 활동과 규제및 절차로 조직의 가치흐름맵을 통한 성과 개선 활동을 지원하는 시스템  

**[핵심/키워드]**  

* ITIL v4.0, 사일로 방지  

&lt;구성요소&gt;  
1) 지도원칙  
2) 거버넌스  
3) 서비스가치 사슬  
4) 지속적 개선  
5) 실행  

&lt;서비스가치사슬&gt;  
 - 계획 (Plan), 개선 (Improve), 참여 (Engage), 설계 및 전환 (Design and Transition)  
 - 획득 및 구축 (Obtain and Build), 제공 및 지원 (Deliver and Support)  

### [신기술, BigUp모의고사/합숙] 시프트-레프트 테스팅(Shift-Left Testing)

**[정의]**  

개발의 초기부터 테스팅에 대한 우선순위를 높이고 SDLC의 각 단계에서 발생되는 문제점을 식별하고 성능수준을 평가하는 기법  

**[핵심/키워드]**  

* 개발 초기부터 테스트  

&lt;특징&gt;  
 - 정적코드분석 도구, 단위테스트 프레임워크, 테스트 자동화 도구, 지속적 통합도구  

&lt;활용&gt;  
 - SAST, JUnit, SonarQube  

### [신기술, BigUp모의고사/합숙] CMMI 3.0

**[정의]**  

소프트웨어 개발 및 서비스관리 등 다양한 산업에서 프로세스 성숙도를 평가하고 개선하기 위한 글로벌 표준 모델  

**[핵심/키워드]**  

* 보안(Security), 안전(Safety), 데이터(Data), 가상(Virtual) 환경 도메인 추가  

&lt;8개 도메인&gt;  
 - 기본(Core), Development(DEV), Services (SVC), Suppliers (SPM), Security (SEC)  
 -Safety (SAF), People (PPL), Data (DAT), Virtual (VRT)  

&lt;카테고리별 역량영역&gt;  
 - DOING : 서비스 제공 및 관리, 제품 개발 및 엔지니어링, 품질 보장  
 - MANAGING : 비즈니스 연속성 관리, 인력 관리 및 운영, 업무 계획 및 관리  
 - ENABLING : 데이터 관리, 보안 및 안전 관리, 이행 지원  
 - IMPROVING : 성과 향상 및 유지, 습관 유지 및 지속성 관리  

<역량 수준(Capability Levels)과 성숙도 수준(Maturity Levels)>
 1) 역량 수준:  
  - 레벨 0 (Incomplete), 레벨 1 (Initial), 레벨 2 (Managed), 레벨 3 (Defined)  
 2) 성숙도 수준  
  - 레벨 0(Incomplete), 레벨 1(Initial), 레벨 2 (Managed), 레벨 3 (Defined),  
  - 레벨 4(Quantitatively Managed), 레벨 5(Optimizing)  

&lt;특징&gt;  
 - 유연성 강화, 애자일 및 디지털 트랜스포메이션 지원  
 - 리스크 및 성과 중심, 모듈화된 구조, 데이터 중심 접근  

### [신기술, BigUp모의고사/합숙] 데이터 가치평가

**[정의]**  

데이터산업법 제14조 근거, 데이터의 경제적 가치를 시장, 수익, 원가접근법 중 가능한 기법을 사용해서 평가하는 제도  

**[핵심/키워드]**  

* 데이터산업법 제14조  

&lt;평가요인&gt;  
 - 데이터 특성 분석, 법적 특성 분석, 사업성 분석, 시장성 분석  

&lt;평가기법&gt;  
 - 수익접근법 : 추가이익기준, 증분수익, 데이터기여도  
 - 원가접근법 : 생산비용, 역사적, 재생산, 대체원가  
 - 시장접근법 : 유사 데이터, 시장거래 사례, 로열티 공제  

&lt;핵심변수&gt;  
 - 경제적 수명, 할인율, 데이터기여도  

&lt;평가절차&gt;  
 1) 평가의뢰, 2) 서류제출, 3) 계획수립, 4) 평가준비, 5) 현장실사  
 6) 평가요인, 7) 가치산정, 8) 결과통보, 9) 사후관리  

### [신기술, BigUp모의고사/합숙] 범용 인공지능(AGI, Artificial General Intelligence)

**[정의]**  

기계가 자신의 지능을 이해하고, 학습하고, 적용하여 인간 지능과 구별할 수 없는 방식으로 문제를 해결할 수 있는 수준의 인공 지능  

**[핵심/키워드]**  

* 인간과 유사 수준, 범용성  

&lt;Level&gt;  
 - Level 0 (미진입), Level 1(신진), Level 2(유능), Level 3(전문가),  
   Level 4(거장), Level 5(슈퍼휴먼)  

&lt;AGI 주요 기술&gt;  
 - 딥러닝, 머신러닝, 자연어 처리, 컴퓨터 비전, 로보틱스, 추론과 결정,  
    심리 인식, 사회적 지능  

&lt;ANI vs AGI vs ASI&gt;  
 * ANI : 특정 기능, 업무  
 * AGI : 인간지능 유사  
 * ASI : 인간지능 초월  

### [신기술, BigUp모의고사/합숙] 탐색적 데이터 분석(EDA, Exploratory Data Analysis)

**[정의]**  

데이터 분석과정에서 수집된 데이터 입력 시 데이터의 구조, 특성, 패턴 등 넓은 시각에서 직관적으로 이해 및 관찰한 후 연구자의 가설 수립을 위한 분석 기법  

**[핵심/키워드]**  

<탐색적 데이터 분석(EDA)의 4가지 주제>
 1) 저항성  
 2) 잔차의 해석  
 3) 데이터의 재표현  
 4) 데이터의 현시성  

&lt;분석영역&gt;  
 - 데이터탐색 (특성, 분포, 시각화), 전처리 (결측값, 정규화, 표준화)  

&lt;유형&gt;  
 - 일변량 비그래픽, 일변량 그래픽, 다변량 비그래픽, 다변량 그래픽  

### [신기술, BigUp모의고사/합숙] 확증적 데이터 분석(CDA)

**[정의]**  

도출된 가설의 유의성 및 모형 검증을 위해 데이터를 수집, 평가하여 분석하는 기법  

**[핵심/키워드]**  

&lt;절차&gt;  
 - 가설설정 → 데이터 수집 → 통계적 분석 → 가설검증  

&lt;기법&gt;  
 - T-test, ANOVA, 상관분석, 회귀분석  

### [신기술, BigUp모의고사/합숙] 권력/관심 모델

**[정의]**  

이해관계자들이 프로젝트 팀에 대한 관심도와 영향력을 통해 어떤 영향을 받게 될지 분석하는 모델  

**[핵심/키워드]**  

&lt;유형&gt;  
- 잠재적 관계자 (관심 낮음, 권력 높음)  
- 후원적 관계자 (관심 높음, 권력 높음)  
- 옹호적 관계자 (관심 높음, 권력 낮음)  
- 무관심 관계자 (관심 낮음, 권력 낮음)  

### [신기술, BigUp모의고사/합숙] 양자전자서명

**[정의]**  

양자 상태를 활용하여, 위조·부인 방지·서명자 검증 가능한 전자서명 기술  

**[핵심/키워드]**  

* 양자 + 전자서명  

&lt;특징&gt;  
 – 양자 키분배 기술(QKD), 다자간 양자 비밀 분산  
 – 별도의 안전한 통신 채널 보장, 일방향 해시함수 사용  

&lt;주요기술&gt;  
 - 양자 키 분배(QKD) : 송신자-수신자 간 공유 비밀키 생성  
 - 양자 원타임 패드(Quantum One-Time Pad) :  생성된 양자 키 사용, 한 번만 암호화  
 - 양자 메시지 인증코드(QMAC)  
 - Quantum Digital Signature Protocols : 수신자 간 이중 확인  
 - Quantum Fingerprinting / Hashing :  서명 데이터 축소 및 검증  

&lt;방식&gt;  
 - 양자 디지털 서명 (QDS, Quantum Digital Signature) : 양자역학 기반  
 - 양자내성 전자서명 (PQC Signature, Post-Quantum Cryptography) :  
       양자내성 수학적 기반 전자서명  

### [신기술, BigUp모의고사/합숙] 트래픽 폴리싱(Traffic policing)

**[정의]**  

정의된 트래픽 기준을 초과하는 트래픽을 버림으로서 대역폭을 제어하고 과부하를 방지하는 기법  

**[핵심/키워드]**  

* 초과 시 Drop / Remark, 속도제한  

&lt;구성요소&gt;  
 - Token Bucket  
 - Meter / Rate Limit : CIR, PIR, CBS  
 - Marker : Remark, Drop  

&lt;특징&gt;  
 - Burst : 제한 / 불허  
 - Buffer : 미사용  

&lt;활용&gt;  
 - 통신사, 백본 라우터, Inbound  

### [신기술, BigUp모의고사/합숙] 인공지능 생성물 워터마크(Watermark)

**[정의]**  

인공지능에 의해 생성된 콘텐츠(이미지, 텍스트, 오디오 등)를 식별하기 위해 삽입되는 고유한 표시나 패턴  

**[핵심/키워드]**  

* AI 기본법, AI 투명성 확보 가이드라인  

&lt;분류&gt;  
 1) 인지가능(가시적) 워터마크  
  - 이미지 (로고, 가시적 워터마크 삽입)  
  - 동영상 (상시 노출, 시작/종료 자막)  
  - 오디오 (음성 안내)  
 2) 인지불가능(비가시적) 워터마크 (+사전안내)  
  - C2PA, SynthID (사람 인식 안내 필수)  
  - 동영상/오디오 (시작이나 재생 초기 문구 / 멘트)  
  - 이미지 병행 문구 명시적  

&lt;목적&gt;  
 - AI 생성물 오남용 방지  

&lt;기법&gt;  
 - 이미지 : 공간기반 (LSB), 변환기반 (DCT, Edge Masking), 학습기반 (Stable)  
 - 오디오 (변환) : 시간 (Audio Seal), 주파수 (WavMark, Spread Spectrum)  
 - 텍스트 (학습) : 학습기반, 추론 (로짓 생성, 토큰 샘플링)  

### [신기술, BigUp모의고사/합숙] 사전 적정성 검토 제도

**[정의]**  

AI 등 신서비스·신기술이 ‘개인정보보호법’에 위반되지는 않는지 사전에 검토 및 컨설팅해주는 제도  

**[핵심/키워드]**  

* 개인정보 보호법 제7조의 8, 제7조의 9  

&lt;목적&gt;  
 - 개인정보보호법 위반 사전 방지, 혁신 저해 예방 , 안전한 데이터 활용  

&lt;절차&gt;  
 - 신청서 제출 → 신청요건 검토 → 현황분석 → 적용방안 마련 →  
    적용방안 검토 → 결과통보 → 환류  

&lt;검토사항&gt;  
 - PBD, 개인정보, 영상정보, 생체인식정보, PET, 정부주체 권리행사  

### [신기술, BigUp모의고사/합숙] 벡터 데이터베이스(Vector Database)

**[정의]**  

방대한 양의 고차원 데이터를 벡터 형태로 최적화하여 보관하고 쿼리하기 위해 특화된 데이터베이스  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 벡터화된 데이터의 저장 및 검색, 근사 최근접 이웃 검색(ANN) 지원, LLM, RAG  

&lt;동작방식&gt;  
 1) Indexing : 임베딩, 벡터 저장, 인덱싱  
 2) Querying : 쿠리 임베딩, 유사도 검색  
 3) Post-processing : 후처리 및 결과 반환  

&lt;구성 요소&gt;  
 - 임베딩 벡터 (Embedding Vector) : 고정된 차원의 벡터  
 - 벡터 인덱스(Vector Index) : 벡터 간 유사도 계산 구조(ANN 기반)  
 - 유사도 함수 (Similarity Function) : Cosine Similarity, Euclidean Distance  

<근사 최근접 이웃 검색(ANN)>
 - HNSW : 그래프 기반 탐색  
 - IVF : 벡터를 클러스터링 후 후보만 탐색  
 - PQ : 벡터를 압축·양자화  
 - ScaNN : IVF + PQ + 재정렬  
 - ANNOY : 트리 기반 디스크 검색  

### [신기술, BigUp모의고사/합숙] 분산분석(ANOVA, Analysis of Variance)

**[정의]**  

여러 집단(3개 이상)의 평균 차이를 검정하기 위해, 집단 간 분산(차이)과 집단 내 분산(오차)을 비교하는 통계 기법  

**[핵심/키워드]**  

* 3개이상, 평균차이, 집단 간 분석 / 집단 내 분산  

&lt;가정사항&gt;  
 - 독립변수(3개 집단 이상), 종속변수(연속형 변수)  
 - 독립성, 정규성, 등분산성, 사후검정(귀무가설 기각시, 집단간 평균 차이 확인 )  
 - 모수검정, F검정  

&lt;유형&gt;  
 - 일원분산분석(One-Way ANOVA),  
 - 이원분산분석(Two-Way ANOVA),  
 - 반복측정 분산분석(Repeated Measures ANOVA)  

&lt;검정방법&gt;  
 - F-test / F통계량 = 집단간분산/집단내분산  
 - F통계량이 1근처이면 집단간 차이없음, 1보다 크면 집단간 차이 있음  

### [신기술, BigUp모의고사/합숙] OAuth 2.0

**[정의]**  

OAuth 1.0의 단점을 개선하여 다양한 인증 플로우와 간소화된 프로세스를 제공하는 프로토콜  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 표준화 : RFC 6749 및 RFC 6750에 의해 표준화  
 - 보안 방식 : 액세스 토큰 기반, HTTPS로 보안.  
 - 플로우 : 다양한 인증 플로우 제공  
 - 장점 : 다양한 클라이언트 유형(모바일, 데스크톱 등) 지원, 사용성과 확장성 개선.  
 - 단점 : 액세스 토큰 유출 시 보안 위협 가능, 토큰 관리가 중요  

&lt;구성요소&gt;  
 - Resource Owner (자원 소유자): 웹 서비스의 사용자, 자원 소유  
 - Client (클라이언트) : 자원 요청 서버  
 - Authorization Server (권한 서버) : Authorization Code, Access Token  
 - Resource Server (자원 서버) : 데이터 저장 서버  
 - Access Token (액세스 토큰) : 자원 접근 권한 부여 토큰  
 - Refresh Token (리프레시 토큰) : 새로운 Access Token 요청  

&lt;인증플로우&gt;  
 - Authorization Code, PKCE  
 - 현재 거의 미사용(Implicit, Client Credentials)  

&lt;동향&gt;  
 - OAuth 2.1 표준으로의 통합 가속화  
 - 패스키(Passkey) 및 OIDC와의 결합  

### [신기술, BigUp모의고사/합숙] PQC(Post-QuantumCryptography)

**[정의]**  

양자 컴퓨터로도 해독 불가한 수학적 난제를 활용, 양자 환경에서도 기밀성·무결성·인증을 보장하는 차세대 암호 체계  

**[핵심/키워드]**  

* 가트너 2025, Shor 알고리즘, Grover 알고리즘, HNDL 공격 대응  

&lt;유형&gt;  
 - 다변수기반 : Rainbow, Gui  
 - 코드기반 : QC-MCPC, Wild McEliece (암호화)  
 - 격자기반 : Kyber (암호화), Dilithium (서명), SS- NTRU, FrodoKEM  
 - 아이소제니기반 : SIDH  
 - 해시기반 : SPHINCS+ (서명, 무 상태형), XMSS(상태 유지형)  

&lt;동향&gt;  
 - NIST : FIPS 203 (ML-KEM), FIPS 204 (ML-DSA), FIPS 205 (SLH-DSA)  
 - 한국형 알고리즘(K-PQC)  

 - 기술적 관점 : 암호 민첩성 기반 설계, 키·서명 크기 증가 대응  
 - 운영.관리적관점 : 암호 자산 목록 구축 (CBOM), 전문 인력  
 - 정책.규제 관점 : SNDL선제 대응, 규제 준수 및 일정  

&lt;단계적 전환 방안&gt;  
 1) AS-IS진단 - 암호 자산 목록화  
 2) 위험 평가 - 양자 보안 위험 평가  
 3) TO-BE설계 -PQC알고리즘 및 키관리 구조 설계  
 4) 시범 적용 -성능·호환성 검증  
 5) 피드백 반영 - 암호 민첩성 보완  
 6) 단계 전환 - 기존 암호+PQC병행 적용  
 7) 운영 안정화- PQC거버넌스 정착  

### [신기술, BigUp모의고사/합숙] 역 페이지 테이블(Inverted Page Table)

**[정의]**  

효율적인 메모리 관리를 위해 크기가 고정된 페이지 테이블에 프레임 번호를 맵핑하는 메모리 관리 기법  

**[핵심/키워드]**  

&lt;특징&gt;  
 – 크기 고정 페이지 테이블 하나  
 – 테이블 항목은 메모리 한 프레임씩  
 – 테이블 항목 탐색을 위해 pid 정보  
 – 분산 메모리 할당의 페이징 방식  

<역페이지 테이블(Inverted Page Table)의 주소 변환 과정>
 - CPU → 논리주소(가상주소) → 역페이지테이블 탐색 → 물리주소 변환 →  
     물리메모리 접근  
 - 물리 프레임 번호 → (프로세스ID, 가상 페이지번호)를 저장  

&lt;동작&gt;  
 - 입력 : 논리 주소(pid, p, d)  
 - 탐색 : 역페이지 테이블에서 (pid, p) 일치 항목 검색  
 - 출력 : 물리 주소(i, d) 생성  

### [신기술, BigUp모의고사/합숙] Dark Factory

**[정의]**  

AI, IoT 등 최첨단 기술을 활용해 사람의 개입 없이 생산, 검사, 포장 등 모든 공정이 자동으로 이뤄지는 무인화된 “암흑 공장”  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 완전 자동화, 24시간 무중단 생산, 비용 절감, 안전성 향상  

&lt;기술요소&gt;  
 - 데이터 수집 : IIoT 센서, RFID·바코드, OPC-UA·MQTT, Edge Gateway  
 - 지능형 분석 : AI·ML 모델, MLOps, AutoML로 지능형 분석 및 예측 자동화  
 - 실행·제어 : 로보틱스·피지컬AI, AGV·AMR, PLC·MES 연동으로 현장 자동 제어  
 - 통합 운영 : CPS, 디지털트윈, SDF 기반 통합 시뮬레이션 및 운영 최적화  
 - 보안·관리 : OT 보안·SOC, AMO로 산업제어시스템 보안·운영 관리 강화  
 - 인간·조직 : HMI, HITL, RLHF, 러터리스·변화관리로 인간 중심 협업 강화  

&lt;적용 사례&gt;  
 - 독일 : 지멘스 – 암베르크 공장  
 - 미국 : 테슬라 – 상하이 기가팩토리  
 - 한국 : 현대자동차 – 미국 메타플랜트  

### [신기술, BigUp모의고사/합숙] Slowloris

**[정의]**  

불완전한 HTTP GET헤더를 지속 전송하여 서버 연결 풀을 점진적으로 고갈시키는 DoS공격  

**[핵심/키워드]**  

&lt;특징&gt;  
 - GET 헤더, IDS우회, 소량 데이터 연결 유지, 낮은 대역폭, 애플리케이션 계층  

&lt;절차&gt;  
 1) TCP 세션 생성 : HTTP 연결, 유지  
 2) 미완성 헤더 전송 : 요청 종료 (CRLF) 생략 전송  
 3) Request 대기 : 세션 유지  

&lt;대응&gt;  
 - 연결시간 제한, 속도 제한, 최소 전송 속도, 보안 장비 / 솔루션  

&lt;유사&gt;  
 - Slow Http Header DoS  

### [신기술, BigUp모의고사/합숙] 디지털 트윈 네트워크(DTN, Digital Twin Network)

**[정의]**  

현실의 네트워크를 실시간으로 디지털로 재현, 이를 바탕으로 네트워크를 예측, 운영, 최적화하는 네트워크  

**[핵심/키워드]**  

&lt;핵심요소&gt;  
 - Data, Model, Interface, Mapping  

&lt;구성요소&gt;  
 - 물리 네트워크, 디지털 트위윈, 데이터 수집, 분석 엔진, 시뮬레이션 엔진,  
   제어 시스템  

&lt;아키텍처 계층&gt;  
 - 물리 네트워크 계층, 디지털 트윈 계층, 네트워크 응용 계층  

&lt;기술요소&gt;  
 - IoT, 센서 데이터, 클라우드, 엣지 컴퓨팅, AI, 머신러닝, SDN, 가상화 기술  

### [신기술, BigUp모의고사/합숙] AI-DLC(AI-Driven SDLC)

**[정의]**  

기획, 구현, 테스트 등 소프트웨어 개발 전과정(SDLC)에 인공지능을 통합하여, AI가 계획수립과 코딩을 주도하고 사람이 검증하는 방식의 차세대 개발방법론  

**[핵심/키워드]**  

&lt;특징&gt;  
 - AI역량과의 정렬, 고속반복 (Bolt), 단계 최소화, 흐름 극대화, 설계기법 내재화  

&lt;동작&gt;  
 1) 착수 : 몹 정교화(Mob Elaboration), 비즈니스 의도 요구사항, 스토리 변환  
 2) 구축 : 몹 구축(Mob Construction), 아키텍처, 모델, 테스트  
 3) 운영 : 코드형 인프라와 배포를 관리  

&lt;구성요소&gt;  
 - 인텐트 : 높은 수준 목표  
 - 유닛 : 독립적 측정 가능 작업 묶음  
 - 볼트 : 가장 작은 반복단위  
 - 에픽 : 작업 단위  

### [신기술, BigUp모의고사/합숙] 공공SLA표준안

**[정의]**  

서로 합의한 서비스 품질 수준을 정량적 지표로 명문화하고 이를 체계적으로 관리·평가하기 위해 정부가 제정한 표준 가이드라인  

**[핵심/키워드]**  

* 표준운영절차 (SOP : Standard Operating Procedure)  
* ITIL v4 및 ISO/IEC 20000 기반  

&lt;대상&gt;  
 - 예전 등급 (필수 1등급, 2등급, 권고 3등급, 4등급)  
 - 의무 (A1~A3등급, 13개 운영절차 의무화), 권고 (A4등급)  

&lt;표준절차&gt;  
 1) 서비스 정의 : 환경식별, 중요도 등급(A1~A4) 부여  
 2) 지표 및 목표 설정 : 최저 기준 바탕으로 SLA, RFP 명시  
 3) 모니터링 및 측정 : 표준운영절차(SOP)에 따라 측정  
 4) 평가 및 환류  

<표준운영절차/영역>
 - 공통 (요청, 변경, 장애, 문제), 인프라 (구성, 이벤트, 서비스수준, 백업)  
 - 응용 (배포, 테스트, 연계, 형상, 운영상태)  

&lt;핵심지표&gt;  
 - 장애관리 : VM가동률, 하이퍼바이저 가동률, 장비 가동률  
 - 운영관리 : 반복장애건수, 백업준수율  
 - 정보보안관리 : 보안취약점 양호율, 침해사고 발생 건수  
 - 성능관리 : 서비스 응답시간  
 - 선택지원관리 : 요청 적기 처리율, 서비스 만족도  

### [신기술, BigUp모의고사/합숙] LLM모델 테스트

**[정의]**  

대규모 언어모델의 출력 품질, 안전성, 신뢰성, 공정성을 다차원적으로 검증하는 테스트  

**[핵심/키워드]**  

&lt;4대품질특성&gt;  
 - 정확성 (Accuracy), 안전성 (Safety), 공정성 (Fairness), 효율성 (Efficiency)  

&lt;절차&gt;  
 1단계 : 테스트계획 수립 (Test Planning), 품질지표 정의 기법  
 2단계 : 데이터셋 구성 (Dataset Construction), 벤치마크 및 적대적 데이터 기법, MMLU, HellaSwag  
 3단계 : 기능 테스트 (Functional Testing), 정확성, 일관성, 추론기법, 정확성 테스트  
 4단계 : 안전성, 윤리 테스트 (Safety, Ethics Testing), 편향(Bias) 테스트  
 5단계 : 성능, 효율 테스트 (Performance Testing), 부하테스트, 스트레스 테스트, 토큰비용 분석  
 6단계 : RAG, 통합 테스트, 검색 정확도(Retrieval Precision, Recall)  
 7단계 : 배포 후 지속평가 (Continuous Evaluation), A/B Test  

&lt;LLM 표준 벤치마크 테스트&gt;  
 - 언어 이해력(MMLU), 상식 추론 능력(HellaSwag)  
 - GSM-8K(수학 추론 능력) 평가  
 - 환각 방지 능력(TruthfulQA) 평가  

&lt;LLM 적대적 입력 테스트&gt;  
 - 프롬프트 인젝션, 탈옥(Jailbreak), 경계값 입력으로 취약점 점검  

### [신기술, BigUp모의고사/합숙] 매터(Matter)

**[정의]**  

스마트 홈 장치 및 IoT 플랫폼 간의 상호운용성, 신뢰성, 안정성 등을 확보하기 위해 누구나 사용 가능한 개방형 스마트홈 연동 표준(프로토콜)  

**[핵심/키워드]**  

&lt;목적&gt;  
 - 단순성, 상호연동성, 신뢰성, 안전성  

&lt;특징&gt;  
 - 멀티어드민 : 동일 디바이스 ID로 여러 스마트홈 플랫폼에 동시 등록  
 - 로컬 제어 : 디바이스 상태 확인 및 제어를 로컬에서 진행가능  

&lt;데이터모델&gt;  
 - Node : 물리적 기기  
 - EndPoint : 독립적 기능/서비스, 논리적 단위  
 - Cluster : 엔트포인트의 특정한 기능  

&lt;통신&gt;  
 - Wi-Fi, Thread, IPv6, Bluetooth, Ethernet, IEEE 802.15.4  

&lt;클러스터 구조&gt;  
 - Attribute : 속성, 현재상태  
 - Command : 제어, 지시  
 - Event : 상태변화, 알림  

&lt;보안&gt;  
 - DAC(Device Attestation Certificate) : 기기별 보안 신분증  

&lt;매터 최근 버전&gt;  
 - 1.4 : 홈 라우터 연동, 태양광·EV 충전기 등 에너지 기기 통합 예정  
 - 1.5 : 에너지 관리기능, 보안카메라 지원  
 - 1.6 : NFC 오프라인 페어링, 공동관리 (Joint Fabric)  

### [신기술, BigUp모의고사/합숙] AVL Tree

**[정의]**  

삽입/삭제 시 균형 인수를 체크하여 좌우 서브 트리 높이 차가 1 이하를 유지하게 회전을 수행하는 이진트리  

**[핵심/키워드]**  

* 균형인수 (-1, 0, 1), 좌우 1이하 높이, 균형이진트리  

<회전, Rotation>
 - LL, LR, RL, RR  

&lt;복잡도&gt;  
 - 시간 복잡도 O(logN)  

&lt;활용&gt;  
 - T-Tree  

### [신기술, BigUp모의고사/합숙] 동기부여이론

**[정의]**  

효율적인 조직 관리를 위해 조직원들이 어떤 욕구나 보상에 의해 어떠한 행동을 보이고, 그 성과는 어떠한가를 분석하는 이론  

**[핵심/키워드]**  

1) 내용 이론 (What – 무엇이 사람을 동기부여하는가)  
  - 매슬로우 욕구 5단계 이론: 생리 → 안전 → 사회적 → 존경 → 자아실현  
  - 매슬로우 7단계 : 5단계 + 심미 + 인지  
  - 허즈버그의 2요인이론: 위생요인(불만족 해소)과 동기요인(만족 유발)  
  - 맥클리랜드 성취 동기 이론: 성취, 권력, 친화 욕구  
  - 앨더퍼의 ERG 이론: 생존, 관계, 성장 욕구  
 2) 과정 이론 (How – 어떻게 동기가 유발되는가)  
  - 아담스 공정성 이론: 타인과의 보상 비교를 통해 동기 형성  
  - 브룸 기대 이론: 노력 → 성과 → 보상의 인과관계 인식  
  - 로크 목표 설정 이론: 구체적이고 도전적인 목표가 동기 자극  
 3) 강화 이론 (Why – 왜 특정 행동이 강화되는가)  
  - 스키너의 강화 이론: 행동에 대한 결과(강화·처벌)가 행동 반복에 영향  
  - 긍정적 강화, 부정적 강화, 처벌, 소거의 네 가지 행동조정 방식  

### [신기술, BigUp모의고사/합숙] IaC(Infrastructure as Code)

**[정의]**  

인프라 자원(서버, 네트워크, 스토리지 등)을 수동 설정이 아닌 코드로 정의·관리하는 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 자동화, 버전관리 가능, 일관성 확보, 재현 가능성 우수, 골든패스 구축  

&lt;주요 도구&gt;  
 - Terraform, Ansible, CloudFormation, Pulumi, OpenTofu  

&lt;유형&gt;  
 - 선언형 (Declarative) : 원하는 상태를 정의 (ex: Terraform, CloudFormation)  
 - 절차형 (Imperative) : 수행할 명령 순서를 정의 (ex: Ansible, Chef)  

&lt;기술요소&gt;  
 - 코드 기반 구성관리,  선언형/절차형 스크립트,  
 - 버전관리 시스템(Git 등), 템플릿 엔진(예: Jinja2),  
 - 상태관리(State File), CI/CD 통합, 프로비저닝 도구(Terraform, Ansible 등),  
 - 테스트 및 검증 도구(Testinfra, Kitchen), 클라우드 API 연동  

### [신기술, BigUp모의고사/합숙] 유지보수 감리

**[정의]**  

정보시스템 개발, 구축 완료 후 기능변경, 추가, 보완, 폐기, 사용방법의 개선, 문서 보완 등의 정보시스템 개선에 필요한 제반 활동  

**[핵심/키워드]**  

* 전자정부법 시행령 71조, 의무아님  

<감리대상/점검>
 - 개발소프트웨어 (13개) : 모니터링, 성능관리, 요구사항관리  
 - 상용소프트웨어 (12개) : 유지보수계획, 패치, 예방점검  
 - 인프라 (13개) : 업그레이드, 긴급/장애처리  

### [신기술, BigUp모의고사/합숙] 분석모델의 적합도 검정

**[정의]**  

실험에서 얻은 결과가 이론 분포와 일치하는 정도  

**[핵심/키워드]**  

* Goodness of Fit  
* 적합도, 확률분포 타당성, 모델의 예측성, 가설설정, 검정통계량  

&lt;단계&gt;  
 - 가설 설정, 검정 통계량 선택, 임계값 설정, 유의성 검정, 결과해석  

&lt;종류&gt;  
 - 정규분포 비가정 : 카이제곱검정(Chi-Square Test)  
 - 정규분포 가정 : 샤피로-윌크 검정(Shapiro Wilk Test), 콜모고로프-스미르노프 검정(Kolmogorov-Smirnov Test), Q-Q Plot(Quantiles-Quantiles Plot)  

### [신기술, BigUp모의고사/합숙] SNN(Spiking Neural Network)

**[정의]**  

뇌의 뉴런이 시간에 따라 이산적인 전기적 스파이크(펄스)를 발생시키는 생물학적 신경 활동을 모사한 신경망 모델  

**[핵심/키워드]**  

* 뉴런, 스파이크, STDP, 저전력  

&lt;구성&gt;  
 - Input Spike, Synapse, Weight, Neuron, Output Spike  

 1) 뉴런 활성화(Spiking Mechanism)  
  - 입력 (Input) → 입력 인코딩 층 (Input Encoding Layer)  
 2) 스파이크 전파 및 누적 (Spike Propagation & Integration)  
  - 입력 인코딩 층 → 스파이킹 뉴런 층 (Spiking Neuron Layer)  
 3) 학습 규칙 적용(Weight Update)  
  - 스파이킹 뉴런 층(STDP 연결,  측면 억제 연결)  
 4) 출력 스파이크 패턴 분석 (Output Spike Pattern Interpretation)  
  - 출력 (Output) 뉴런  

&lt;활용&gt;  
 - NPU, 뉴로모픽  

### [신기술, BigUp모의고사/합숙] 디지털 시장법(Digital Markets Act)

**[정의]**  

빅테크 기업 게이트키퍼라 칭함이 투명하게 경영하고 사용자 데이터를 독점하지 못하도록 규제하는 법안  

**[핵심/키워드]**  

* 독점방지, EU  

<게이트키퍼(총 6 개)>
 - 알파벳(구글), 아마존, 애플, 메타, 마이크로소프트, 바이트댄스(틱톡)  

&lt;주요내용&gt;  
 - 자사우대금지, 외부결제 허용, 데이터 결합제한  

&lt;유사법률&gt;  
 - 디지털시장법 : 독점방지  
 - 디지털서비스법 : 책임 및 투명성 강화  
 - 사이버복원력법 : 제품 보안성 강화  

### [신기술, BigUp모의고사/합숙] 클라우드 책임공유모델(SRM, Shared Responsibility Model)

**[정의]**  

클라우드 서비스 제공자(Cloud Service Provider)와 사용자가 클라우드 영역별 보안에 대한 책임을 분담하는 모델  

**[핵심/키워드]**  

* 책임분담  
* 클라우드서비스사용자, 클라우드서비스제공자, 기업외부  

### [신기술, BigUp모의고사/합숙] DPU(Data Processing Unit)

**[정의]**  

CPU의 인프라 기능 분산을 위해 네트워크 인터페이스 하드웨어에서 암호화, 웹서비스, 스토리지 제어 등 데이터 처리 가능한 컴퓨팅 프로세서  

**[핵심/키워드]**  

* 데이터 중심, 가상화, smart NIC  

&lt;핵심기능&gt;  
 - 패킷처리 가속 (L2~L7), 암호화 복호화 오프로드, 스토리지 프로토콜 처리  
 - 가상화, 컨테이너 네트워크 처리, 보안 기능  

&lt;구성요소&gt;  
 1) 제어부 (Control Plane)  
  - CPU Complex (ARM 코어), System Level Cache  
 2) 데이터 가속부 (Data Plane)  
  - Data Acceleration Block, PCIe Switch (Internal)  
 3) 네트워크 서브시스템 (NIC Subsystem)  
  - Data Path Accelerator, RDMA, TCP, UDP Engine  
  - Packet Processing Engine, Ethernet, Infini Band Controller  
 4) 메모리 서브시스템  
  - DRAM, On-chip Memory  
 5) 호스트, 주변장치 인터페이스  
  - PCIe Switch (Host 연결), SSD, GPU 연결  
 6) 외부 네트워크 인터페이스  
  - Network Ports  

### [신기술, BigUp모의고사/합숙] 프로덕트 마켓핏(Product Market Fit)

**[정의]**  

제품이나 서비스가 충분한 수의 고객에게 가치를 인정받아 그들의 요구를 충족시키며, 동시에 기업에게도 지속 가능한 수익을 창출하는 상황  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 마케팅 최적화, 수익창출, 최적 제품, MVP, 피드백 루프, 검색최적화, A/B테스트  

&lt;주요지표&gt;  
 1) 정량적 : 성장률, 순추점점수, 재방문율, 고객 생애 가치, 고객 획득 비용, 40% rule  
 2) 정성적 : 입소문, 추천, 시장 반응  

### [신기술, BigUp모의고사/합숙] 데이터 오염 공격

**[정의]**  

공격자가 의도적으로 잘못된 정보를 포함한 데이터를 학습 데이터셋에 추가함으로써, 모델이 잘못된 패턴을 학습하도록 유도하는 공격  

**[핵심/키워드]**  

&lt;목적&gt;  
 - 정확도 저하, 백도어 삽입  

&lt;공격방법&gt;  
 1) 라벨 조작, 2) 샘플 추가, 3) 데이터 비율조정  

&lt;공격유형&gt;  
 - Label Flipping, backdoor injection, clean-label poisoning, feature collision  

&lt;대응방안&gt;  
1) 데이터 검증필요, 2) 모델 견고성 강화, 3) 앙상블 기법  

### [신기술, BigUp모의고사/합숙] 안전한 다자간 연산(SMPC, Secure Multi-Party Computation)

**[정의]**  

여러 참여자가 각자의 입력값을 외부에 공개하지 않고, 공동으로 특정 함수 연산 결과만을 안전하게 계산하는 암호기술  

**[핵심/키워드]**  

&lt;핵심 원리&gt;  
 - 개인 입력값은 비밀, 계산 과정에서 노출없음  

&lt; 매커니즘 절차 &gt;  
 1) 참여자들 간 데이터 수집  
 2) 암호화를 통해 다른 참여자들에게 공개없이 연산  
 3) 통계 및 연산 후 관심 데이터 생성, 공유  

&lt;대표 기법&gt;  
 1) 비밀공유 (Secret Sharing)  
  - 비밀을 여러 조각으로 나누어 분배  
  - 일정 수 이상의 조각을 모아야 원래 비밀 복원 가능  
  - 예: Shamir’s Secret Sharing  
 2) 임계값 서명 (Threshold Signature)  
  - 여러 참여자가 협력해 디지털 서명 생성  
  - 개인 키 유출 방지, 일부 참여자 불참 시에도 서명 가능  
  - 비밀공유의 응용 사례  
 3) 동형암호 (Homomorphic Encryption)  
  - 암호화된 데이터 상태에서 덧셈·곱셈 연산 수행  
  - 복호화 시 최종 결과만 확인 가능  
 4) 가비지 서킷 (Garbled Circuit)  
  - 연산 과정을 암호화된 회로로 표현  
  - 입력값을 넣으면 결과만 도출, 중간 과정 노출 없음  

### [신기술, BigUp모의고사/합숙] 스핀락(Spin Lock)

**[정의]**  

임계 구역에 진입이 불가능할 때 진입이 가능할 때까지 루프를 돌면서 재시도하는 방식으로 구현된 락킹(locking) 매커니즘  

**[핵심/키워드]**  

* Busy Waiting, 짧은 시간 Lock 획득  
 * spin-lock timeout, Polling 반복 확인  
 * 간단한 구현, 문맥교환 오버헤드 없음  

&lt;유형&gt;  
 - 기본 스핀락, Target 스핀락, MCS 스핀락  

### [신기술, BigUp모의고사/합숙] Able Tech

**[정의]**  

단순한 의료 용품과 보조 기기를 넘어 IT 기술과 결합하여 근본적인 문제 해결에 도움을 줌으로써 장애인의 불편을 덜어주는 기술  

**[핵심/키워드]**  

* 장애인 불편해소, 포용성  

&lt;기술&gt;  
 1) 감지/입력 : 센서, 시선추적, BCI, 음성인식, 터치스크린  
 2) 출력/피드백 : 텍스트 음성 변환, 햅틱, 촉각 피드백, 로보틱스, 실시간 자막, 음성 문자  
 3) 인식/지능 : 컴퓨터비전, NLP, AI, ML  
 4) 통신/플랫폼 : IoT, VR, AR, 클라우드 서비스  

### [신기술, BigUp모의고사/합숙] 2-3 Tree

**[정의]**  

모든 내부 노드가 두 개 또는 세 개의 자식을 가지며, 모든 리프 노드가 동일한 레벨(깊이)에 위치하는 균형 트리  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 다진트리, 균형 트리(리프 깊이 동일),노드 유형(2-node,3-node),정렬된 키,  
 - 탐색 효율(O(logn)),삽입 시 분할,삭제 시 병합/재배치  

&lt;시간복잡도&gt;  
 - 삽입/삭제/탐색 : O(logn)  

&lt;구성요소&gt;  
 - 2-node : 키 1개 + 자식 2개  
 - 3-node : 키 2개 + 자식 3개  
 - Internal Node : 1개 이상의 자식을 가진 노드, 트리의 분기점 역할  
 - External Node : 자식이 없는 노드, 즉 리프 노드와 동일  
 - 키 (Key) : 정렬 기준 값. 노드 내부에서 오름차순 정렬됨  
 - 자식 포인터 : 하위 노드를 가리키는 링크  
 - 균형 조건 : 모든 리프노드가 같은 깊이를 유지해야 함  

&lt;연산&gt;  
 - 삽입 : 분할(Split) → 3-node에 삽입 시 중간 키 부모로 올리고 분리  
 - 삭제  
 - 병합(Merge) → 키 삭제 후 형제도 2-node이면, 형제+보무 키와 합침  
 - 재분배(Redistribution) → 키 삭제 후 형제가 3-node이면, 형제에게서 키 빌림+부모 키 재배치  

### [신기술, BigUp모의고사/합숙] OT 특화 제로트러스트

**[정의]**  

산업 제어 설비(OT) 환경에 맞춰서 모든 것을 신뢰하지 않는다는 기본 원칙을 따르는 보안모델  

**[핵심/키워드]**  

&lt;도입원칙&gt;  
 - 실시간성, 가용성, OT 장비 독립성, 지속적 모니터링, 침해가정  

&lt;특성&gt;  
 - 운영목표 : 가용성.실시간성 최우선  
 - 시스템구조 : Purdue모델 기반 계층 구조  
 - 프로토콜 : 전용·비공개 산업 특화  
 - 제약사항 : 암호화·인증 기술 적용 제한  

&lt;적용 프로세스&gt;  
 1) 자산식별 / 대상 정의, 2) 운영흐름 가시화, 3) 아키텍처 설계, 4) 정책수립/구현, 5) 지속적 모니터링 / 유지관리  

### [신기술, BigUp모의고사/합숙] EDF(Earliest Deadline First)

**[정의]**  

임의의 실행시점에서 가장 가까운 마감시간을 기준으로 우선순위가 동적으로 부여되는 스케줄링  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 동적 우선순위 (마감시간에 따라 우선순위), 선점 스케줄링 (더 이른 마감이 선점)  
 - 최적 알고리즘 (CPU 활용률 극대화 100%), 실시간 적합, 기아발생 가능  

&lt;단계&gt;  
 1\. 태스크 도착  
 2\. 실행 큐 삽입  
 3\. 우선순위 결정 : 가장 이른 마감시간 선택  
 4\. 선점 조건 검사  
 5\. 태스크 실행  
 6\. 완료 후 다음 태스크  
 7\. 반복 수행  

### [신기술, BigUp모의고사/합숙] SP인증

**[정의]**  

SW기업 및 개발 조직의 SW프로세스 품질역량 수준을 심사하여 등급을 부여하는 제도  

**[핵심/키워드]**  

&lt;법적근거&gt;  
 - 소프트웨어 진흥법 제21조, 같은 법 시행령 제18조 ~ 제22조, 같은 법 시행규칙 제8조부터 제11조  

&lt;인증기준&gt;  
 - 5개영역, 16개 항목, 63개 세부항목  
 - 5개영역 (개발, 프로젝트관리, 지원, 조직관리, 프로세스개선)  

&lt;인증등급&gt;  
 - 1등급 (개발), 2등급 (개발, 프로젝트관리, 지원), 3단계 (5갱영역)  

&lt;인증절차&gt;  
 - 인증신청 → 계약 → 현장심사 → 인증심의 → 인증결과  

<유효기간/연장/대상>
 - 유효기간 : 신규 (3년), 연장 (2년)  
 - 심사대상 : 기업  / 조직  

&lt;혜택&gt;  
 - SW 기술성 평가 시 우대, 사업자 선정 시 인센티브 부여, 하도급 계약 적정성 판단 가산점  

### [신기술, BigUp모의고사/합숙] EAI(Enterprise Application Integration)

**[정의]**  

기업 내 다양한 이기종 시스템(ERP, CRM, SCM 등)을 유기적으로 연동하고 통합하여, 데이터 흐름과 비즈니스 프로세스를 자동화 및 최적화 기술 및 접근 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 구조 : 허브 앤 스포크(Hub & Spoke) 중앙 집중형  
 - 통합 방식 : 커넥터 기반, 특정 플랫폼 의존적  
 - 유연성 : 확장성과 유연성 제한  
 - 목적 : 내부 애플리케이션 통합 중심  
 - 구현 비용 : 초기 비용 및 유지보수 비용 높음  
 - 확장성 : 중앙 허브의 한계로 확장성 낮음  

 - EAI : 이기종 시스템 통합, 내부  
 - ESB : EAI 구현, 서비스 지향, SOA  
 - API G/W : 내부 API 외부 제공, 중간통로  
 - Service Mesh : 내부 서비스 통신 조율  

### [신기술, BigUp모의고사/합숙] LIME(Local Interpretable Model-agnostic Explanations)

**[정의]**  

복잡한 머신러닝 모델의 예측 결과를 개별 사례(로컬) 단위로 해석하기 위해, 해당 사례 주변에서 단순하고 해석 가능한 대체 모델(예: 선형 회귀, 의사결정나무)을 학습시켜 설명을 제공하는 기법  

**[핵심/키워드]**  

&lt;특징&gt;  
 - 특정 예측 결과에 대한 지역적 해석, 모델 비종속적, 부분적  
 - 부분적으로 단순화된 근사 모델, local surrogate model  

&lt;동작절차&gt;  
 - 대상 샘플 선택 → 데이터 주변 샘플링 → 모델 예측 실행 → 가중치 부여 → 단순 모델 학습 → 설명 생성  

### [신기술, BigUp모의고사/합숙] 지식 그래프(KG, Knowledge Graph)

**[정의]**  

현실 세계의 개체(Entity)와 관계(Relation)를 그래프 구조로 표현해 의미적 연결과 추론을 가능하게 하는 지식 표현 방식  

**[핵심/키워드]**  

&lt;그래프 이론 기반 표현방식&gt;  
 - 노드(Node) : 엔티티(Entity)  
 - 엣지(Edge) : 관계(Relationship)  
 - 속성(Attribute) : 엔티티나 관계의 특성  

&lt;데이터 중심 표현방식&gt;  
 - 엔티티(Entity) : 사람,장소,사물,개념  
 - 속성(Attribute) : 엔티티 특성(이름,나이,위치 등)  
 - 관계(Relationship) : 엔티티 간 의미적 연결(예:A-고용→B)  

&lt;지식 그래프의 지식 표현 체계&gt;  
 - 온톨로지(Ontology) : 개념·관계 정의 체계  
 - RDF(Resource Description Framework) : 웹 표준 데이터 표현 언어  
 - SPARQL : 그래프 질의(Query)언어  
 - 트리플 저장소(Triple Store) : RDF기반 데이터 저장 시스템  
 - 그래프 데이터베이스 : Neo4j,TigerGraph 등  
 - 추론 엔진(Inference Engine) : 논리 규칙 기반 자동 추론  
 - 엔티티 정규화(Entity Linking) : 동일 개체 식별·연결  

&lt;구성절차&gt;  
 - 지식 수집 (텍스트, DB, 로그 등에서 개체·관계 추출)  
 - 지식 정규화 (개체 통합, 관계 표준화)  
 - 그래프 구축 (노드/엣지로 모델링, Triple 생성)  
 - 지식 저장/관리 (그래프 DB, 예: Neo4j)  
 - 질의/추론 (SPARQL, 규칙 기반, 임베딩 활용)  
 - 지식 확장 (새로운 데이터 반영, 지속적 업데이트)  

### [신기술, BigUp모의고사/합숙] SSPL(System&Software Product Line) 개발 방법론

**[정의]**  

핵심 자산(Core Asset)의 공통성과 가변성을 기반으로 관련 제품군을 효율적으로 개발하는 방식  

**[핵심/키워드]**  

* ISO/IEC 26550  

&lt;특징&gt;  
 - 공통성 : 모든 제품 공유, 재사용  
 - 가변성 : 제품별로 선택, 대안 특징  

&lt; 프로세스&gt;  
 - 도메인공학 : 핵심 자산 개발  
 - 애플리케이션 공학 : 맞춤형 개별 제품 개발  

### [신기술, BigUp모의고사/합숙] 포아송 분포(Poisson Distribution)

**[정의]**  

단위 시간 또는 단위 공간에서 발생하는 사건의 수를 모델링하는 이산 확률분포  

**[핵심/키워드]**  

&lt;가정사항&gt;  
 1) 독립성 : 서로 다른 구간에서의 사건의 수는 서로 독립  
 2) 비례성 : 짧은 구간에서의 사건 발생 확률은 길이에 비례  
 3) 희소성 : 짧은 시간에 두 번 이상 발생 확률은 매우 작음  
 4) 일관성 : 특정 단위 내에서의 사건 발생 확률은 동일  

&lt;특징&gt;  
 * 기대값 =  분산 = 평균 =  λ  
 * λ가 클수록 정규분포 근사  
 * 이항분포의 극한 형태  

### [신기술, BigUp모의고사/합숙] 프롬 스크래치(From Scratch)

**[정의]**  

기존 모델이나 가중치를 사용하지 않고 데이터 수집부터 모델 학습까지 전 과정을 자체 수행하는 방식  

**[핵심/키워드]**  

&lt;특징&gt;  
 - zero base, 모델, 구조, 가중치 없음, 대규모 클러스터 필수, 높은 개발비용, 장기간 개발  
 - 느린 개발속도, 최고수준 데이터 주권  

&lt;유형&gt;  
 - 완전, 아키텍처, 데이터, 도메인, 시스템 프롬 스크래치  

&lt;대표기법&gt;  
 - 대규모 사전학습, 자기지도학습, 대규모 분산학습  

&lt;활용&gt;  
 - 소버린 AI, 국가대표 AI  

### [신기술, BigUp모의고사/합숙] 델타레이크(Delta Lake)

**[정의]**  

기존 데이터 레이크 위에 ACID 트랜잭션, 데이터 버저닝, 스키마 검증 및 스키마 진화와 같은 데이터 관리 기능을 제공하는 오픈소스 저장 계층  

**[핵심/키워드]**  

<특징/기능>
 - 데이터레이크 + ACID 트랜잭션, 데이터 버저닝, Schema-On-Read, 높은 기술 복잡도  
 - 메달리온 아키텍처 (Bronze → Silver → Gold)  

### [신기술, BigUp모의고사/합숙] EVM(Earned Value Management)

**[정의]**  

프로젝트의 계획된 일정과 범위를 비용관점으로 정량화 하여 계획대비 실적을 확인하는 성과위주의 위험 사전 예측 기법  

**[핵심/키워드]**  

&lt;목적&gt;  
 - 수주자 관점 : 내부비용, 일정 통제방안  
 - 발주자 관점 : 제품 측면의 개발 진척도 분석  

&lt;기대효과&gt;  
 - 획득가치기준, 프로젝트 가시화, 위험 조기 대응  

&lt;주요지표&gt;  
 - 측정요소 : PV, EV, AC, BAC  
 - 분석요소 : SV, CV, SPI, CPI  
 - 예측요소 : ETC, EAC, TCPI, VAC  

### [신기술, BigUp모의고사/합숙] PCB (Process Control Block)

**[정의]**  

프로세스마다 고유하며, 커널 내 위치하여 문맥 교환이 발생하면 현재 점유중인 프로세스의 문맥 정보를 저장하는 자료구조  

**[핵심/키워드]**  

* 프로세스마다 고유 PCB  

&lt;특징&gt;  
 - 고유식별 ID, 상태정보 저장, 스케쥴링 기초, 커널 공간, 문맥교환  

&lt;구성&gt;  
 - 프로세스 식별자, 프로세스 상태, 메모리 포인터, 프로그램 카운터,  
   레지스터, 스케줄링 정보, 계정정보, I/O 정보, Paget Table, List of File  

### [신기술, BigUp모의고사/합숙] SNAP(Software Non-functional Assessment Process)

**[정의]**  

소프트웨어의 비기능적 요구사항(Non-functional Requirements)의 크기를 정량적으로 측정하는 국제 표준 방법론  

**[핵심/키워드]**  

* FP 한계 보완, 비기능 요구사항 크기, ISO/IEC/IEEE 32430:2025  
* AI 규모 산정 지원 가능, 4개 카테고리, 14개 서브카테고리  

&lt;4개 카테고리&gt;  
 - 데이터 운영, 인터페이스 설계, 기술 환경, 아키텍처  

&lt;절차&gt;  
 - 비기능 요구사항 식별 → 서브 카테고리 식별 → 비기능 규모 식별 → 규모계산 → 기술요소 예산 도출  

### [신기술, BigUp모의고사/합숙] AI 에이전트 하이재킹(AI Agent Hijacking)

**[정의]**  

공격자가 직접 AI 모델을 공격하는 대신, 에이전트가 처리하는 데이터나 환경을 조작, 에이전트의 판단과 실행 과정을 가로채는 공격기법  

**[핵심/키워드]**  

* OWASP Top 10 for Agentic Applications for 2026  

&lt; 특징 &gt;  
 - 에이전트 목적 악의적 변경, 데이터 탈취 및 오남용, 에이전트 판단 및 실행 탈취  

&lt; 공격 &gt;  
 1\. 공격자 데이터 오염 > 2. 사용자 작업 지시 > 3. AI Agent 작업 데이터 확인 >  
 2\. 공격자의 작업 지시 / AI Agent Hijacking > 5. 공격자의 작업 수행 >  
 3\. 사용자 작업 완료 응답  

&lt; 대응 &gt;  
 - Agent 추적, 최소권한, 실시간 모니터링, 지시문 분리, 프레임워크 검증  
 - OWASP의 AI Agent 보안 위험 식별 평가 프레임워크 등 활용  

