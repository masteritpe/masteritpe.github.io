---
layout: post
title: "WritingDrill_Rounds_6"
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

### [보안] 백도어 (Backdoor) 공격

**[정의]**

컴퓨터 시스템, 암호화 시스템 또는 알고리즘의 보안을 우회하여 원격으로 접속하고 악성코드를 실행할 수 있게 하는 비밀 통로를 이용한 공격기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 보안 우회, 비밀 통로, 원격 접속, 악성코드 실행, 데이터 탈취

&lt; 유형 &gt;
* 시스템, 소프트웨어, 네트워크

&lt; 절차 &gt;
1\. 침투 및 백도어 설치 
2\. 원격 제어 및 시스템 통제 
3\. 추가 악성행위 실행 
4\. 은닉 및 지속적 피해

&lt; 탐지 &gt;
* 프로세스 확인, 네트워크 연결확인, 파일 시스템 점검, 로그 파일 분석, 백도어 스캐너 사용

&lt; 조치 &gt;
* 프로세스 종료 및 파일 삭제, 네트워크 차단, 보안 업데이트, 원격 접근 차단, 백신, 무결성 확인 도구, 강력한 인증, 방화벽, 접근최소화

&lt; 백도어 취약점 활용 사례 &gt;
* BPFDoor, XZ-Utils 백도어 취약점

### [보안] DDoS (Distributed Denial of Service)

**[정의]**

다수의 공격자(좀비 PC, 봇넷 등)를 이용해 동시에 특정 서버나 네트워크에 과도한 트래픽을 발생시켜 정상적인 서비스를 방해하는 공격

**[핵심/키워드]**

&lt; 특징 &gt;
* 분산공격, 대규모 트래픽, 가용성 저하, 좀비 PC, 봇넷

&lt; 절차 &gt; 
1\. 악성코드 은닉 
2\. 악성코드 감염(좀비 PC, Agent 감염) 
3\. 감염 사실 은폐 및 명령 대기 
4\. DDoS 공격 수행 (공격자의 C&C 서버에 의한 제어)

&lt;대응방안&gt; 
* ACL 적용, 공격 IP 차단, SYN Proxy 사용, 보안 패치/장비 교체, 서버 설정 변경, 웹서버 증설, 불필요한 서비스 차단, 공격자 IP 차단, DNS 서버 다중화, DNS 전용회선 준비, IP 필터링, 지리적 차단, 의심 트래픽 필터링, 트래픽 이상 감지, AI 기반 분석 도입, Blackhole / Sinkhole 라우팅

&lt; 고도화 공격 &gt; 
* DRDoS (분산반사 서비스 거부 공격, Distributed Reflected Denial of Service),
Ransom DDos, Multi-Vector DDos

### [보안] 부채널공격 (Side Channel Attack)

**[정의]**

실제구현 과정에서 발생하는 물리적 정보 (시간, 전력, 소리, 전자파 등)를 분석하여 비밀 정보를 추출하는 공격방식

**[핵심/키워드]**

&lt; 분류 &gt;
* 제어 / 능력 (소극적 Passive, 적극적 Active) 
* 모듈접근 (침입 Invasive, 준침입 Semi-invasive, 비침입 Non-Invasive) 
* 전력분석 (단순 SPA, 차분 DPA (Differential))
* 공격대상 (하드웨어 Hardware, 소프트웨어 Software, 암호) 

&lt; 유형 &gt;
* 소요시간 (Timing), 오류 (Fault), 오류 메시지 (Error Message), 전력 분석, 전자파 분석, Tempest, Cold Boot, Cache Side Channel (Meltdown, Spectre), Dolphin

&lt; 잘차 &gt;
1\. 정보수집 (Timing, power)
2\. 정보분석 (키 추론)
3\. 정보추출

&lt; 대응 &gt;
* Fixed Time, 전력 균등화, 무작위 지연, 차폐, 메모리 암호화, 오류 감지 회로 내장, 최신버전 업데이트, Secure Boot

### [보안] 스턱스넷(Stuxnet)

**[정의]**

폐쇄망을 USB로 뚫고, 제로데이와 루트킷으로 은폐 확산한 뒤, PLC 코드를 변조해 고도화된 산업제어시스템(ICS/SCADA)을 공격하는 악성코드

**[핵심/키워드]**

&lt; 특징 &gt;
* 루트킷, USB, PLC, SCADA

&lt; 단계 &gt;
1\. UBS 감염 전파 
2\. 산업 시스템 탐색 
3\. PLC 감염 
4\. 물리시스템 교랸

&lt; 대응 &gt;
* 저장매체 보안관리, 시스템 패치, 전용 백신, 비밀번호 정책 강화, 보안 감사, 전사 보안, 망분리

### [보안] 공격표면관리 (ASM, Attack Surface Management)

**[정의]**

인터넷 등 외부에서 수집 가능한 모든 디지털 정보를 분류, 분석, 우선순위 지정하여 지속적으로 모니터링하고 위험을 사전에 식별 및 차단하는 보안 프로세스

**[핵심/키워드]**

&lt; 특징 &gt;
* 위협 관리, 자산 관리, 가시성, Zero Trust, 위험 경고

&lt; 공격 표면 유형 &gt;
* 외부 (도메인, API), 내부 (내부망, 사내 시스템), 동적 (클라우드, CI/CD, BYOD)

&lt; 공격 표면 관리 유형 &gt;
* 사이버자산 (CAASM), 외부공격 (EASM), 디지털 위험 보호 서비스 (DRPS)

&lt; 관리 방법 &gt;
* 공격 표면 식별, 공격 표면 관리 자동화, 공격 표면 최소화

&lt; 관리 방안 &gt;
* 디지털 발자국 발견, 자산 재고 및 분류, 지속적 보안 모니터링, 자산 사칭 및 사고 모니터링, 위험 감지 및 식별

### [보안] RBAC (Role-BasedAccessControl)

**[정의]**

사용자의 역할(Role)에 따라 시스템 자원에 대한 접근 권한을 부여하는 접근통제 모델

**[핵심/키워드]**

&lt; 특징 &gt;
* 접근 통제 모델, 역할 기반

&lt; 구분 &gt;
* 권한관리, 역할분배, 최소권한, 직무분리, 객체분류

&lt; 구성 &gt;
* User, Role, Permission, Session

&lt; 연관 &gt;
* 정책 (DAC, MAC, ABAC, CapBAC), 모델 (Lattice, Clark & Wilson, 만리장성)

### [보안] 스푸핑(Spoofing)

**[정의]**

공격자가 허위 정보를 조작하거나 위조하여 자신을 다른 사용자나 시스템으로 가장하는 공격 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 정보 조작 및 위조, 적극적 공격 (Active)

&lt; 유형 &gt; 
* IP 스푸핑, ARP 스푸핑, DNS 스푸핑, ICMP Redirect 공격, 이메일 스푸핑, 웹사이트 스푸핑, MAC 스푸핑 

&lt; 절차 &gt;
1\. 공격대상 정보 수집 
2\. 공격대상 식별 및 위조 
3\. 공격실행 및 유출

&lt; 대응 &gt; 
* IP 스푸핑 : Ingress 필터링, 위조 IP 차단
* ARP 스푸핑 : 정적 ARP, DAI(Dynamic ARP Inspection)
* DNS 스푸핑 : DNSSEC(DNS Security Extensions), DoH, DoT 
* ICMP Redirect 공격 : ICMP Redirect 메시지 수신 차단
* DDoS 공격 : 트래픽 필터링, 속도 제한(Rate Limiting), Anti-DDoS

### [보안] LOTL (Living off the Land,시스템내 자원활용 공격)

**[정의]**

공격자가 외부 악성코드 없이 운영체제(OS)나 시스템에 기본적으로 존재하는 정식도구를 이용해 공격을 수행하는 방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 탐지 회피, 내장 도구 악용, 권한 상승, LOT Bins

&lt; 공격절차 &gt;
1\. 초기 접근 (소셜 엔지니어링, SW 취약점) 
2\. 도구 악용 (Power Shell, BASH, WMI, PsExec) 
3\. 내부확산 (권한 상승, NW 확산) 
4\. 은밀한 활동 (데이터 탈취, 지속성 확보) 
5\. 흔적 제거 (로그 삭제 및 은페)

&lt; 대응방안 &gt;
* 권한 최소화, 사용 도구 통제, 행위 기반 탐지, 로그 정밀 분석, EDR, XDR, SBOM, 사용자 보안 교육

### [보안] 동형암호화 (Homomorphic Encryption

**[정의]**

암호화된 데이터(암호문)를 복호화하지 않고도 덧셈, 곱셈 등의 연산을 수행할 수 있는 암호기술

**[핵심/키워드]**

&lt; 특징 &gt;
* 복화화 없음, 프라이버시 보존

&lt; 종류 &gt;
* 부분동형 (Partially) 암호화, 준동형 (Somewhat) 암호화, 단계적 완전동형 (Leveled Fully) 암호화, 완전동형 (Fully) 암호화

&lt; 기술유형 &gt;
* Gen09, DGHV10, CRT-Based

&lt; 알고리즘 &gt;
* Pailler, RSA, BGV, BFV, CKKS, TFHE, HeaAN, Helib

### [보안] ISO/IEC 27014

**[정의]**

정보보안 거버넌스를 효과적으로 수립·유지·모니터링하기 위한 원칙과 모델을 제공하는 국제 표준

**[핵심/키워드]**

&lt; 원칙 &gt;
* 책임 (Responsibility), 전략 (Strategy), 확보 (Acquisition), 성과 (Performance), 준수 (Conformance), 행동 (Human Behavior) 

&lt; 프로세스 &gt;
* 평가 (Evaluate), 지시 (Direct), 모니터링 (Monitoring), 소통 (Communicate), 정책 일치 (Policy Alignment), 보증 (Assurance)

&lt; 기반 &gt;
* ISO/IEC 38500

### [보안] 제로트러스트 성숙도 모델 2.0

**[정의]**

조직의 보안 시스템이 제로 트러스트 원칙에 얼마나 성숙하게 대응하고 있는지를 측정하는 도구

**[핵심/키워드]**

&lt; 도입절차 &gt;
1\. 준비 (현재수준, Prepare)  
2\. 계획 (설계, Plan) 
3\. 구현 (솔루션, Implement) 
4\. 운영 (Operate) 
5\. 피드백 및 개선 (Feedback & Improvement)

&lt; 성숙도 수준 &gt;
* 기존 (Traditional), 초기 (Initial), 고급/향상 (Advanced), 최적화 (Optimal)

&lt; 주요 영역 &gt;
* 식별자 및 신원 (Identity), 기기 및 엔드포인트 (Devices), 네트워크 (Networks), 시스템 (System), 애플리케이션 및 워크로드 (Applications & Workloads), 데이터 (Data)

&lt; 주요 기능 &gt;
* 가시성 및 분석 (Visibility & Analytics), 자동화 및 오케스트레이션 (Automation & Orchestration), 거버넌스 (Governance)

### [보안] 국가망보안체계 (National Network Security Framework, N2SF)

**[정의]**

국가 공공기관에서 업무 중요도에 따라 기밀(Classified), 민감(Sensitive), 공개(Open) 등 3개 등급으로 분류, 차등적인 보안 통제를 적용, 보안성과 데이터 공유를 동시에 달성하는 정책

**[핵심/키워드]**

&lt; 특징 &gt;
* 등급 (기밀, 민감, 공개), 제로 트러스트 (Zero Trust), 차등적 보안통제

&lt; 적용절차 &gt;
1\. 준비 (Prepare) 
2\. 등급분류 (Categorize) 
3\. 위협식별 (Identify) 
4\. 보안대책수립 (Select) 
5\. 적절성 평가 및 조정 (Assess)

&lt; 등급 &gt;
* 기밀 (안전 직결, Classified), 민감 (침해가능성, Sensitive), 공개 (기밀, 민감 외 공개 가능, Open)

&lt; 연관 &gt;
* 다증계층 보안체계 (Multi Level Security, MLS)

### [보안] ISMS-P 간편인증제도

**[정의]**

영세 및 중소 기업의 ISMS-P 인증 편입을 촉진, 경량화된 인증기준, 저렴한 인증 수수료, 기간 단축 등 기업 부담을 완화한 간이 ISMS-P 인증제도

**[핵심/키워드]**

&lt; 목적 &gt;
* 중소기업 대상, 기업 부담 완화, 인증 기간 단축

&lt; 인증대상 &gt;
* 소기업, 300억 미만 중기업, 주요정보통신설비 미보유 기업

&lt; 대상 불가 &gt;
* ISP, IDC, 상급종합병원, 금융회사, 가상자산사업자

&lt; 인증 항목 수 &gt;
* 소기업 / 300억 미만 ISMS-P (관리체계 8, 보호대책 33, 개인정보 21), 101개 → 62개
* 300억이상 시설 미운영 (관리체계 11, 보호대책 33, 개인정보 21), 101개 → 65개

&lt; 연관 &gt;
* ISMS-P 인증, 금융 ISMS-P

### [보안] IAST (Interactive Application Security Testing)

**[정의]**

애플리케이션 실행 중 내부 코드 흐름과 외부 요청/응답을 동시에 분석하여 정적 + 동적 분석을 결합한 보안 테스트 기법 

- DevSecOps, DevOps

**[핵심/키워드]**

&lt; 특징 &gt;
* 정적 + 동적 보안취약점 분석 테스트 
* 내부 센서(Agent) 삽입, 코드 수준 추적 + 요청 이벤트 분석 병행 

&lt;주요 매커니즘&gt; 
* 코드 실행 여부(실행함), 테스트 위치(내부 흐름 + 외부 요청 동시 분석), 정확도(높음), 적용 시점(개발~테스트 연속 가능), 통합 가능성(DevSecOps 최적화)

&lt; 대표 도구 &gt;
* Contrast, Seeker, Veracode IAST

&lt; 활용 &gt;
* DevSecOps, CI/CD

&lt; 연관 &gt;
* 테스트 (SAST, DAST), 운영 (RASP)

### [보안] 프라이버시보호기술 (PET: Privacy Enhancing Technologies)

**[정의]**

개인정보를 수집, 처리, 분석, 공유하는 과정에서 개인의 프라이버시를 보호하기 위한 기술의 집합

**[핵심/키워드]**

&lt; 특징 &gt;
* 프라이버시 보호

&lt; 도구 &gt;
* 데이터 난독 (차분 프라이버시, 합성 데이터, 영지식 증명)
* 암호화된 정보 (동형암호 (HE), 신원기반 암호 (IBE), 안전한 다자연산 (SMPC), 기밀 컴퓨팅, 신뢰받는 실행환경 (TEE))
* 연합 및 분산분석 (연합학습 (FL), 분산분석, 프라이버시 보호형 AI (PPAI)
* 데이터 책임 (책임 시스템, 개인정보 관리 시스템, 개인집합 교차연산)

&lt; 반대 &gt;
* PIT (Privacy Invading Technology, 개인정보 침해)

### [보안] ABAC (Attribute-BasedAccessControl)

**[정의]**

사용자, 자원, 환경 등의 속성(attribute)을 기반으로 접근 허용 여부를 동적으로 판단하는 접근통제모델

**[핵심/키워드]**

&lt; 특징 &gt;
* 속성+규칙, 유연, 동적

&lt; 절차 &gt;
1\. 접근요청 
2\. 평가시작 
3\. 정책 / 속성 검색 
4\. 정책/속성 확인 
5\. 접근평가 
6\. 결과 집행

&lt; 구성 &gt;
* 접근제어 (주체, 행동, 객체)
* 정책 결정 및 실행 (정책 결정 지점 (PDP), 정책 집행 지점 (PEP))
* 속성 기반 (정책 정보 제공 (PIP), 주체속성, 객체속성, 환경속성)
* 정책/규칙 (정책 관리 지점 (PAP), 정책 검색 지점 (PRP))

&lt; 활용 &gt;
* 제로 트러스트, 클라우드

&lt; 연관 &gt;
* RBAC, CapBAC, DAC, MAC

### [보안] 전자서명 (Electronic Signature)

**[정의]**

서명자의 신원을 확인하고, 전자문서의 위변조 여부를 검증하기 위해 전자적 방식으로 생성된 데이터

**[핵심/키워드]**

&lt; 특징 &gt;
* 위조불가, 서명자 인증, 부인방지, 변경불가, 재사용불가, 분쟁해결가능

&lt; 구성요소 &gt;
* 서명 생성 (문서, 해시함수, 개인키, 서명알고리즘, 전자서명, 디지털 인증서)
* 서명 검증 (공개키, 전달된 해시값, 복호화된 해시값, 비교 단계)
* 보안 및 부가요소 (타임스탬프, 키관리, 보안프로토콜, 생체인식)

&lt; 적용 알고리즘 &gt;
* 기본 (RSA, DSA), 차세대 (ECDSA, KCDSA), 양자내성

&lt; 생성절차 &gt;
1\. 원문 
2\. 해시함수 
3\. 해시값 암호화 (개인키)
4\. 원문+서명 전송

&lt; 확인절차 &gt;
5\. 원문 해시값 계산 
6\. 서명 복호화  (공개키)
7\. 해시값 비교 
8\. 확인결과 판단

### [보안] 사회공학 (Social Engineering)

**[정의]**

인간 상호작용의 깊은 신뢰를 바탕으로 사람들을 속여, 정상 보안절차를 깨뜨리고 비기술적인 수단으로 정보를 얻는 행위

**[핵심/키워드]**

&lt; 특징 &gt;
* 신뢰, 심리, 보안우회

&lt; 공격절차 &gt;
1\. 정보수집 
2\. 관계형성 
3\. 공격 및 실행

&lt; 공격유형 &gt;
* 인간기반 (직접 접근, 도청, 훔쳐보기, 휴지통 뒤지기, 프리텍스팅, 테일게이팅, 피기백킹, 퀴드 프로 쿼, 비싱, 페이퍼 피싱)
* 컴퓨터기반 (피싱, 스미싱, 파밍, 악성 소프트웨어, 디지털 포렌식 악용)
* 물리적 (베이팅, USB 드롭)

&lt; 대책 &gt;
* 인간 (교육, 출입통제, 비인가 절차화, 감시 및 신고 체계)
* 컴퓨터 (필터링, 멀웨어 탐지, 2단계 인증, 브라우저 보안 강화, DNS 보호)
* 물리적 (외부 저장장치 통제, 문서보안 폐기, 감시장비, 무단장비 반출입 차단)

### [보안] APT (Advanced Persistent Threat)

**[정의]**

특수목적을 가진 공격자가 피해 대상을 표적으로 삼고 다양한 IT기술과 방식들을 이용해 지속적으로 정보를 수집하고 취약점을 파악하여 이를 바탕으로 피해를 끼치는 공격

**[핵심/키워드]**

&lt; 특징 &gt; 
* 지능성 (Advanced), 지속성 (Persistent), 목표지향성 (Targeted), 조직성 (Organized) 

&lt; 공격절차 &gt; 
1\. 침입 (Incursion) : 사회공학, 제로데이 취약점, 수동 공격, 탐색
2\. 탐색 (Discovery) : 관찰, 탐색, 다중 벡터, 은밀한 활동, 연구 및 분석
3\. 수집 (Capture) : 수집, 은닉, 권한 상승
4\. 유출 및 제어 (Exfiltration & Control) : 유출/제어, 유출, 중단 

&lt; 대응방안 &gt; 
* 관리적 대응 : 보안관리 및 운영, 보안교육 강화, 위협 인텔리전스 활용, 침해사고 대응 체계 수립
* 기술적 대응 : 엔드포인트 보안, EDR/XDR 도입, DLP 및 중요정보 암호화, 계층형 방어
접근 및 권한 관리: 접근권한관리, 다단계 인증(MFA), 네트워크 접근 제어(NAC)

### [보안] CISO (정보보호 최고책임자)

**[정의]**

조직 내 정보보호 및 보안 전반을 총괄하는 최고 책임자로, 정보보호 정책 수립, 위험관리, 보안 사고 대응, 보호대책 운영 등을 담당하는 임원급 역할

**[핵심/키워드]**

&lt; 근거 &gt;
* 정보통신망법, 제45조의3(정보보호 최고책임자의 지정 등) 

&lt; 역할 &gt; 
* 정보보호 계획 수립 및 개선, 정보보호 실태 감사 및 개선, 위험 식별 및 대책 마련, 정보보호 교육·훈련 계획 수립 및 시행, 정보보호 공시 업무 (정보보호산업법), 기반보호법상 정보보호책임자 업무, 전자금융거래법상 CSO 업무, 개인정보보호법상 개인정보 보호책임자(CPO) 업무, 기타 정보보호 관련 법령상 업무

### [보안] 암호문 공격 (Crypt Analysis)

**[정의]**

암호문과 평문을 가지고 평문과 암호문을 알아내거나 암호화하는데 쓰인 알고리즘이나 키를 알아내는 방법

**[핵심/키워드]**

&lt; 종류 &gt;
* 암호문 단독 (COA), 알려진 평문 (KPA), 선택 평문 (CPA), 선택 암호문 (CCA)

&lt; 대응 &gt;
* 강력한 암호 알고리즘, 충분한 키 길이, 안전한 키 관리, 보안 인식 교육

### [보안] 클라우드보안인증제도 (Cloud Security Assurance Program, CSAP)

**[정의]**

클라우드컴퓨팅 서비스의 정보보호 수준을 정부가 인증하는 제도로, 공공기관이 안전한 클라우드 서비스를 이용하도록 보장하기 위한 제도

**[핵심/키워드]**

&lt; 근거 &gt;
* 클라우드 발전법 제23조의 2

&lt; 인증유형 &gt;
* 최초 (5년), 사후 (5년동안 매년 총 4번), 갱신 (5년 연장) 
&lt; 인증등급 유형 &gt;
* 상 (물리), 중 (물리), 하(논리/물리) 

&lt; 인증기준 &gt; 
* 기존 인증제도 : IaaS (14개분야, 116개), SaaS (표준등급, 13개분야, 79개), SaaS (간편등급, 11개분야 31개), DaaS (14개분야, 110개)
* 등급제 시행 이후 : 하등급(공통, 14개분야 63개), 하등급 SaaS (11개분야 30개) 

&lt; 통제 항목 &gt;
* 정보보호 정책 및 조직 (정보보호 정책, 정보보호 조직) 
* 인적보안 (내부인력 보안, 외부인력 보안, 정보보호 교육)
* 자산관리 (자산 식별 및 분류, 자산 변경관리, 위험관리)
* 서비스 공급망 관리 (공급망 관리정책, 공급망 변경관리)
* 침해사고관리 (침해사고 대응 절차 및 체계, 침해사고 대응, 사후관리)
* 서비스연속성 (장애대응, 서비스 가용성)
* 준거성 (법 및 정책 준수, 보안 감사)
* 물리적 보안 (물리적 보호구역, 정보처리 시설 및 장비보호)
* 가상화 보안 (가상화 인프라, 가상 환경)
* 접근통제 (접근통제 정책, 접근권한 관리, 사용자 식별 및 인증)
* 네트워크 보안 (네트워크 보안)
* 데이터 보호 및 암호화 (데이터 보호, 매체 보안, 암호화)
* 시스템 개발 및 도입 보안 (시스템 분석 및 설계, 구현 및 시험, 외주 개발 보안, 시스템 도입 보안)
* 보안요구사항 (관리적 보호조치, 물리적 보호조치, 기술적 보호조치)

### [보안] 멀티팩터인증

**[정의]**

서로 다른 유형의 인증요소 2개 이상을 조합하여 인증하는 방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 2개 이상 요소 조합

&lt; 사례 &gt;
* 비밀번호 + OTP, 생체인식 + 카드

&lt; 연관 &gt;
* 2단계 인증, 멀티 채널 (Multi Channel) 인증

### [보안] TLS1.3 (Transport Layer Security1.3)

**[정의]**

TLS 1.2의 보안 취약점과 성능 문제를 개선하여 더 빠르고 안전한 통신을 제공하기 위한 프로토콜

**[핵심/키워드]**

&lt; 특징 &gt;
* TLS 1.2 보안 및 성능 개선, 1RTT, AEAD 암호, PFS 기본 적용

&lt; 표준 &gt;
* RFC 8446

&lt; 성능 개선 &gt;
* 1-RTT, 0-RTT, 연결 단축, AEAD만 허용, 불필요 기능 제거

&lt; 보안 강화 &gt;
* PFS 기본 적용, 레거시 알고리즘 제거, AEAD 강제 적용, 모든 메시지 암호화, 세션 재협상 제거

&lt; 활용 &gt;
* QUIC, HTTP/3

### [보안] IAM(Identity Access Management)

**[정의]**

사용자의 신원(Identity)을 확인하고, 해당 사용자에게 적절한 자원 접근 권한을 부여 및 관리하는 보안 프레임워크

**[핵심/키워드]**

&lt; 특징 &gt;
IAM = EAM + 감사 + 정책 + Provisioning (사용자 계정과 권한의 생성·배포·회수·삭제 자동화)

&lt; 연관 &gt;
* SSO, EAM

### [보안] 개인정보보호중심설계 (Privacy by Design, PbD)

**[정의]**

기획, 설계단계부터 개인정보보호를 고려하여, 사후 대응이 아니라 선제적으로 보호조치를 설계하는 접근방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 기획부터 보호조치 설계

&lt; 법적근거 &gt;
* 개인정보보호법 제3조 제2항

&lt; 7대원칙 &gt;
* 사전예방, 초기설정부터 보호조치, 프라이버시 보호 내재 설계, 프라이버시 보호와 사업기능 균형, 생애주기 전체 보호, 가시성 및 투명성, 프라이버시 존중

&lt; 8대전략 &gt;
* 최소화, 숨기기, 분리, 총계화, 정보제공, 통제, 집행, 입증

&lt; 활용 &gt;
* 개인정보보호중심 설계 인증제 (개인정보 처리 적법성 평가)

< 관련 표준 / 인증 >
* 국내 (PbD 인증), 유럽(EuroPrivacy, ePrivacy)
* ISO 31700 (part 1 원칙, part 2 실무지침)

### [보안] 다자간 계산 (MPC, Multi-Party Computation)

**[정의]**

서로 신뢰하지 않는 다수의 참여자가 개별 입력을 노출하지 않고, 공동의 연산 결과만을 계산할 수 있도록 하는 암호 기반 분산 계산 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 프라이버시 보장, 분산 신뢰 모델

&lt; 주요기술 &gt;
* Yao의 개릿 서킷 (Gabled Circuit), 시크릿 셰어링 (Secret Sharing), 동형암호, 소수정밀연산, 무지 전송 (Oblivious Transfer), 임계값 서명 (Threshold Signature), 블라인드 평가, 하이브리드 MPC

&lt; 활용 &gt;
* 개인정보보호, 비밀경매, 생체인증

&lt; 도구 &gt;
* MPyC, Sharemind

### [보안] CC (Common Criteria)

**[정의]**

서로 다른 국가 간에도 보안 평가 결과를 상호 인정받기위해, IT 보안 제품 및 시스템의 보안성 평가를 위한 국제 표준

**[핵심/키워드]**

&lt; 특징 &gt;
* 상호인증 (CCRA), 국제표준적용, 보안성 검증

&lt; 표준 &gt;
* ISO/IEC 15408, ISO/IEC 18045 (CEM)

&lt; 유효기간 &gt;
* 최초인증 (5년), 갱신인증 (연장 1회, 5년)

&lt; 평가내용 &gt;
* 기능 요구사항(SFR), 보증 요구사항(SAR)

&lt; 구성 &gt;
* 공통평가기준 (PP), 특정평가기준 (ST), 보안제품 (TOE), 평가등급 (EAL), 평가방법론 (CEM)

### [보안] OpenID Connect (OIDC)

**[정의]**

OAuth 2.0 기반으로 사용자 신원(ID) 확인 및 ID토큰을 활용하여 프로필 정보 제공 할 수 있는 사용자 인증(Authentication) 프로토콜

**[핵심/키워드]**

&lt; 특징 &gt;
* OAuth 확장 : 인증 정보를 포함한 ID Token 사용
* 사용자 정보 포함 : 로그인한 사용자 정보 확인 가능
* JWT 기반 : 경량 구조로 모바일/웹 모두 적합

&lt; 절차 &gt;
1\. RP (Client)는 OP (OpenID Provider) 요청
2\. OP는 최종사용자 인증, 권한 획득
3\. OP는 RP에 ID 토큰과 Access 토큰 응답
4\. RP는 UserInfo Endpoint에 정보 요청
5\. UserInfo Endpoint는 Claim (정보) 반환

&lt; 인증종류 &gt;
* 인증코드 흐름 (Authorization Code Flow), 암시적 흐름 (Implicit Flow), 하이브리드 흐름 (Hybrid Flow)

### [보안] 서비스형 랜섬웨어 (Ransomware as a Service, RaaS)

**[정의]**

전문 해커가 개발한 랜섬웨어 도구를 다른 범죄자에게 서비스 형태로 제공하고, 감염 수익을 공유하는 사이버 범죄 비즈니스 모델

**[핵심/키워드]**

&lt; 특징 &gt;
* 서비스 형태 제공, 운영자 (툴 제공), 사용자 (꽁격 실행)

&lt; 유형 &gt; 
* 구독형 (Rental), 수익 공유형 (Affiliate), 혼합형 

&lt; 사례 &gt; 
* 갠드크랩 (Gand Crab), - REvil (Sodinokibi), LockBit 

&lt; 대응방안 &gt; 
* 보안 정책 및 백업 체계 수립, 버그바운티 프로그램 운영, 랜섬웨어 대응 시나리오 및 대응계획 수립, 주기적인 백업 복구 테스트 및 모의훈련 수행, 사용자 권한 최소화 및 외부기기 제한, 보안 인식 교육 정기적 시행, 업무용 PC·노트북 보안 점검 및 통제, 방화벽, IDS/IPS, 보안관제체계 운영, 행위 기반 탐지 (EDR, SandBox 등), WAF 및 웹 보안관제 적용 (웹서비스 대응), SIEM(보안정보 이벤트 통합관리) 구축, 보안 개발 생명주기(Secure SDLC) 적용, 애플리케이션 화이트리스트 적용 (실행 통제), 백신(Anti-Virus) 및 최신 보안 패치 적용, 주기적 백업 및 백업 데이터 무결성 검증

### [보안] 정보보호제품 신속확인제도

**[정의]**

신기술 및 융·복합 정보보호 제품에 대해 최소한의 절차와 인증기준으로 보안 제품을 평가한 뒤 평가기준이 마련될 때까지 공공부문에 제품을 적용할 수 있도록 하는 제도

**[핵심/키워드]**

&lt; 특징 &gt;
* 신기술 및 융복합 제품, 최소 절차, 인증기준

&lt; 절차 &gt;
1\. 대상 검토 (기존제도 검토, 신속확인 준비)
2\. 신속 확인 (신청, 심의, 확인서 (유효기간 2년))
3\. 사후 관리 (변경승인, 연장, 이의신청, 기준관리)

&lt; 추가 &gt;
* 인증 및 평가기준 마련되면 더 이상 만료 이후 연장 불가

### [보안] 타이포스쿼팅 (Typosquatting)

**[정의]**

실제 도메인에서 일부 글자가 누락되거나, 순서가 바뀌는 등의 사용자 입력 실수(오타)로 가짜 도메인에 접속하여 공격하는 사회공학 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 흔한 입력실수 / 오타 이용, 2차 공격 가능, 탐지 및 피해 인지 어려움

&lt; 절차 &gt;
1\. 유사 도메인 접속 
2\. 악성코드 유포 및 실행 
3\. 악성코드 전파

&lt; 대응 &gt;
* 의심 열람 금지, 링크 실행 금지, 불법 SW 사용 금지, 주기적 백업, 실시간 검사, 최신 패치 업데이트

&lt; 유사 용어 &gt;
* URL 하이재킹, 스팅 사이트, 카운슬 도메인, 가짜 URL

### [보안] CBPR (Cross Border Privacy Rules, 국경 간 개인정보 보호 규칙)

**[정의]**

국경간 개인정보 이전 시 개인정보 보호를 보장하기 위해 APEC 회원국간 운영되는 개인정보 보호 인증제도

**[핵심/키워드]**

&lt; 특징 &gt;
* APEC, 자율인증, 상호국가 인증, 공통 프라이버시 기준, BCR 유사, 기업 중심 인증

&lt; 인증체계 &gt;
* 국내 정책, APEC, 인증기관, 인증위원회, 인증심사원

&lt; 인증절차 &gt;
1\. 준비 
2\. 심사 
3\. 인증 
4\. 유지관리

&lt; 인증기준 &gt;
* 개인정보 관리 체계수립 (2개), 개인정보 수집 (9개), 개인정보 이용, 위탁 제공 (7개), 정보주체 권리 (11개), 무결성 (5개), 보호 대책 (16개)

&lt; 연관 &gt;
* APEC Privacy Framework / APEC 원칙

### [보안] CWPP (Cloud Workload Protection Platform,워크로드보안)

**[정의]**

클라우드 환경에서 실행되는 워크로드에 대해 보안 가시성 확보, 위협탐지 및 보호기능을 제공하는 워크로드 전용 보안 플랫폼

**[핵심/키워드]**

&lt; 특징 &gt;
* 워크로드 기반, 에이전트 기반, DevSecOps 통합, 런타임 보호,

&lt; 보안영역 &gt;
* IaaS, PaaS

< 우선순위 모델 (가트너) >
* 운영 및 보안 위생 (Security Hygiene), 핵심, 중요, 옵션

< 우선순위 모델 / 주요기능 (가트너) >
* 운영 및 보안 위생 (보안 강화 (Hardening) 및 설정 / 취약점 관리, 네트워크 방화벽, 가시성 확보 및 마이크로 세그멘테이션,)
* 핵심 (시스템 무결성 보장, 애플리케이션 제어, 익스플로잇 예방 및 메모리 보호)
* 중요 (서버 워크로드 EDR, 행위 모니터링 및 위협 탐지·대응, 호스트 기반 침입 탐지 시스템)
* 옵션 (안티 멀웨어)

&lt; 구성요소 &gt;
* 에이전트, 취약점 분석기, 런타임 보호 모듈, 정책 제어/적용 엔진, 무결성 검사기, 관리자 콘솔

&lt; 주요방법 &gt;
* 마이크로 세분화, 베어메탈 하이퍼바이저

### [보안] HashDos

**[정의]**

클라이언트에서 전달되는 각종 파라미터 값을 관리하는 해시테이블의 인덱스 정보가 중복되도록 유도하여 기저장된 정보 조회 시 많은 자원을 소모하도록 유도하는 공격

**[핵심/키워드]**

&lt; 특징 &gt;
* 해시 테이블 인덱스 중복, cpu 소모, 해시 충돌

&lt; 공격절차 &gt;
1\. 매개변수 전달 
2\. 해시 테이블 충돌 
3\. 자원소모

&lt; 대응 &gt;
* POST 파라미터 제한, 메시지 크기 제한, HashDos 차단

### [보안] 전자봉투 (Electronic Envelope)

**[정의]**

데이터를 비밀키(대칭키, 세션키)로 암호화하고, 해당 비밀키를 수신자의 공개키로 암호화하여 안전하게 전달하는 하이브리드 암호화 방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 전자서명, 비대칭키(RSA), 비밀키, 수신자 공개키, 수신자 개인키

&lt; 송신 &gt;
1\. 메시지 및 해시 생성
2\. 전자서명 생성 (송신자 개인키)
3\. 원문 및 서명 암호화 (일회용 비밀키)
4\. 전자봉투 생성 (수신자 공개키)
5\. 전송

&lt; 수신 &gt;
6\. 전자봉투 복호화 (수신자 개인키)
7\. 원문 및 서명 복호화 (획득한 비밀키)
8\. 전자서명 검증 (송신자 공개키)

### [보안] 다중벡터공격 (Multi-Vector Attack)

**[정의]**

사이버 범죄자가 피싱, 악성코드, DDoS 등 다양한 공격 수단을 동시에 또는 연계하여 사용함으로써 조직 보안 시스템 침투 성공률을 높이는 공격방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 다양한 공격 경로, 탐지 회피, 복잡한 대응, 높은 성공 확률

&lt; 단계 &gt;
1\. 탐색 
2\. 공격실행 
3\. 은밀한 접근 
4\. 권한유지 
5\. 목표수행

&lt; 대응 &gt;
* 탐지/예방 (지능형 위협 차단, 예방 중심 보안)
* 관리/대응 (중앙 집중식 가시성 및 관리, 지동화된 인시던트)

### [보안] 양자내성암호 (Post-Quantum Cryptography, PQC)

**[정의]**

Shor/Grover 알고리즘이 효율적으로 해결할 수 없는 수학적 문제를 이용해 양자환경에서도 공개키 암호의 보안성을 유지할 수 있도록 설계된 암호방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 양자 내성, 새로운 수학 기반, 공개 키 대체 가능

&lt; 유형 &gt;
* 다변수, 코드, 격자, 아이소제니, 해시

&lt; 알고리즘 &gt;
* 다변수 (Rainbow, GeMSS), 코드 (McEliece, QC-MDPC, QC-MCPC), 격자 (Kyber, Dilithium, FrodoKEM, NTRU), 아이소제니 (SIDH, SIKE), 해시 (SPHINCS+, XMSS)

### [보안] 주스 재킹 (Juice Jacking)

**[정의]**

공공장소의 USB 충전기나 케이블에 악성 장치를 설치하여 개인 정보를 탈취하는 공격 수법

**[핵심/키워드]**

&lt; 특징 &gt;
* 전기 케이블 + 하이재킹

&lt; 공격절차 &gt;
1\. 악성 충전 장치 설치 
2\. 기기연결 유도 
3\. 기기 연결 및 악성코드 설치 
4\. 데이터 탈취
5\. 공격 종료 및 다음 공격 준비

&lt; 대응 &gt;
* 벽면 콘센트, 개인 충전 장비, 데이터 전송 차단, 의심스러운 동작 감시

&lt; 유사 &gt;
* 초이스 재킹 (사용자 승인 창 조작 + 하이재킹)

### [보안] 프롬프트 인젝션 (Prompt Injection)

**[정의]**

조작된 입력을 삽입하여 AI 시스템을 속여 의도된 행동에서 벗어나도록 조종하는 사이버 공격 기법

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

### [알고리즘] 카프-라빈 탐색

**[정의]**

해시 함수를 이용해 텍스트에서 패턴의 해시값과 같은 부분 문자열을 빠르게 탐색하는 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 빠른 후보 찾기, 롤링 해시 사용 (이전해시로 다음해시 계산), 대규모 문자열 탐색

&lt; 시간복잡도 &gt;
* N (텍스트 길이), M (패턴 길이)
* 평균 O (N+M), 최약 O (NxM)

&lt; 동작 &gt;
1\. 패턴 해시 계산
2\. 첫번째 문자열 계산
3\. 해시 비교
4\. 일치하면 문자열 비교
5\. 롤링 해시
6\. 3~5번 반복 및 종료

### [알고리즘] 힙 정렬 (Heap Sort)

**[정의]**

완전 이진트리 기반의 자료구조인 힙(Heap)을 이용하여 정렬하는 방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 완전 이진트리, 비교 기반, 제자리 정렬, 불안정 정렬

&lt; 복잡도 &gt;
* 최선 = 최악 = 평균 = O (n log n)

&lt; 유형 &gt;
* Max Heap, Min Heap

< 정렬과정 (Min Heap) >
1\. 최소힙 구성 
2\. 루트 삭제와 마지막 교환 
3\. 힙 크기 감소 및 재정비 
4\. 반복 및 정렬완료

### [알고리즘] Quad Tree

**[정의]**

2차원 공간을 4개의 사분면(quadrant)으로 재귀적 분할하여 표현하는 트리 기반 자료구조

**[핵심/키워드]**

&lt; 특징 &gt;
* 2차원 공간 분할, 4개 자식, 고속 탐색, 공간 효율성, 유연한 구조, 다양한 활용

&lt; 복잡도 &gt;
* 최악 O(n), 평균 O(log n)

&lt; 공간분할 매커니즘 &gt;
* 조건기반 분할, 적용형 구조

&lt; 유형 &gt;
* 영역 쿼드 트리 (Region), 점 쿼드 트리 (Point), 점-영역 쿼드 트리 (PR)

&lt; 절차 &gt;
1\. 영역확인 
2\. 분할조건 확인 (분할 불가능한 크기 확인) 
3\. 단말 노드 생성 
4\. 영역 분할 (재귀적)

### [알고리즘] 다익스트라 (Dijkstra) 알고리즘

**[정의]**

양의 가중치 방향 그래프에서 하나의 출발 정점으로부터 모든 정점까지의 최단 경로를 구하는 알고리즘

**[핵심/키워드]**

&lt; 내용 &gt;
* 최단경로, 그리디 알고리즘, 가중치 제약, 단일 출발점, 우선순위 큐 사용, 간선에 음수 포함 시 사용 불가

&lt; 시간복잡도&gt;
* V (정점), E (간선)
* 인접행렬 O (V^2), 우선순위 큐 O (E log V) or O (E + V log V)

&lt; 절차 &gt;
1\. 출발/종료 노드 설정 
2\. 테이블 초기화 
3\. 미방문 노드 중 가장 짧은 노드 방문 
4\. 최단거리 테이블 업데이트 
5\. 방문-업데이트 반복

### [알고리즘] 크루스칼 (Kruskal) 알고리즘

**[정의]**

그래프에서 간선을 가중치 오름차순으로 선택하여,사이클이 생기지 않도록 연결함으로써 최소 신장 트리를 구성하는알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
*최소신장, 간선 중심(선택 기준), 사이클 방지(조건), 그리디 알고리즘, 서로소 자료구조 (Find-Union 연산)

&lt; 시간복잡도 &gt;
* 최악 = 평균 = O (E log E)

&lt; 동작 &gt;
1\. 간선 정렬
2\. 초기화
3\. 간선 선택 및 연결
4\. 사이클 확인 후 반복

### [알고리즘] 그리디 알고리즘 (Greedy's Algorithm)

**[정의]**

특정 순간 최적해를 구하기 위해 최적성과 효율성 개선을 통해 최적의 해를 도출하는 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 근시안적, 현재 단계 최적

&lt; 성립조건 &gt;
* 탐욕 선택 속성(Greedy Choice Property), 최적 부분 구조(Optimal Substructure):

&lt; 단계 &gt;
1\. 문제 정의 및 최적 조건 확인
2\. 후보해 선택 (Selection)
3\. 적용 및 타당성 검사 (Feasibility Check) 
4\. 종료 조건 확인 및 반복 (Iteration)

&lt; 활용 &gt;
* 최소신장 (크루스칼, 프림), 최단경로 (다익스트라)

### [알고리즘] Red-Black Tree

**[정의]**

균형 유지를 위해 노드에 색상(레드 또는 블랙)을 추가하여 동작하는 자기 균형 이진 탐색 트리(Self-Balancing Binary Search Tree)

**[핵심/키워드]**

&lt; 특징 &gt;
* 자가 균형 이진트리

&lt; 복잡도 &gt;
* 항상 O (log N)

&lt; 규칙 &gt;
* 노드 색상 (Red, Black), 루트 노드 (Black), 리프 노드 (Black), Red 노드 자식은 Black, 모든 리프 노드 경로 높이 Black 수 동일

&lt; 균형 유지 &gt; 
* 색상 변경 (Recoloring), 회전 (Rotation)

< 동작 (삽입) >
1\. 노드 삽입
2\. 속성 위반 확인 (규칙 확인)
3\. 재조정 (색상변경, 회전)
4\. 반복

### [알고리즘] 프림 (Prim) 알고리즘

**[정의]**

하나의 정점에서 시작하여 인접한 간선 중 가장 가중치가 작은 간선을 선택해 전체 정점을 연결하는 방식의최소 신장 트리 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 최소신장, 정점(V) 중심, 그리디(탐욕) 알고리즘

&lt; 시간 복잡도 &gt;
* V (정점), E (간선)
* 인접행렬 O (V^2), 인접리스트+최소 힙 O (E log V) or O (E log E)

&lt; 동작 &gt;
1\. 시작 정점(V)선택 
2\. 인접 간선 탐색
3\. 최소비용 간선(E) 선택 
4\. 트리 추가 (정점 및 간선) 
5\. 반복

### [알고리즘] 동적계획법 (Dynamic Programming)

**[정의]**

복잡한 문제를 작은 부분 문제로 나누고, 그 결과를 저장하여 중복 계산을 피하는 최적화 알고리즘 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 부분 → 전체, 중복제거, 하위 문제 반복, 메모이제이션(Memoization) / 테이블화 (Tabulation)

&lt; 성립조건 &gt;
* 겹치는 하위 문제 (Overlapping Subproblems), 최적 부분 구조 (Optimal Substructure)

&lt; 구현방식 &gt;
* Top-down(재귀 +메모이제이션)
* Bottom-up (반복문 기반 테이블 채우기)

### [알고리즘] 연결 리스트 (Linked List)

**[정의]**

데이터를 저장하는 노드들이 포인터를 통해 순차적으로 연결된 선형 자료구조

**[핵심/키워드]**

&lt; 특징 &gt;
* 선형 자료구조, 포인터 (pointer) / 링크 (link), 동적확장, 빠른 삽입/삭제, 느린 탐색

&lt; 구성 &gt;
* 노드 (node), 헤드 (head), 테일 (tail), NULL

&lt; 유형 &gt;
* 단일 (Single), 이중 (Double), 원형 (Circular)

### [알고리즘] 분할정복 알고리즘 (Divide and Conquer)

**[정의]**

큰 문제를 작은 부분 문제로 나눈 뒤,각 부분을 독립적으로 해결하고,그 결과를 합쳐서 전체 문제를 해결하는 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 큰 문제 → 작은 부분 문제, 하위 문제 독립적

&lt; 원리 &gt;
* 분할 (Divide), 정복 (Conquer), 결합 (Combine)

### [알고리즘] KMP (Knuth-Morris-Pratt) 탐색

**[정의]**

패턴의 접두사-접미사 정보를 미리 계산한 실패함수(π배열)을 이용해, 불일치 시 비교를 되돌리지 않고 점프함으로써 선형 시간에 문자열을 탐색하는 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 실패 함수 (LPS 배열), 접두사 / 접미사 구조, 전처리 활용

&lt; 복잡도 &gt;
* N (텍스트 길이), M (패턴 길이)
* O (N + M)

&lt; 동작절차 &gt;
1\. 실패 테이블 생성 
2\. 텍스트 문자열 탐색
3\. 비교 시 일치면 포인터 이동
4\. 불일치 시 실패 함수 위치로 이동 후 탐색
5\. 반복

### [알고리즘] A* 알고리즘

**[정의]**

휴리스틱(heuristic) 이라는 추정치를 사용, 출발점에서 목표점까지 최단 경로를 찾는 그래프 탐색 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 휴리스틱, 최단경로, 최적성 + 속도

&lt; 함수 &gt;
* f(n) = g(n) + h(n)

&lt; 구성 &gt;
* 평가함수 (총 예상 비용 f(n), 실제 이동 비용 g(n), 목료 예상 비용 h(n))
* 탐색제어 (Open 리스트, Closed 리스트, 휴리스틱 함수)

&lt; 절차 &gt;
1\. 시작/종료 설정 
2\. 시작 Closed 추가 
3\. Open에서 최소 노드 선택 
4\. Closed 추가 
5\. 목표 확인
6\. 이웃 계산 
7\. Open 갱신 
8\. 반복

### [알고리즘] AVL (Adelson-Velsky and Landis) Tree

**[정의]**

모든 노드에서 왼쪽과 오른쪽 서브트리의 높이 차이(Balance Factor)가 1이하가 되도록 자동으로 균형을 맞추는 이진 탐색 트리(BST)의 확장 구조

**[핵심/키워드]**

&lt; 특징 &gt;
* 좌우 1 이하, balance factor, 자동 균형

&lt; 시간 복잡도 &gt; 
* 삽입 = 삭제 = 탐색 = O (log n)

&lt; 회전 연산 &gt;
* LL, LR, RL, RR

< 동작 (삽입) >
1\. 노드 삽입 
2\. 균형 확인
3\. 균형 깨진 경우 회전 균형 복구

### [알고리즘] 비선형 자료구조 (Non Linear Data Structure)

**[정의]**

데이터가 계층적 또는 복잡하게 연결되어 있는 구조로 하나의 요소가 여러 요소와 관계를 가질 수 있는 형태

**[핵심/키워드]**

&lt; 특징 &gt;
* 비선형, M : N, 다양한 관계 표현, 계층적 구조 가능

&lt; 유형 &gt;
* Tree, Graph

### [알고리즘] 솔린 (Soline) 알고리즘

**[정의]**

각 단계에서 모든 정점을 연결하는 포레스트(Forest)를 만들고 이를 연결하는 최소 신장 트리

**[핵심/키워드]**

&lt; 특징 &gt;
* 최소신장트리, 동시 간선 선택, 그리디 알고리즘, 정점 = 독립적 하나의 트리

&lt; 시간복잡도 &gt;
* V (정점), E (간선)
* O (E log V)

&lt; 동작 &gt;
1\. 초기화 (컴포넌트)
2\. 최소비용 간선 선택 (다른 트리 연결, 사이클 없음)
3\. 트리 병합 
4\. 반복 및 종료

### [알고리즘] 퀵정렬 (Quick Sort)

**[정의]**

기준 값(피봇) 을 중심으로 작은 요소는 왼쪽, 큰 요소는 오른쪽으로 분할(partition) 하여 재귀적으로 정렬을 수행하는 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* pivot 중심, 분할과 정복, 제자리 정렬


* 시간복잡도 : 최악 O (n^2), 평균 O (n log n)
* 공간복잡도 : O (log n)

&lt; Pivot 선택 방식 &gt; 
* 첫번째, 중간, 랜덤 선택

&lt; 절차 &gt;
1\. Pivot 선택
2\. 분할 (Partition)
3\. 정복 (Conquer) (재귀적)
4\. 종료

### [알고리즘] 백트래킹 (Backtracking)

**[정의]**

가능한 모든 경우를 탐색하면서 조건에 맞지 않으면 즉시 되돌아가는(가지치기) 방식의 완전 탐색 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 되돌아가기 (가지치기), DFS 방식

&lt; 주요원리 &gt;
* 가지치기 (상태공간트리, 유망성 검사, 가지치기 / 되돌아가기)

&lt; 동작 &gt;
1\. 결정 (Decision)
2\. 검사 (Check)
3\. 탐색 (Explore) : 재귀적 다음 탐색
4\. 되돌아가기 (backtracking) : 이전단계로

&lt; 활용 &gt;
* N-Queen 문제, 스도쿠(Sudoku) 풀이

### [알고리즘] 이진 트리 (BinaryTree)

**[정의]**

각 노드가 최대 두 개의 자식 노드 (왼쪽, 오른쪽)를 가지는 트리구조

**[핵심/키워드]**

&lt; 특징 &gt;
* 최대 자식 2개, 순서 있는 계층, 순회 방식 다양 (전위, 중위, 후위), 재귀적 구조

&lt; 시간 복잡도 &gt;
* 균형 O (log n), 불균형 O (n)

&lt; 유형 &gt;
* 포화 (Perfect) 이진트리, 완전 (Complete) 이진트리, 전 (Full) 이진트리, 편향 (Skew) 이진트리, 균형 (Balanced) 이진트리, 이진탐색 (Binary Search) 트리, 힙 (Heap) 트리

&lt; 순회 &gt;
* 전위 (Preorder, 루트, 왼쪽, 오른쪽), 중위 (Inorder, 왼쪽, 루트, 오른쪽), 후위 (Postorder, 왼쪽, 오른쪽, 루트), 레벨 (Level Order, 위에서 아래, 왼쪽에서 오른쪽)

< 동작 (삽입) >
1\. 탐색 : 루트노드부터 시작
2\. 값 비교 및 이동 : 작으면 왼족, 크면 오른쪽
3\. 빈공간 확인 : Null 확인
4\. 새노드 연결

&lt; 연관 &gt;
* 이진탐색트리, 힙트리

### [알고리즘] B-Tree

**[정의]**

데이터를 정렬된 상태로 저장하면서, 검색, 삽입, 삭제를 모두 빠르게 처리할 수 있도록 설계된 트리구조

**[핵심/키워드]**

&lt; 특징 &gt;
* M원트리, 다중 분기, 균형 유지, 정렬 유지, 빠른 탐색, 효율적 디스크 접근

&lt; 복잡도 &gt;
* 평균 = 최약 = O (log N)

&lt; 구성 &gt;
* 데이터 구성 (키, 데이터 포인터, 데이터)
* 트리 (트리 포인터, 루트 노드, 내부 노드, 리프 노드)
* 조건 (자식 수 제한, 키 수 제한, 루트 노드 조건, 트리 균형 조건)

&lt; 연산 &gt;
* 분할, 차용 / 재분배, 병합

< 동작 (삽입) >
1\. 삽입 위치 탐색 : 키 위치 탐색
2\. 삽입 : 리프노드 삽입
3\. 노드 분할 : 노드 초과 시 분할
4\. 반복 및 종료

&lt; 연관  &gt;
* B+ Tree, B* Tree

### [알고리즘] 삽입 정렬 (Insertion Sort)

**[정의]**

현재 값을 그보다 앞에 있는 정렬된 부분과 비교하여, 알맞은 위치에 삽입해가며 정렬하는 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 정렬된 앞쪽 비교, 구현 간단, 제자리 정렬, 안정 정렬

&lt; 복잡도 &gt;
* 최선 O (n), 최악 = 평균 O (n^2)

&lt; 동작 &gt;
1\. 두번째부터 시작
2\. 현재 요소 선택
3\. 위치 찾기 및 삽입: 앞쪽 정렬된 부분 확인
4\. 요소 이동 : 삽입 뒤쪽은 한 칸씩 이동
5\. 2~4 반복 및 종료

### [알고리즘] 보이어무어 탐색

**[정의]**

패턴의 오른쪽부터 왼쪽으로 비교하면서,불일치 발생 시 두 가지 규칙(Bad Character,Good Suffix)을 이용해 패턴을 한 번에 여러 칸 건너뛰는 고속 문자열 검색 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 문자열 탐색, 오른쪽에서 왼쪽으로 비교, 불일치 시 점프, skip_table (이동거리)

&lt; 주요규칙 &gt;
* 나쁜 문자 규칙 (Bad Character Rule), 좋은 접미사 규칙 (Good Suffix Rule) 

&lt; 복잡도 &gt;
* N (텍스트 길이), M (패턴 길이)
* 평균 O (N/M) or O (N), 최악 O (N x M)

### [알고리즘] 다차원 검색 트리

**[정의]**

2개 이상의 속성(차원)을 가진 데이터를 효율적으로 저장, 관리, 검색하기 위한 자료구조

**[핵심/키워드]**

&lt; 특징 &gt;
* 다차원 자료, 복수 키, 공간질의, Pivot (분할 및 기준점), 거리함수 (삼각부등식)

&lt; 유형 &gt; 
* PAM (Point, 점), SAM (Spartial, 공간)
* PAM : K-D tree, Quad tree, VP (조망점) tree, KDB tree
* SAM : R tree, R+ tree, R* tree, M-Tree (MBB, 최소경계구)

### [알고리즘] Bellman-Ford 알고리즘

**[정의]**

모든 간선을 최대 (정점 수 - 1)번 반복하며, 음수 가중치를 허용하는 단일 출발점 최단 경로 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 최단경로, 음수 가중치 허용(음수 간선 처리 가능), 음수 사이클 탐지 가능, 모든 간선 반복

&lt; 복잡도 &gt;
* V (정점), E (간선)
* O (V x E)

&lt; 동작 &gt;
1\. 초기화
2\. 간선 및 완화 업데이트 : 간선 거리 확인 후 업데이트
3\. 음수 사이클 확인 : 마지막 1회 추가(완화)

### [알고리즘] 배열 리스트 (Array List)

**[정의]**

인덱스를 이용해 요소에 빠르게 접근할 수 있으며, 크기를 자동으로 조절하는 기능을 가질 수 있는 배열을 기반으로구현된 선형 자료구조

**[핵심/키워드]**

&lt; 특징 &gt;
* 배열 + 리스트, 연속된 메모리 +자동 크기 확장, 순차 저장, 동적 크기, 내부적 배열 사용

&lt; 복잡도 &gt;
* 접근 O(1), 삽입/삭제 O(N) 

< 동작 (삽입) >
1\. 초기할당 : 초기 배열
2\. 빈공간 있으면 추가
3\. 용량 초과 시 새로운 배열 생성
4\. 새로운 배열에 기존 데이터 복사 및 데이터 추가
5\. 내부 배열 교체

### [알고리즘] 버블정렬 (Bubble Sort)

**[정의]**

인접한 두 개의 원소를 비교하여 서로 교환(swap)하는 방식을 반복적으로 수행하는 정렬 알고리즘

**[핵심/키워드]**

&lt; 특징 &gt;
* 인접 비교, 안정적, 제자리 정렬

&lt; 복잡도 &gt;
* 시간복잡도 : 최악 = 평균 = 최선 O(n²)
* 공간복잡도 : O(1)

&lt; 동작 &gt;
1\. 인접비교
2\. 위치 교환 (현재원소가 큰경우 (오름차순))
3\. 반복 (결과적 가장 큰 값이 마지막 위치)
4\. 다음 패스 (1~3 반복)
5\. 정렬 완료

### [알고리즘] 알고리즘 시간복잡도 (Time Complexity)

**[정의]**

입력 크기 n에 따라 알고리즘이 수행하는 연산 횟수로 알고리즘의 수행시간 평가하는 척도

**[핵심/키워드]**

&lt; 특징 &gt;
* 수행시간 평가, 컴파일+실행시간

&lt; 접근법 &gt; 
* 빅오, 오메가, 세타

&lt; 노테이션 사례 &gt; 
* O(1), O(log n), O(n), O(n log n), O(n²)

### [프로젝트 관리] 역량삼각형 (Talent Triangle)

**[정의]**

프로젝트 관리자에게 필요한 기술에 대해 3가지 측면에서의 역량 개발 프레임워크

**[핵심/키워드]**

&lt; 특징 &gt;
* 프로젝트 관리자의 핵심 역량

&lt; 3가지 역량 &gt;
* 기술적 프로젝트 관리 (Technical Project Management) 
→ 일하는 방식 (Ways of Working)
* 리더십 (Leadership) 
→ 파워스킬 (Power Skills)
* 전략 및 비즈니스 관리 (Strategy & Business Management)
→ 비즈니스 통찰력 (Business Acumen)

### [프로젝트 관리] 범위 관리

**[정의]**

프로젝트를 성공적으로 완료하기 위해 반드시 필요한 작업만을 빠짐없이 프로젝트에 포함시키기 위해 필요한 프로세스

**[핵심/키워드]**

&lt; 특징 &gt;
* 반드시 필요한 작업 포함

&lt; 프로세스 &gt;
* 계획단계 (범위계획, 요구사항수집, 범위정의, WBS 작성)
* 감시 및 통제 (범위확인, 범위통제)

&lt; 관련 표준 &gt;
* ISO/IEC 21500, ISO/IEC 21502

### [프로젝트 관리] 요구사항 명세서 (Software Requirement Specification, SRS)

**[정의]**

프로젝트의 목표, 기능, 성능, 제약 조건 등 소프트웨어가 충족해야 할 요구사항을 체계적으로 정리한 문서

**[핵심/키워드]**

&lt; 내용 &gt;
* 요구사항 체계적 정리 문서

&lt; 원칙 &gt; 
* 명확, 완전, 일관, 추적가능, 검증가능, 변경용이, 우선순위, 이해가능

&lt; 주요항목 &gt;
* 프로젝트 개요, 이해관계자 정의, 기능적 요구사항, 비기능적 요구사항, 시스템 인터페이스, 제약 조건, 변경 관리, 수락 기준

&lt; 추가 &gt;
* 요구사항 추적 매트릭스, IEEE 830, ISO/IEC/IEEE 29148, SW 진흥법 제44조

### [프로젝트 관리] 주공정경로법 (Critical Path Method, CPM)

**[정의]**

가장 오래 걸리는 경로를 찾아 프로젝트 최소 완료 시간을 계산하는 방법

**[핵심/키워드]**

< 주 공정/경로 >
* Critical Path, 가장 긴 경로

&lt; 용어 &gt;
* ES, EF, LS, LF, Total float, Free float, 선행, 후행, 전진계산, 후진계산

&lt; 절차 &gt;
1\. 개별활동 명시 및 순서 결정 
2\. 네트워크 다이어그램 작성 (PDM, ADM) 
3\. 주공정 계산 (전진, 후진) 
4\. 여유시간 계산 
5\. 주경로 분석 및 수행시간 산정

&lt; 한계 및 개선 &gt;
* 자원 제약 무시 → CCM (주공정연쇄법)

### [프로젝트 관리] 품질 비용(Quality Cost)

**[정의]**

제품이나 서비스의 품질을 확보하고 유지하거나, 품질 실패로 인한 손실을 측정하기 위한 비용

**[핵심/키워드]**

< 비용 유형 (COPQ) / 명시적 >
* 적합 (예방 (Prevention), 평가 (Appraisal))
* 부적합 (내부실패 (Internal Failure), 외부실패 (External Failure))

&lt; 잠재 비용 &gt;
* 잠재 실패 비용 (Hidden Failure Cost) : 기회비용, 이미지 손상, 사기 저하

### [프로젝트 관리] 터크만 사다리 모델 (Tuckman's Ladder Model)

**[정의]**

팀워크 성숙도를 높이기 위해 팀이 겪는 심리적·행동적 단계를 설명한 모델

**[핵심/키워드]**

&lt; 특징 &gt;
* 갈등은 팀워크 위한 필수과정, 단계별 순환 가능, 성숙도에 따라 리더쉽 변화 중요

&lt; 5 단계 &gt;
* 형성(Forming), 격동(Storming), 규범화(Norming), 성과(Performing), 해산(Adjourning)

### [프로젝트 관리] 현저성 모델 (Salience Model)

**[정의]**

이해관계자를 권력, 정당성, 긴급성에 따라 분류하고, 누구에게 우선적으로 대응할지를 판단하는 이해관계자 분석 기법

**[핵심/키워드]**

&lt; 3요소 &gt;
* 권력 (Power), 정당성 (Legitimacy), 긴급성 (Urgency)

&lt; 이해관계자 7가지 분류 &gt;
* 결정적 (Definitive, 권력 + 정당성 + 긴급성, 최우선), 
* 지배적 (Dominant, 권력 + 정당성), 위험적(Dangerous, 권력 + 긴급성), 의존적 (Dependent, 정당성 + 긴급성), , 잠자는 (Dormant, 권력), 임의 (Discretionary, 정당성), 요구 (Demanding. 긴급성)

&lt; 추가 집단 &gt;
* 비 이해관계자 (Non-Stakeholder) : 세가지 속성 전부 없음, 무관한 관리 대상

### [프로젝트 관리] 공정압축법 (Crashing)

**[정의]**

원가와 일정 관계를 분석하여 자원을 추가적으로 투입하여 기간을 단축하는 방법

**[핵심/키워드]**

&lt; 특징 &gt;
* 일정단축, 자원추가, 비용 상승, 리스크 증가 가능
* 새로운 주공정 확인 필요

### [프로젝트 관리] 매슬로우 욕구이론 (Maslow's Hierarchy of Needs Theory)

**[정의]**

하위 욕구가 충족되어야 상위 욕구가 활성화된다는 전제 하에 인간의 동기는 단계별 욕구가 위계적으로 충족되며 발생한다고 보는 심리학 이론

**[핵심/키워드]**

&lt; 특징 &gt;
* 동기부여 내용이론, 하위 욕구 만족 → 상위 욕구 가능, 위계적 

&lt; 단계 &gt;
* 기본 5단계 (생리,안전,소속,존중,자아실현)
* 6단계 (5단계 + 자기초월)
* 7단계 (생리, 안전, 소속, 존중, 인지, 심미, 자아실현)
* 8단계 (7단계 + 자기초월)

### [프로젝트 관리] 작업분해도 (Work Breakdown Structure, WBS)

**[정의]**

프로젝트 팀에서 실행할 전체 작업범위를 계층구조로 세분해 놓은 계통도

**[핵심/키워드]**

&lt; 내용 &gt;
* 작업 범위 계층구조, 작업 할당, 인도물(산출물) 중심

&lt; 구성 &gt;
* Work Package, Planning Package, Control Account, Decomposition, Code of Account, WBS Dictionary

&lt; 원칙 &gt;
* 100% rule, rolling wave, 8/80 rule

### [프로젝트 관리] 획득가치관리 (Earned Value Management, EVM)

**[정의]**

프로젝트의 범위, 일정, 자원 측정치를 모두 결합하여 프로젝트 성과 및 진척율을 평가하는 방법론

**[핵심/키워드]**

&lt; 특징 &gt;
* 범위, 일정,, 자원 측정치 결합, 성과 및 진척률

< 지표 / 분석 >
* 기본(계획 PV, 획득 EV, 실제 AC)
* 성과 (원가 CV, CPI, 일정 SV, SPI)
* 예측 (BAC, EAC, ETC, VAC, TCPI)

### [프로젝트 관리] 주공정연쇄법 (Critical Chain Method, CCM)

**[정의]**

프로젝트 일정의 불확실성에 대비하기 위해 버퍼를 두고 관리하는 일정 관리 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 자원 제약 고려, CPM 개선, 버퍼 사용

&lt; 버퍼 &gt;
* 프로젝트 버퍼, 피딩 버퍼, 자원 버퍼

### [프로젝트 관리] 책임배정매트릭스 (Responsibility Assigned Matrix, RAM)

**[정의]**

프로젝트 활동 또는 산출물에 대해 누가 어떤 역할과 책임을 가지는지를 명확히 표현한 표 형식 도구

**[핵심/키워드]**

&lt; 특징 &gt;
* 역할, 책임 표현

&lt; 역할 &gt;
* RACI (R ((Responsible, 실행 담당), A ((Accountable, 의사결정자), C ((Consulted, 자문), I (Informed, 보고대상자)

&lt; 원칙 &gt;
* 하나의 작업에는 하나의 A, 모든 작업에는 R/A, C/I는 반드시 필요하지는 않음, R/A와 C/I는 중복 가능

&lt; 개선 &gt;
* RACI-VS (Verifier, 검증자)
* RASCI (Support 지원)
* DACI (Driver, 주도자)

### [프로젝트 관리] ISO 31000

**[정의]**

조직의 모든 수준에서 위험을 식별, 평가, 관리하는 프레임워크를 제시한 위험관리에 대한 국제 표준

**[핵심/키워드]**

&lt; 특징 &gt;
* 국제 표준 가이드라인, 위험관리

&lt; 주요구성 &gt;
* 원칙 (Principles), 프레임워크 (Framework), 프로세스 (Process)
* 원칙 (가치 창출, 통합적 접근, 구조화, 맞춤화, 포함성, 동적 대응)
* 프레임워크 (리더십, 통합, 설계, 실행, 평가, 개선)
* 프로세스 (식별, 분석, 평가, 처리, 모니터링, 보고)

&lt; 국내 &gt;
* KS Q ISO 31000

### [프로젝트 관리] 기대이론 (Vroom's Expectancy Model )

**[정의]**

노력이 좋은 성과로 이어지고, 자신에게 가치 있는 보상을 가져올 것이라고 기대하는 동기부여 이론

**[핵심/키워드]**

&lt; 특징 &gt;
* 동기부여 과정이론, * 보상 가치 중요

&lt; 핵심 요소 &gt;
* 달성 가능성 (Expectancy, 기대감), 보상 가능성 (Instrumentality, 수단성), 보상의 가치 (Valence, 유의성)

&lt; 동기부여 &gt;
* 동기부여 = 기대감 x 수단성 x 유의성

### [프로젝트 관리] 고정가 계약 (Fixed-Price Contract)

**[정의]**

공급 받기로 한 제품, 서비스 및 결과물에 대한 고정가 총액을 설정하는 계약 방법

**[핵심/키워드]**

&lt; 특징 &gt;
* 고정 금액, 합의 금액

&lt; 계약유형 &gt;
* 확정 고정가 (FFP, 고정), 성과급 가산 고정가 (FPIF, 고정가+성과급), 가격조정 조건부 고정가 (FP-EPA, 고정가+변동반영)

### [프로젝트 관리] 권력 이해관계도 (Power / Interest Grid)

**[정의]**

권위 수준과 프로젝트 결과물에 관한 관심도 수준으로 그룹화하는 이해관계자 분석 방법

**[핵심/키워드]**

&lt; 특징 &gt;
* 권력 (Power), 관심도 (Interest)

&lt; 4분면 유형별 관리전략 &gt;
* 핵심 관리 대상 (높은 권력, 높은 관심), 영향력 유지 (높은 권력, 낮은 관심), 정보 제공 (낮은 권력, 높은 관심), 최소 노력 (낮은 권력, 낮은 관심)

&lt; 유사 &gt;
* 권력 이해관계도 + 태도 (Attitude) => 이해관계자 큐브 (3차원)

### [프로젝트 관리] 금전적 기대값 분석 (Expected Monetary Value Analysis, EMV)

**[정의]**

향후 발생할 지 여부를 알 수 없는 시나리오가 수반할 때 평균 결과값을 산출하는 통계적 기법

**[핵심/키워드]**

&lt; 특징 &gt;
* 불확실성 전제, 리스크중립 가정, 기회 (양수), 위협(음수)

&lt; 계산 방법 &gt;
* 발생확률 * 결과값

### [프로젝트 관리] 갈등관리 (Conflict Management)

**[정의]**

조직이나 팀 내에서 발생하는 의견 충돌, 이해관계 대립 등의 갈등을 인식하고 효과적으로 해결하거나 조정하는 활동

**[핵심/키워드]**

&lt; 원인 &gt;
* 일정우선, 희소자원, 개인스타일

&lt; 해결 &gt;
* 강요 (Force / Direct), 철회/회피 (Avoidance / Withdraw), 절충/타협 (Compromise / Recouncil), 협력/해결 (Collaboration / Problem Solve), 수용  (Accommodation / Smoothing)

### [프로젝트 관리] 리스크 대응 계획

**[정의]**

식별된 리스크에 대해 사전 대응 방안을 수립하고, 리스크 발생 시 영향을 최소화하기 위한 전략을 마련하는 과정

**[핵심/키워드]**

&lt; 특징 &gt;
* 위협 감소, 기회 극대화

&lt; 대응 전략 &gt;
* 공통 (에스컬레이션 (Escalation), 수용 (Accept))
* 기회 (활용 (Exploit), 공유 (Share), 강화 (Enhance))
* 위협 (회피 (Avoid), 전가 (Transfer), 완화 (Mitigate))
* 대응 이후 잔여리스크, 2차 리스크 관리

### [프로젝트 관리] 연동기획 (Rolling Wave Planning)

**[정의]**

가까운 시기에 완료할 작업은 상세히 계획, 장기적 작업은 개략적 계획하는방식

**[핵심/키워드]**

&lt; 특징 &gt;
* 점진적 상세화, 가까운건 상세히, 장기적인건 개략적

### [프로젝트 관리] 제안요청서 (Request for Proposal, RFP)

**[정의]**

발주자가 수행하고자 하는 사업이나 프로젝트에 대해 공급자(수행사)로부터 적절한 제안서를 받기 위해 요구사항을 명시한 문서

**[핵심/키워드]**

&lt; 특징 &gt;
* 보편성, 현실성, 구체성

&lt; 주요내용 &gt;
* 사업 개요, 범위 및 내용, 일정 및 예산 등

### [프로젝트 관리] 3점 산정 (Three-Point Estimating)

**[정의]**

불확실성과 리스크를 고려하여 활동 기간 산정치의 정확도를 개선할 수 있는 기법

**[핵심/키워드]**

&lt; 구성 &gt; 
* 최빈치 (Most Likely, M), 낙관치 (Optimistic, O), 비관치 (Pessimistic, P)

&lt; 분포 &gt;
* 삼각분포 (Triangular Distribution), 베타분포 (Beta Distribution / PERT 분포)

&lt; 공식 &gt;
* 삼각분포 (O + M + P) / 3, 베타분포 (O + 4M + P ) / 6

