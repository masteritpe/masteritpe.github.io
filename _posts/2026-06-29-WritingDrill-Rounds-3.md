---
layout: post
title: "WritingDrill_Rounds_3"
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

### [분야] 프로세스 제어블록 (Process Control Block, PCB)

**[정의]**

운영체제가 프로세스의 상태와 제어 정보를 저장하기 위한 데이터 구조
* Task Control Block

**[핵심/키워드]**

[ 특징 ]
* 프로세스 식별, 상태정보 저장소, 커널 공간, 문맥교환, 고유의 PCB
[ 구성 ] 아포상카레어입&lt;/font&gt;
* 프로세스 식별자 (PID), 프로세스 현상태, 프로세스 카운터 (PC), 레지스터 저장영역, 프로세스 스케줄링 정보, 계정정보, 입출력 상태정보, 메모리 관리정보, 포인터 (PCB 테이블 내 자신의 위치)
[ 활용 ]
* 문맥교환, 프로세스 상태관리, 프로세스 스케줄링

### [분야] 가트너 2026 10대 전략기술

**[정의]**

가트너에서 선정한, 향후 3~5년 사이 기업의 비즈니스 성장에 영향을 미치는 10가지 핵심기술들에 대한 보고서

**[핵심/키워드]**

[ 테마 ] 설융개&lt;/font&gt;
* 설계자 (Architect), 융합자 (Synthesist), 개척차 (Vanguard)
[ 전략기술 ]
* 설계자 (AI 네이티브 개발 플랫폼, AI 슈퍼 컴퓨팅 플랫폼, 컨피덴셜 컴퓨팅)
* 융합자 (다중 에이전트 시스템, 도메인특화 언어모델, 피지컬 AI)
* 개척자 (선제적 사이버보안, 디지털 출처, AI 보안 플랫폼, 지리적 이전)

### [분야] DRDoS (Distributed ReflectionDenial of Service)

**[정의]**

공격자가 &lt;u&gt;제3의 서버 (중계 서버)&lt;/u&gt;를 이용해 피해자에게 공격 트래픽을 전달하도록 유도하는 DDoS 변형 공격

**[핵심/키워드]**

[ 특징 ]
* 반사 (Reflection), 증폭 (Amplification), 정상서버 이용, 대귭모 증폭, 출처 은폐
[ 단계 ]
1) SYN 패킷 전송
2) IP 스푸핑
3) 반사 응답 발생
4) 대량 응답 트래픽
[ 반사서버 유형 ]
* DNS 서버, NTP 서버, SNMP 서버, CHARGEN 서비스, LDAP 서버
[ 대응 ]
* IP 스푸핑 방지, 반사서버 차단, 오픈서버 필터링, 이상탐지, Rate Limiting&lt;/font&gt;

### [분야] 문맥교환 (Context-Switching)

**[정의]**

실행 중인 프로세스 상태를 PCB에 보관하고 새로운 프로세스의 상태를 CPU에 적재하는 과정

**[핵심/키워드]**

[ 종류 ]
* 자발적 (실행-&gt;대기), 비자발적 (실행-&gt;준비)
[ 수행과장 ]
1) P1 실행  
2) 인터럽트 / 시스템 콜 
3) 문맥저장 (P1-&gt;PCB1) 
4) 문맥복원 (PCB2 -&gt; P2 / CPU) 
5) P2 실행 
6) 인터럽트 / 시스템 콜 
7) 문맥저장 (P2-&gt; PCB2) 
8) 문맥복원 (PCB1 -&gt; P1 / CPU) 
9) P1실행
[ 오버헤드 (문맥교환 단점) 해결방안 ]
* 원인 (상태 저장/복원 비용, TLB 무효화, 캐시 무효화, 스케줄링, 다중 프로그래밍)
* 문제점 (CPU 낭비, 성능 저하, 응답지연, 전력 소비 증가)
* 최소화 (타임슬라이스, 우선순위 스케줄링, 프로세스수 제한, I/O와 CPU 분리, 프로세서 바인딩, Working Set 기반 메모리 관리&lt;/font&gt;)
* 최소화 (스레드) (동일 프로세스 자원 공유, 문맥교환 비용 저렴, 스레드 풀 사용)

### [분야] 피지컬 AI (Physical AI)

**[정의]**

인공지능(AI)이 &lt;u&gt;물리적 환경에서 직접 동작&lt;/u&gt;하며, 감각, 학습, 행동을 수행하는 시스템
= 물리 AI

**[핵심/키워드]**

[ 특징 ]
* 3D 가상공간, 물리적 환경 실시간 학습 / 적응, 가상/현실 통합, 물리장치 연동
[ 기술 ] 센아액바&lt;/font&gt;
* 센싱 (카메라, Lidar, IoT 센서)
* 컴퓨터 비전 (온디바이스 비전 AI, 모델 경량화)
* 강화학습 (강화학습, RLHF, PPO)
* 자연어처리 (sLLM)
* 엣지 AI (온디바이스 AI, AI 전용 칩셋)
* 액츄에이션 (액츄에이션 제어, 동작 제어)
* 로보틱스 (SLAM, 고정밀지도)
* 통신 (5G / 6G, 초저지연 IoT NW)
* 개발 F/W (LWM, Tokenizer, 디지털트윈, 메타버스, AI 가속기)
* DB (Vector DB)
* 서비스 (자율주행, 휴머노이드 로봇)

### [분야] WPA3 (Wi-Fi Protected Access3)

**[정의]**

WPA2의 취약점을 보완, 더욱 강력한 보안성과 개인정보 보호를 제공하기 위해 Wi-Fi Alliance가 발표한 무선랜 보안 표준

**[핵심/키워드]**

[ 특징 ]
* SAE 도입&lt;/font&gt; (딕셔너리 차단), GCMP &lt;/font&gt;(고속 암호화), PMF 필수 (프레임 보호), Forward Secrecy (세션 노출 방어)
[ 동작절차 ]
1) SAE로 사용자 인증 (PSK 대체)
2) PMK 생성
3) 4-way handshaking (PTK, GTK)
4) GCMP 통해 암호 / 무결성 검증
5) 관리 프레임은 별도 PMF로 보호
[ 구성요소 ]
* SAE (PSK 대체, ECC기반 키 교환), AES-GCMP (AES + HMAC), PMK, PTK, GTK, PMF

### [분야] 인터럽트(Interrupt)

**[정의]**

CPU가 처리하던 프로그램을 중단하고 컴퓨터 제어를 특수 사건이나 환경을 처리할 수 있도록 보내는 &lt;u&gt;제어신호&lt;/u&gt;

**[핵심/키워드]**

[ 특징 ]
* 우선순위처리, 비동기처리, 문맥교환
[ 구성 ]
1) 요청 (IRQ) 
2) 처리루틴 (IPR / Vector) 
3) 서비스루틴 (ISR)
[ 우선순위 / 종류 ] 전기외입프S
&lt;/font&gt;* 외부 (전원이상 &gt; 기계이상 &gt; 외부신호 &gt; 입출력신호) &gt; 내부 (프로그램검사 / 트랩) &gt; 소프트웨어 (SVC)
[ 처리방식 ]
* 처리 주체 (Polling, 인터럽트기반)
* 진입방식 / 처리방식 (비벡터 인터럽트, 벡터 인터럽트)
* 연결구조 / 하드웨어 (직렬 (Daisy Chain), 병렬 (Multiple))
* 우선순위 / 중첩 (단일, 인터럽트, 중첩 인터럽트)
* 발생방식 (하드웨어, 소프트웨어)
[ 하드웨어 연결기준 ] 다대폴&lt;/font&gt;
* 단일회선 ((직렬)daisy chain, polling), 다중회선 ((병렬) multiple)
[ 중첩인터럽트 처리 ]
* Pending, 우선순위

### [분야] 디지털 면역 시스템 (Digital Immune System)

**[정의]**

시스템, 네트워크, 장치를 &lt;u&gt;사이버 위협 및 공격으로부터 보호&lt;/u&gt;하도록 설계된 SW 또는 시스템

**[핵심/키워드]**

[ 특징 ]
* 사이버 위협 / 공격으로부터 보호, 서비스 복원력 최적화
[ 6가지 요소 ]
1) 관찰 가능성
2) AI 증강 테스트
3) 카오스 엔지니어링
4) 자동복구
5) 시스템 신뢰성 엔지니어링 (SRE)
6) App 공급망 보안

### [분야] SQL 인젝션 (SQL Injection)

**[정의]**

사용자 입력값이 SQL 쿼리에 삽입되어 데이터베이스 명령이 조작되는 보안 취약점

**[핵심/키워드]**

[ 특징 ]
* 명령 조작, 쿼리 조작, 인증 우회, 정보탈취
[ 유형 ]
* Classic SQL Injection, Blind SQL Injection, Error Based SQL Injection, Union Based SQL Injection&lt;/font&gt;
[ 대응 ]
* Prepared Statement, Prepared Query, 입력값 검증, 최소 권한 원칙, DB 오류 메시지 숨김, White-list Filtering&lt;/font&gt;

### [분야] 최단 잔여시간 우선 (Shortest Remaining First, SRT) 스케쥴링

**[정의]**

&lt;u&gt;남은 실행시간이 가장 짧은&lt;/u&gt; 프로세스를 우선 선택하는 &lt;u&gt;선점형&lt;/u&gt; CPU 스케줄링 방식
* Shortest Remaining First Time, SRTF

**[핵심/키워드]**

[ 특징 ]
* 선점형, 남은 실행시간 예측, 짧은 작업 유리, 기아현상, 문맥교환 발생 가능
[ 스케쥴링 기준 ]
* 처리능력 최대화, 반환시간, 대기시간, 응답시간 최소화

### [분야] 가트너 2025 AI 하이프 사이클 (Hype Cycle)

**[정의]**

인공지능 관련 신기술의 현재 시장내 위치와 성숙 경로를 5단계로 시각화한 기술 수명주기 모델

**[핵심/키워드]**

[ 특징 ]
* 인공지능 중심 지속가능 기술

[ 주요 분야 ]
* AI Agent, AI Ready Data, 멀티모달 AI, AI TRiSM

### [분야] SSRF (Server-Side Request Forgery)

**[정의]**

공격자가 서버측에서 실행되는 요청 기능을 조작하여, 서버가 내부 또는 외부 자원에 요청을 보내도록 유도하는 공격

**[핵심/키워드]**

[ 특징 ]
* 서버측 요청 기능 조작, 서버가 프록시 동작, 탐지 어려움, 메타 데이터 접근 가능, 보안 장비 우회 가능
[ 절차 ]
1) 조작된 요청 생성 (Attacker)
2) 방화벽 우회 (Firewall)
3) 취약한 웹 사이트가 요청 실행 (Web site)
4) 내부 서버 접근 (Internal Server)
5) 정보 유출 (Data leak)
[ 대응방안 ]
* 입력값 검사 (Whitelist Filtering, Blacklist Filtering)
* OS / NW (ACL, 최소권한, 망분리 등)
* 접속기록 / 모니터링 (이상 / 오용 / 행위 탐지, 로그기록 탐지, 내부 IP 접근 차단)

### [분야] 최단 작업 우선 (Shortest Job / Process First, SJF / SPF) 스케줄링

**[정의]**

예상 실행시간이 가장 짧은 작업을 먼저 실행하는 비선점 스케줄링 방식

**[핵심/키워드]**

[ 특징 ]
* 비선점, 짧은 실행시간 유리, 기아현상 발생 가능

[ 스케쥴링 기준 ]
* 처리능력 최대화, 반환시간, 대기시간, 응답시간 최소화

### [분야] AI 워싱 (Washing)

**[정의]**

AI기술을 &lt;u&gt;실제보다 과장하거나 존재하지 않는데도 적용된 것처럼&lt;/u&gt; 표시·광고하는 행위

**[핵심/키워드]**

[ 발생원인 ]
* AI 열풍, 정보 비대칭, 투자유치 경쟁, 규제 공백
[ 주요유형 ]
* 허위표시형, 과장표시형, 모호표시형&lt;/font&gt;
[ 규제동향 ]
* 미국 (과징금, 제제), EU (EU AI Act, 소비자법), 한국 (공정위 중심 점검)&lt;/font&gt;
[ 대응방안 ]
* 법적규제 근거, 에방 가이드라인 배포, 투명성 및 신뢰성 강화

### [분야] 보안 소프트웨어 생명주기 (SECURE SDLC)

**[정의]**

안전한 소프트웨어를 개발하기 위해 SDLC 상에서 보안을 강화한 개발 프로세스

**[핵심/키워드]**

[ 특징 ]
* 보안성 + SDLC 
[ 단계 ]
* SDLC 단계에 보안활동 포함
* 보안 요구사항, 보안설계, 보안개발, 보안 테스트, 보안유지보수 등
[ 방법론 ]
* MS SDL&lt;/font&gt; (Pre SDL, Post SDL, 위협 모델링)
* Secure SW CLASP&lt;/font&gt; (검증 중심, 애플리케이션 보안 문제 명시)
* Seven TouchPoint&lt;/font&gt; (7가지 중점 관리 대상)
* BSIMM (성숙도 수준)
* OPEN SAMM (점진적 확대, 개방원칙)

### [분야] 세마포어 (Semaphore)

**[정의]**

다중 프로세스 환경에서 공유 자원에 대한 접근을 제어하기 위해 P, V 연산을 활용해서 사용되는 정수기반 동기화 도구

**[핵심/키워드]**

[ 자원 대기 방식 ]
* Busy wait, Sleep Queue
[ 자료구조 ]
* S (정수 변수, 요청 시 -, 해제 시 +), Qs (대기 큐)
[ 매커니즘 ]
1) 초기화 
2) P 연산 (Wait)
3) V 연산 (Signal)&lt;/font&gt;
[ 유형 ]
* Binary Semaphore (상호배제)
* Counting Semaphore (자원관리)
[ 단점 ]
* 문맥교환, 타이밍 문제 발생 가능

### [분야] 비지상망 (Non-Terrestrial Network, NTN)

**[정의]**

위성·고고도 플랫폼·드론 등 지상 기지국이 아닌 &lt;u&gt;비지상 인프라를 활용하여&lt;/u&gt; 통신 서비스를 제공하는 네트워크

**[핵심/키워드]**

[ 특징 ]
* 광역 커버리지, 재난복구, 6G 핵심기술, UAM, 위성통신
[ 등장배경 ]
* 커버리지 한계, 보편적 커버리지 확보
[ 구성요소 ]
* 위성 (Satellite), 고고도플래폼 (HAPS), UAV / 드론&lt;/font&gt;
[ 기술 ]
* 위성통신 (Feeder, iSL), 빔포밍, MIMO, Doppler, 하이브리드 연동, Ka밴드, Ku밴드, mmWAVE&lt;/font&gt;
[ 적용분야 ]
* 해양, 군사, 재난안전, 자율주행, 드론, LBS

### [분야] 사회공학 (Social Engineering)

**[정의]**

인간 상호작용의 깊은 &lt;u&gt;신뢰를 바탕으로&lt;/u&gt; 사람들을 속여, 정상 보안 절차를 깨뜨리고 비기술적인 수단으로 정보를 얻는 행위

**[핵심/키워드]**

[ 특징 ]
* 상호작용, 신뢰바탕, 심리, 실수 활용, 피해 인지 어려움, 보안 우회 가능, 쉬운 연계 공격
[ 절차 ]
1) 정보수집 (Information Gathering)
2) 관계형성 (Developing Relationship)
3) 공격 (Exploitation)
4) 실행 (Execution)&lt;/font&gt;
[ 공격유형 ]
* 인간기반 (직접접근, 도청, 훔쳐보기, 휴지통 뒤지기, 프리텍스팅 (Pretexting), 퀴드 프로 쿼 (Quid pro quo), 비싱 (Vishing), 페이퍼 피싱)
* 컴퓨터기반 (Phishing, Smishing, Pharming, Malware, 포렌식 악용)
* 물리적 (Baiting, USB Drop)&lt;/font&gt;
[ 대응 ]
* 인간기반 (교육, 출입통제, 비인가 절차 강화, 감시 및 신고)
* 컴퓨터기반 (URL 필터링, 탐지 솔루션, MFA, 브라우저 보안 강화, DNSSEC)
* 물리적 (외부 저장장치 통제, 문서 폐기 절차, 감시장비 설치, 반출입 관리)&lt;/font&gt;

### [분야] 뮤텍스 (Mutex)

**[정의]**

&lt;u&gt;하나의 쓰레드 또는 프로세스만&lt;/u&gt; 임계영역에 진입할 수 있도록 상호배제를 보장하는 락객체

**[핵심/키워드]**

[ 특징 ]
* 소유권(Owner), 블록킹(Blocking)
[ 자료구조 ]
* 상태변수 (Locked, Unlocked), 대기 큐
[ 매커니즘 ]
1) 초기화
2) lock()
3) unlock()&lt;/font&gt;

### [분야] 저궤도 위성 통신 (LEO Satelite Communication)

**[정의]**

지상 약 500~2,000km 고도에서 운용되는 &lt;u&gt;저궤도 위성&lt;/u&gt;을 활용한 통신방식

**[핵심/키워드]**

[ 특징 ]
* 저궤도, 초저지연, 다수 위성 군집 기반
[ 구성요소 ]
* 위성 (ISL, OBP Payload, Beamforming, Feeder Link)
* 사용자 (사용자 단말, Spot Beam, Wide Beam)
* 지상 (Feeder Link, Gateway, Baseband Router, Core Network, NMC)&lt;/font&gt;
[ 주요 사례 ]
* Starlink, OneWeb, Kuiper, 누리호

### [분야] 피싱 (Phishing)

**[정의]**

공격자가 신뢰할 수 있는 기관이나 사람으로 위장, 이메일, 웹사이트, 메시지 등을 통해 &lt;u&gt;사용자를 속이고&lt;/u&gt; 민감한 정보를 입력하게 유도하는 사회공학 공격기법

**[핵심/키워드]**

[ 특징 ]
* 사회공학기반, 비기술적 활용, 낮은 공격 난이도, 지속적 진화 / 변형)
[ 공격 절차 ]
1) 이메일 등 발송
2) 위장사이트 개인정보 입력
3) 입력정보 탈취 및 악용
[ 유형 ]
* Spear phishing (특정 대상)
* Whaling / Whale phishing (고위 인사)
* Smishing (문자 메시지, 소액결제)
* Vishing / Voice phishing (음성, 전화)
* Qshing (QR)
* Pharming (DNS, Host 조작)&lt;/font&gt;
[ 대응방안 ]
* 출처확인, 교육강화, 필터링 / 차단, 신뢰 인증 강화, MFA, 보안솔루션, HTTPS&lt;/font&gt;

### [분야] 우선순위역전 (Priority Inversion)

**[정의]**

우선순위가 높은 타스크가 READY상태로 바뀌었지만, &lt;u&gt;더 낮은 우선순위 타스크가 CPU를 점유하고 있어 실행되지 못하는&lt;/u&gt; 상태

**[핵심/키워드]**

[ 발생원인 ]
* 공유자원 사용, 선점형 스케줄링, 중간 우서순위 태스크의 개입
[ 문제점 ]
* 우선순위 정책 왜곡, 기아상태, 실시간성 보장 실패, 디버깅 어려움, 성능저하
[ 동작절차 ]
1) T3 자원획득 
2) T1 실행 
3) T1 자원 요청 (대기) 
4) T3 실행 &gt; T2 실행 
5) 우선순위 역전 
6) T2 종료 / T3 실행 
7) T3 자원반환 
8) T1 실행&lt;/font&gt;
[ 해결방안 ]
* 우선순위 상속 (Priority Inheritance)
* 우선순위 올림 (Priority Celling
* 랜덤 부스팅 (Random Boosting)
* 인터럽트 금지, Lock-Free, Messaging Passing&lt;/font&gt;

### [분야] 울트라 이더넷 (Ultra Ethernet)

**[정의]**

GPU간 대규모 병렬 연산과 AI 학습/추론 성능 극대화를 목표로 하는 개방형 네트워크 기술

**[핵심/키워드]**

[ 특징 ]
* 대규모 병렬 연산, 초저지연, 고대역폭, 벤더 종속 탈피, AI / HPC 최적화&lt;/font&gt;
[ 네트워크 ]
* Frontend N/W, Backend Scale-out N/W, Scale-Up N/W
[ 계층 ]
* Software, Transport, Network, Link, Physical
[ 기술 ]
* Software (libfabric mapping, Semantic)
* Transport (PDS, CMS, TSS)
* Network (Packet Trimming)
* Link (LLR, CBFC, UE Link)
* Physical (Channel Quality, FEC Statistics)

### [분야] 파밍 (Pharming)

**[정의]**

정상적인 웹사이트에 접속한 것처럼 보이지만, 실제로는 악성 DNS 조작 등을 통해 공격자가 만든 &lt;u&gt;가짜 사이트로 유도하여&lt;/u&gt; 개인정보를 탈취하는 공격

**[핵심/키워드]**

[ 특징 ]
* 도메인, Host, DNS 변조, 탐지 어려움
[ 공격 ]
1) 가짜 사이트 설치
2) DNS 해킹 / 변조
3) IP 조회 및 제공 / 가짜 사이트 접속
4) 개인정보 등 데이터 유출 및 악용
[ 공격유형 ]
* DNS 서버 파밍, Hosts 파일 조작, 악성코드 기반 파밍, 웹 프록시 파밍&lt;/font&gt;
[ 대응방안 ]
* DNSSEC, DoT, DoH, Hosts 파일 보호, 악성코드 차단, 보안 인식 교육&lt;/font&gt;

### [분야] IPC (Inter Process Communication)

**[정의]**

프로세스들 사이에 서로 데이터를 주고 받는 행위 또는 그에 대한 방법이나 동기화 방법

**[핵심/키워드]**

[ 목적 ]
* 동기화, 직접 데이터 공유 불가 해결, 데이터 전달, 자원 공유
[ 종류 ]
* 파일 기반 (File, FIFO, Pipe, Named Pipe)
* 메모리 기반 (Shared Memory, Memory Queue, Memory Map)
* 네트워크 기반 (RPC, Socket)
* 동기화 전용 (Semaphore)&lt;/font&gt;

### [분야] 와이파이8 (Wi-Fi 8, IEEE 802.11bn)

**[정의]**

AI 기반 지능형 네트워크 제어와 &lt;u&gt;초고신뢰 (UHR)&lt;/u&gt;를 구현하는 차세대 무선 LAN 기술

**[핵심/키워드]**

[ 특징 ]
* 초고신뢰 (UHR), 다수 AP 협업, 스마트 전력, AI 기반 지능형 제어
[ 주요기능 ]
* Cross Layer (DSO (동적 서브채널 할당), NPCA (주 체널 외 전송))
* MAC Layer (MPCA (보조채널 전송), ELA (MCS 자동조정))
* PHY Layer (DRU (대역확산), ELR (장거리), UEQM (스트림별 변조), DBE (동적 채널폭))&lt;/font&gt;
[ 협력기능 ]
* CO-SR (동적 전력), CO-BF (협력 방향조정)

### [분야] 랜섬웨어 (Ransomware)

**[정의]**

컴퓨터에 저장된 파일들을 암호화하여 사용자가 읽을 수 없는 문자들로 바꿔버린 후, 암호화를 풀어주는 &lt;u&gt;대가로 금전을 요구하는&lt;/u&gt; 악성 프로그램

**[핵심/키워드]**

[ 특징 ]
* 특정 타겟, 비표적 등 다양, 금전 요구 
[ 공격방식 ]
* 암호화, 비암호화 
[ 공격 ]
1) 초기 침투 / 감염
2) 악성코드 실행
3) 파일 암호화
4) 금전 요구
5) 이중 협박
6) 금전 지급
7) 후속 공격&lt;/font&gt;
[ 주요 공격 ]
* 페트야, 낫페트야, 배드래빗, 갠드크랩, 콘티
[ 최근 공격 동향 ]
* 지능형, RaaS, RansomWeb, 랜섬웨어 다중탈취 등으로 진화
[ 대응방안 ]
* 관리적 (보안정책, 백업정책 강화, 버그바운티, 주기적 모의훈련, 보안인식 교육)
* 기술적 (보안솔루션, EDR, 이상탐지, SIEM, 빅신, 최신 패치)&lt;/font&gt;
[ 추가대응 ]
* KISA 백업가이드라인, 랜섬웨어 대응가이드

### [분야] 교착상태 (Deadlock)

**[정의]**

두개 이상의 프로세스가 서로 상대방의 자원을 요구하면서 양쪽 모두 작업 수행을 할 수 없는 대기 상태

**[핵심/키워드]**

[ 발샐조건 ]
* 상호배재 (Mutual Exclusive), 점유와 대기 (Block and Wait), 비선점 (Non preemption), 환경대기 (Curcular wait)&lt;/font&gt;
[ 해결방안 ]
* 예방 (Prevention)
* 회피 (Avoidance, Banker's, Wait-Die, Wound-Wait) 
* 발견 (Detection, 자원할당 그래프, 대기 그래프) 
* 회복 (Recovery) 
* 무시(Ignore)&lt;/font&gt;

### [분야] 소캠 메모리 (Small Outline Compression Attached Memory Module, SOCAMM)

**[정의]**

저전력 D램인 LPDDR을 집적해 전력 효율성을 높이고, 기존 온보드 방식과 달리 &lt;u&gt;메모리를 탈부착할 수 있는 &lt;/u&gt;메모리 모듈

**[핵심/키워드]**

[ 특징 ]
* LPDDR 활용, 범용성, 저전력, 탈부착 형식 모듈&lt;/font&gt;
[ 사양 (SOCAMM 기준) ]
* 기반 메모리 (LPDDR)
* 속도 (9,600 MT/s)
* I/O (694개)
* 표준화 (JEDEC, 범용적)
* 용량 (192GB 모듈)
* 저전력 (매우 향상된 저전력)
* 공급업체 (삼성, 하이닉스, 마이크론 등 다양)
[ SOCAMM 2 개선 ]
* 속도 향상, 용량 증가, 공급업체 다양화, 범용적 표준화, SPD 지원

### [분야] 서비스형 랜섬웨어 (Ransomware as a Service, RaaS)

**[정의]**

전문 해커가 개발한 랜섬웨어 도구를 다른 범죄자에게 &lt;u&gt;서비스 형태로 제공&lt;/u&gt;, 감염 수익을 공유하는 사이버 범죄 비즈니스 모델

**[핵심/키워드]**

[ 특징 ]
* 범죄자 서비스 형태 제공, 수익 공유, 익명성, 비기술자 사용
[ 운영방식 ]
* 구독형 (Rental), 수익공유 (Affiliate), 혼합&lt;/font&gt;
[ 사례 ]
* 갠드크랩, REvil, LockBit, BlackCat
[ 구성 ]
* 개발자, 유포자
[ 대응방안 ]
* 유포 채널 차단, 모니터링, 위협 인텔리전스 공유 강화&lt;/font&gt;

### [분야] CPU 파이프라이닝 (Pipelining)

**[정의]**

명령어 실행을 &lt;u&gt;여러 단계로 분리&lt;/u&gt;, 각 단계를 &lt;u&gt;동시에 중첩 수행하여&lt;/u&gt; CPU 처리성능을 향상시키는 병렬처리 기법

**[핵심/키워드]**

[ 특징 ]
* 여러 단계 분리, 명령어 병렬처리, 처리율 증가, CPI 감소, 중첩 실행, Hazard 발생
[ 수행단계 (4단계 기준) ]
1) Fetch (인출) 
2) Decode (해독) 
3) Execute (실행) 
4) Write back (결과 실행)&lt;/font&gt;
[ 종류 ]
* 단일파이프라인 (Pipeline, 단계별 한 번씩 중첩) 
* 슈퍼 파이프라인 (Super pipeline, 엇갈리게 중첩)
* 슈퍼 스칼라 (Super scalar, 동시실행 중첩)
* 슈퍼 파이프라인드 슈퍼 스칼라 (Super pipelined Super scalar)
* VLIW (Very Long Instruction Word, 실행 여러 개 하나로)&lt;/font&gt;
[ 성능 측정 기준 ]
* 속도 향상 (K x N) / K + (N-1) (K 단계 수, N 명령어 수)
* 처리율, CPI, 지연시간, 효율

[ 문제점 ]
* 해저드 발생 가능 (구조적, 데이터, 제어)

### [분야] PIM (Processing In Memory)

**[정의]**

하나의 칩 내부에 &lt;u&gt;메모리와 프로세서 연산기를 집적한&lt;/u&gt; 차세대 반도체

**[핵심/키워드]**

[ 특징 ]
* 폰 노이만 개선, 메모리 병목 개선, 메모리 내부 연산 처리
[ 유형 ]
* 연산장치 (PIM (메모리 내부), PNM (따로 구현, Die 연결), In-Memory PIM (뒤섞임)
* 연산방식 (Analog PIM (전하, 전류), Digital PIM (ALU, 디지털 로직)
* 메모리 소자 (SRAM PIM, DRAM PIM, ReRAM PIM)&lt;/font&gt;

### [분야] BYOVD (Bring Your Own Vulnerable Driver) 공격

**[정의]**

&lt;u&gt;취약점이 있는 서명된 드라이버를&lt;/u&gt; 시스템에 설치해 이를 악용하여 커널 권한 획득, 보안 우회, 루트킷 설치 등을 수행하는 공격기법
*  EDR Killer

**[핵심/키워드]**

[ 특징 ]
* 합법적 서명, Rootkit, 커널 권한 획득, 서명된 취약한 드라이버
[ 공격 ]
1) Initial Access
2) Privilege Escalation
3) Vulnerble Driver Installation
4) Modify Kernel Structures
5) Disabled Security Controls&lt;/font&gt;
[ 대응방안 ]
* 취약한 드라이버 차단, 최신 보안 업데이트, 최신 드라이버 설치, 지속적 모니터링, 최소권한&lt;/font&gt;

### [분야] 파이프라인 해저드 (Pipeline Hazard)

**[정의]**

파이프라인에서 명령어들이 겹쳐 실행될 때 충돌이나 지연이 발생하여 CPI가 1이 되는 것을 방해하는 현상

**[핵심/키워드]**

[ 특징 ]
* 파이프라인 성능 저해, CPI 1 방해
[ 유형 ]
* 구조적 (Structural, 자원부족, 폰노이만 구조)
* 데이터 (Data, 데이터 의존성, RAW, WAR, WAW)
* 제어 (Control, 분기, 제어)&lt;/font&gt;
[ 해결 ]
* 공통 (Stall, Bubble)
* 구조적 (자원확충, 하버드 아키텍처)
* 데이터 (Change Clock Cycle, Forwarding, Bypassing, 비순차 실행, Renaming, NOP 삽입, 코드 재배치)
* 제어 (분기예측, 지연분기, 추측실행)&lt;/font&gt;

### [분야] UCIe 3.0 (Universal Chiplet Interconnect Express 3.0)

**[정의]**

칩렛간 통신 속도를 비약적으로 높이고, 복잡한 멀티-칩 시스템을 위한 관리 및 테스트 기능을 강화한 차세대 &lt;u&gt;개방형 칩렛 상호연결 표준 버전&lt;/u&gt; 3

**[핵심/키워드]**

[ 특징 ]
* 개방형, 이기종 칩 통합, PCIe / CXL 지원
[ Layer ]
* Protocol Layer, Adapter Layer, Physical Layer
[ 구성 ]
* Protocol (PCIe, CXL, Streaming)
* Adapter (Packetization, ECC / CRC, Retry &amp; Flow, Flit Negotiation)
* Physical (Die to Die, Short / Ultra Short Reach Link)&lt;/font&gt;
[ UCIe 3.0 ]
* 링크 최적화, 사이드채널 확장, 긴급 셧다운 관리
[ UCIe 3.0 주요기술 ]
* 성능 및 전력 효율 (속도 향상, 런타임 재보정, L2 유휴 최적화)
* 시스템 관리 (우선순위 측대역, 고속 스로틀링 및 긴급종료, MTP)
* 설계 유연성 (확장된 측대역 거리, CTP, Raw Mode, 고신뢰 인코딩)

### [분야] XZ-Utils 백도어 취약점

**[정의]**

사회공학적 기법을 사용, &lt;u&gt;장기간 오픈소스 저장소 기여 및 관리자 권한을 합법적으로 양도받은 후&lt;/u&gt; 백도어가 포함된 버전을 배포한 취약점

**[핵심/키워드]**

[ 특징 ]
* 장기간 수행, 사회공학기법, 정식권한 활용
[ 단계 ]
1) 계정생성
2) 기여도 누적
3) 권한 획득
4) 백도어 삽입
5) 정식 배포
[ 대응방안 ]
* 버전관리, 다운그레이드, 이상확인, 비정상 모니터링, 위협탐지, 킬스위치, 동작중지

### [분야] 메모리인터리빙 (Memory Interleaving)

**[정의]**

메모리를 여러 뱅크로 나누어 번갈아 접근함으로써 메모리 대역폭을 높이고 병목을 줄이는 성능향상 기법

**[핵심/키워드]**

[ 특징 ]
* 병렬처리, 메모리지연 완화, 연속주소 처리 최적, 하드웨어 기반 기술
[ 유형 ]
* 하위 (Low order, LSB-모듈, MSB-주소)
* 상위 (High order, MSB-모듈, LSB-주소)
* 혼합 (Combination / Mixed, MSB-뱅크, LSB-뱅크내부모듈)&lt;/font&gt;
[ 설계/접근 방식 ]
* C-Access (병렬, 동시처리)
* S-Access (동시데이터, 폭확장)&lt;/font&gt;

### [분야] HNDL (Harvest Now, Decrypt Later) 공격

**[정의]**

공격자가 암호화된 데이터를 수집 및 저장한 뒤, 나중에 양자기술이 충분히 발전하면 이를 해독하려는 공격방식

**[핵심/키워드]**

[ 특징 ]
* 햔재 데이터 수집 / 나중에 해독 공격
* 모스카 부등식 원리 활용
[ 동작과정 ]
1) 수집 (Harvest Now)
2) 대기 및 보관 (Storage) 
3) 해독 (Decrypt Later)&lt;/font&gt;
[ 대응방안 ]
* PQC (양자내성암호), 하이브리드 암호화, 암호 민첩성&lt;/font&gt;

### [분야] 블록암호화(Block Cipher)

**[정의]**

입력평문을 고정된 크기의 블록단위로 나누어 암호화하는 대칭키 암호방식

**[핵심/키워드]**

[ 구분 ]
- Feistel: 데이터를 두 블록으로 나누고 S-Box를 통한 연산과, XOR로 비선형 변환을 적용하는 구조(DES, 더블DES, 트리플DES, SEED)
- SPN: S-Box와 P-Box를 반복적으로 사용하는 구조(AES-서시미아, ARIA) 
* 평문 -&gt; SBOX -&gt; PBOX -&gt; 암호문

### [분야] 메모리 지역성 (Locality)

**[정의]**

프로그램이 실행되는 동안 기억장치내의 특정 영역을 집중적으로 반복 접근하는 경향성

**[핵심/키워드]**

[ 활용 ]
* Cache, Virtual Memroy, TLB
[ 목적 ]
* Hit율 상승, 평균 접근 시간 (Average Access Time) 단축
[ 종류 ]
* 시간적 지역성 (Temporal, 반복 접근)
* 공간적 지역성 (Spatial, 연속된 영역 접근)
* 순차적 지역성 (Sequential, 순서 접근)&lt;/font&gt;
[ 구현 사례 ]
* SW (선인출, 예상 페이징, 워킹셋, LRU, LFU, 배열접근)
* HW (메모리 계층 구조, 캐시 메모리, TLB, CDN, 프리패치 버퍼)

### [분야] 영지식 증명 (Zero-Knowledge Proof, ZKP)

**[정의]**

증명자(Prover)가 자신만 가진 비밀정보를 공개하지 않고 상대방인 검증자(Verifier)에게 비밀정보를 알고 있음을 증명할 수 있는 암호화 체계

**[핵심/키워드]**

[ 특징 ]
* 비밀정보 미공개 및 증명, 비존재 증명
[ 특성 ]
* 완전성 (Completeness), 건전성 (Soundness), 영지식성 (Zero Knowledge)&lt;/font&gt;
[ 동작 ]
1) Commitment 
2) Challenge 
3) Response 
4) 반복 및 검증
[ 유형 ]
* 대화식 영지식 증명 (여러번 질문/답변)
* 비대화식 영지식 증명 (단한번, 증명키)
[ 주요 알고리즘 ]
* zk-SNARK (짧고 비대화형, 신뢰설정) 
* zk-STARK (투명성, 신뢰설정 불필요)
* Bullet Proof (간소화된 증명) 
* Schnorr Protocol (대화형, 잘의응답) 
* Plonk (범용성, 다양한 회로)

### [분야] 동형 암호화 (Homomorphic Encryption)

**[정의]**

암호화된 데이터(암호문)를 &lt;u&gt;복호화 하지 않고도&lt;/u&gt; 덧셈, 곱셈 등의 연산을 수행할 수 있는 암호기술

**[핵심/키워드]**

[ 특징 ]
*암호 상태에서 연산 가능, 복호키 불필요, 프라이버시 보존
[ 종류 ]
* 부분동형암호화 (PHE), 준동형암호화 (SHE), 완전동형암호화 (FHE)&lt;/font&gt;
[ 알고리즘 ]
* Paillier, RSA, BGV, BFV, CKKS, TFHE
[ 라이브러리 ]
* 미국 (HELib, SEAL, PALISADE 2), 유럽 (NFLib, TFHE), 한국 (HeaAN)
[ 표준 ]
* ISO/IEC 18033-6&lt;/font&gt;

### [분야] 캐시 사상 (Cache Mapping) 방식

**[정의]**

캐시 메모리의 한정된 용량 때문에, 메인 메모리의 어떤 블록을 캐시의 어느 라인에 저장할 지 결정하는 규칙

**[핵심/키워드]**

[ 주소 필드 ]
* Tag / Line (Index) / Word (Offset)
[ 매핑 / 사상 방식 ]
* 직접 매핑 (Direct, Tag | Line | Word)
* 완전연관 (Fully Associative, Tag | Word)
* 집합연관 (Set Associative, Tag | Set Index | Word)&lt;/font&gt;

### [분야] 오펜시브 보안 (Offensive Security)

**[정의]**

&lt;u&gt;공격자의 입장에서&lt;/u&gt; 시스템을 바라보고, 침투 가능한 지점을 사전에 찾아내어 방어 전략을 수립하는 접근방식

**[핵심/키워드]**

[ 특징 ]
* 공격자 입장, 실제 위협 상황
[ 유형 ]
* 취약점 진단 (Vulnerability Assessment, 기본보안 점검)
* 모의 해킹 (Penetration Testing, Pen Test, 침투 가능성)
* 퍼플팀 테스트 (Purple Team Assessment, 레드 / 블루 협력)
* 레드팀 테스트 (Red Team Assessment, 기업 전반 실전 대응)&lt;/font&gt;

### [분야] 앙자 내성 암호 (Post-Quantum Cryptography, PQC)

**[정의]**

Shor/Grover 알고리즘이 효율적으로 해결할 수 없는 &lt;u&gt;수학적 문제&lt;/u&gt;를 이용해 양자환경에서도 공개키 암호의 보안성을 유지할 수 있도록 설계된 암호방식

**[핵심/키워드]**

[ 특징 ]
* 양자 내성, 새로운 수학 기반, 공개 키 대체 가능
[ 유형 ]
* 다변수 기반 (Multivariate, 다변수 다항식, Rainbow, GeMSS)
* 코드 기반 (Code, 복호 어려움, QC-MCPC, Wild McEliece)
* 격자 기반 (Lattice, 짧은벡터문제, Kyber, Dilithium)
* 아이소제니 기반 (Isogeny, 아이소제너경로, SIDH)
* 해시 기반 (Hash, 단방향 해시, SPHINCS+, XMSS)&lt;/font&gt;
[ 동향 ]
* ML-KEM (kyber, 키교환), ML-DSA (Dilithium, 전자서명), SLH-DSA (SPHINCE+, 해시)

### [분야] 캐시 일관성 (Cache Coherence)

**[정의]**

여러 CPU 코어가 동일한 메모리 블록을 각각의 캐시에 복사 시 항상 &lt;u&gt;동일한 최신값&lt;/u&gt;을 유지하도록 보장하는 메커니즘

**[핵심/키워드]**

[ 필요성 ]
* 모든 캐시가 동일한 최근 값 공유, 데이터 불일치 방지
[ 발생상황 [
* 캐시 쓰기 정책 (Write through, Write back), 멀티 Cache 환경
* DMA (Direct Memory Access)
[ 일관성 유지 기법 ]
* 하드웨어 공유 (단일 공유 캐시 사용, 공유 변수 캐시 미저장)
* 디렉토리 (Full, Limited, Linked / Chained)
* 버스 감시 기반 (Write Update, Write Invalidate)
* 쓰기 갱신 (Dragon, Firefly, Token)
* 쓰기 무효화 Write Invalidate (VI, MSI, MESI, MOESI, MESIF
* 소프트웨어 (Cache Clean, Cache Flush)&lt;/font&gt;

### [분야] 사이버 복원력 (Cyber Resilience)

**[정의]**

사이버 공간에서 발생하는 예측 가능한 공격, 알려지지 않았거나 예측 불가능한 위협에 대해 &lt;u&gt;조직의 목표를 달성하는 능력을 유지하고, 부정적 영향에도 불구하고 회복하는&lt;/u&gt; 역량

**[핵심/키워드]**

[ 특징 ]
* 예측 불가능한 위협 -&gt; 능력 유지 및 회복 역량
[ 등장배경 ]
* 디지털 인프라 사고 증가, 보안 사고 예방 한계
[ 구성 ]
* 비즈니스 영향분석, 보안정책통제, 종합적 테스트 정책, 매니지드 보안 도구 설치, 사이버 복구 계획
[ 확보단계 ]
1) 위협역량 평가 확보
2) 사이버보안 방법 도입
3) 위협기반 계획
4) 외부 위협으로부터 보호
5) 내부 위협 최소화
[ 성숙도 참조모델 ]
* 가시성, 사이버 위생, 요구사항, 시험 및 평가, 아키텍처, 정보 공유

### [분야] TLS1.3 (Transport Layer Security 1.3)

**[정의]**

인터넷상에서 안전한 통신을 보장하기 위해 이전 버전인 TLS 1.2의 보안 취약점과 성능 문제를 개선하여 더 빠르고 안전한 통신을 제공하기 위한 프로토콜

**[핵심/키워드]**

[ 표준 ]
* RFC 8446

[ 개선 ]
* 성능개선 (1-RTT Handshake, 0-RTT 전송&lt;/font&gt;, 연결과정 단축, 암호 스위트 단순화&lt;/font&gt; (AEAD&lt;/font&gt;), 불필요 기능 제거 (세션 재협상 등)
* 보안강화 (PFS 기본 적용 (ECDHE), 레거시 알고리즘 제거 (RSA 키교환, SHA-1), AEAD 강제적용, 초기부터 모든 메시지 암호화, 세션 재협상 제거)

### [분야] 메모리 단편화 (Fragmentation)

**[정의]**

주기억장치상에서 프로그램에 의해 사용되지 못하고 낭비되는 부분적인 기억공간

**[핵심/키워드]**

[ 발생원인 ]
* 고정 / 가변 메모리 할당, 프로세스 생성/종료 반복
[ 종류 ]
* 외부 단편화 (External Fragmentation)
* 내부 단편화 (Internal Fragemetation)&lt;/font&gt;
[ 해결기법 ]
* 통합 (Coalescing), 압축 (Compaction), 프레임 (Frame) 고정, Buddy Algorithm, Slab Allocation, Paging, Splitting, Memory Pool&lt;/font&gt;

### [분야] 애플리케이션 보안 테스트 (Application Security Testing, AST)

**[정의]**

소프트웨어 개발 과정에서 취약점 ·보안 결함을 조기에 식별하고 제거하기 위한 보안 테스트 도구

**[핵심/키워드]**

[ 특징 ]
* 개발 전주기 적용, 다양한 기법, 조기 식별 및 제거
[ 유형 ]
* SAST (Static AST, 정적, 실행 전)
* DAST (Dynamic AST, 동적, 실행환경)
* IAST (Interactive AST, 대화형, SAST + DAST, 동시분석)
* MAST (Mobile AST, 모바일)
* RASP (Runtime Apllication Self Protection, 실행중, Runtime)
* SCA (SW Conposition Analysis, SW 구성, 라이선스)
* ASTaaS (AST as a Service, 클라우드 서비스)
* ASTO (AST 오케스트레이션, 도구 통합 관리)&lt;/font&gt;
[ 활용 ]
* CTEM

### [분야] 디지털 워터마킹 (Digital Watermarking)

**[정의]**

디지털컨텐츠에 저작권을 표시할 수 있는 워터마크를 사용자가 지각적으로 &lt;u&gt;인지하지 못하도록&lt;/u&gt; 은닉하여 삽입하는 기술

**[핵심/키워드]**

[ 특징 ]
* 인지 못하도록 은닉 삽입, 저작권 보호, 추적 가능, 비가시성, 강인성
[ 유형 ]
* 기술방식 (디지털 워터마킹, 스테가노그래피, 핑거프린팅)
* 강인성 (강성 워터마킹, 연성 워터마킹)
* 시각성 (가시적 워터마킹, 비가시적 워터마킹)
* 알고리즘 (공간영역 워터마킹, 주퍄수영역 워터마킹)&lt;/font&gt;

### [분야] CPU 스레싱 (Thrashing)

**[정의]**

페이지 부재가 과도하게 발생하여 CPU가 실제 작업보다 페이지 교체에 대부분의 시간을 소비하는 비정상 상태

**[핵심/키워드]**

[ 문제점 ]
* CPU 사용률 급감, 페이지 부재 빈도 급증&lt;/font&gt;
[ 발생원인 ]
* 작은 메모리 할당, 잦은 페이지 교체, 과도하 멀티프로그래밍, 급격한 문맥교환
[ 해결기법 ]
* 발견 (Page Fault 조사, Swapping 조사)
* 프레임 관리 (Working Set, Page Fault Frequency, 프레임 할당 증가)
* 프로세스 관리 (Swap out, Load Control)
* 교체정책 (LRU-Clock, 지역성)
* 운용기반 (Quarantining)
* 자원최적화 (RAM 등 추가)&lt;/font&gt;

### [분야] AI 준비데이터 (AI Ready Data)

**[정의]**

AI가 신뢰할 수 있는 결과를 낼 수 있도록 데이터의 정렬·품질·거버넌스·비용효율성을 &lt;u&gt;체계적으로 갖춘&lt;/u&gt; 상태의 데이터

**[핵심/키워드]**

[ 특징 ]
* 정렬, 품질, 거버넌스, 비용효율성, 표준화 데이터
[ 핵심요소 ]
* 품질 (Quality), 정렬 (Align), 거버넌스 (Govern)
[ 기대효과 ]
* AI 모델 성능 향상, 신뢰기반 의사결정, 규정 준수, 거버넌스 강화
[ 추가 ]
* 가트너 하이퍼사이클 AI 2025

### [분야] OIDC (OpenID Connect)

**[정의]**

&lt;u&gt;OAuth를 기반으로&lt;/u&gt; 인증 기능을 확장한 인증 프로토콜

**[핵심/키워드]**

[ 특징 ]
* OAuth 확장, 사용자 정보 포함, JWT 기반, 사용자 정보 엔드포인트, idP
[ 세가지 역할 ]
* 최종 사용자 (EU), 의존 당사자 (RP), OpenID 공급자 (OP)&lt;/font&gt;
[ 인증 플로우 ]
* 권한 코드 플로우, 암시적 플로우, 하이브리드 플로우&lt;/font&gt;

### [분야] CXL (Compute Express Link)

**[정의]**

CPU·GPU·가속기·메모리 장치를 저지연·고대역폭으로 연결하기 위해 설계된 PCIe기반 &lt;u&gt;개방형 인터커넥트 표준&lt;/u&gt;

**[핵심/키워드]**

[ 필요성 ]
* 메모리 병목 해결, 이기종 지원, AI, HPC 등 고속 처리 
[ 프로토콜 ]
* CXL.io (IO연결)
* CXL.mem (메모리 확장)
* CXL.cache (캐시 일관성)&lt;/font&gt;
[ Device ]
* Type 1 (CXL.io + CXL.cache)
* Type2 (CXL.io + CXL.mem + CXL.cache)
* Type3 (CXL.io + CXL.mem)
[ Version ]
* CXL 1.0 / 1.1 (내부)
* CXL 2.0 (외부, 공유)
* CXL 3.0 / 3.1 (공유, Fabric)
* CXL 4.0 (RAS, PCIe 6.0/7.0, Bundled Port)&lt;/font&gt;

### [분야] AI OS (Artificial Intelligence Operating System)

**[정의]**

LLM을 운영체제의 두뇌로 삼아, 지능형 에이전트로서의 기능을 내재한 새로운 패러다임의 운영체제

**[핵심/키워드]**

[ 특징 ]
* 자율적 의사결정, 지속적 학습, 상황인식
[ 구성 ]
* LLM (LLM Core, LLM Scheduler)
* Data Manager (Context, Memory, Storage)
* Tool Manager (Tool, Access)&lt;/font&gt;
[ 확장 ]
* LLM Agent OS

### [분야] IAM (Identity Access Management)

**[정의]**

사용자의 신원(Identity)을 확인하고, 해당 사용자에게 적절한 자원 접근권한을 부여 및 관리하는 보안 프레임워크

**[핵심/키워드]**

[ 특징 ]
* 중앙집중, 자원 접근부여, 정책기반 제어, 자동화, Provisioning
* EAM + 감사 + 정책 + Provisioning
[ 구성요소 ]
* Identity (신원), Authentication (인증), Authorization (인가), Policies (정책), Audit, Logging, Provisioning&lt;/font&gt;
[ 클라우드에서의 IAM 중요성 ]
* 다중 사용자 환경, 공개 환경 노출, 컴플라이언스 대응

### [분야] DMA (DirectMemory Access)

**[정의]**

&lt;u&gt;CPU 개입 없이&lt;/u&gt; I/O장치가 메모리와 &lt;u&gt;직접 데이터 전송을 수행&lt;/u&gt;하는 고속 I/O방식

**[핵심/키워드]**

[ 특징 ]
* 대량, 고속 I/O, CPU 개입 / 부하 최소
[ 구성요소 ]
* DMA Controller, Memory, 장치 Controller, CPU
[ 동작 과정 ]
* CPU가 DMA 설정 &gt; 버스 요청 (BR) &gt; 버스 양도 (BG) &gt; DMA / IO 장치 전송 &gt; 반복 &gt; CPU에 인터럽트 통보 &gt; CPUr가 다음동작 처리
[ 명령어 ]
* DS (DMA Select), RS (Register Select), BR (Bus Request), BG (Bus Grant)
[ DMA Register ]
* Address Register, Word Count Register, Control Register
[ 전송구조 / 버스 방식 ]
* 단일버스 DMA, 단일통합 DMA, 입출력 버스 DMA
[ 동작 모드 ]
* Burst / Block (버스 독점, 대량 전송)
* Cycle Stealing (사이클 steal, 1 word, 1 byte)
* Transparent / interleaved (유휴시간)&lt;/font&gt;

### [분야] AI 웹 브라우저 (Artificial Intelligence Web Browser)

**[정의]**

AI기술을 핵심으로 사용자에개 인화되고 자동화된 지능형 웹 탐색 경험을 제공하는 차세대 브라우저

**[핵심/키워드]**

[ 특징 ]
* 콘텐츠 용약, 자동화, 지능형 웹 탐색, 고도화된 개인화
[ 주요기술 ]
* 인공지능 (LLM, NLP, Edge AI)
* 인식 (Context, Agent Mode, Contents 분석)
* OS 운영 (개인화, WebGPU, Skill 시스템, Headless 브라우저)&lt;/font&gt;

### [분야] IDS (Intrusion Detect System)

**[정의]**

비인가된 사용자가 자원의 기밀성, 무결성, 가용성을 저해하는 일련의 행동들과 보안 정책을 위반하는 행위, 즉 침입을 실시간으로 탐지하는 시스템

**[핵심/키워드]**

[ 특징 ]
* 실시간 탐지, 침입 및 위협 탐지, 행위기반 탐지, 수동적 대응
[ 구성요소 ]
* 정보수집기, 정보분석기, 로그 저장소, 이벤트 보고기, 패턴 생성기, 패턴 DB / 시그니처 DB&lt;/font&gt;
[ 유형 ]
* 설치 위치 (NIDS, HIDS, Hybrid)
* 탐지 방식 (시그니처 기반, 행위기반 )
* 대응 방식 (수동, 능동)
* 탐지 시점 (사후분석, 실시간)&lt;/font&gt;
[ 탐지 종류 ]
* 오용탐지, 이상탐지

### [분야] RDMA (Remote Direct Memory Access)

**[정의]**

CPU 개입 없이 네트워크를 통해 &lt;u&gt;원격 메모리에 직접 접근하여&lt;/u&gt; 데이터 전송하는 기술

**[핵심/키워드]**

[ 특징 ]
* 다른 Host DMA, CPU 개입 없음, Zero-copy, Kernel bypass, HCA
[ 구성요소 ]
* RNIC (RDMA NIC), RDMA Adapter, RDMA Operation, Queue Pair (QP)&lt;/font&gt;
[ 프로토콜 / 구현방식 ]
* Infiniband (초고속, 저지연, Fabric)
* RoCE (Ethernet, PFC, ECN)
* iWARP (TCP/IP, Q Pair)&lt;/font&gt;

### [분야] 월드모델 (World Model)

**[정의]**

텍스트,이미지,영상을 넘어 &lt;u&gt;현실 세계의&lt;/u&gt; 물리법칙, 공간, 상호작용까지 이해, 시뮬레이션하는 인공지능 모델

**[핵심/키워드]**

[ 특징 ]
* 현실세계 이해, 멀티 모달리티, 상호작용 환경, 미래 예측
[ 구성요소 ]
* 인지, 역학, 메모리, 롤아웃, 시뮬레이터, 플래너
[ 평가지표 ]
* 예측 오차, 롤아웃 품질
[ 초기 시스템 구성 ]
* 비전 (Vision, VAE, 압축), 메모리 (Memory, MDN-RNN, 다음 예측), 컨트롤러 (Controller, 보상최대화)
[ 주요고려사항 ]
* 데이터 큐레이션 (Data Curation), 토큰화 (Tokenization), 파인튜닝 (Fine-tuning), 강화학습 (RL)&lt;/font&gt;
[ 4가지 패러다임 / 모델 ]
* 암시적 모델 (미분리, 하나의 신경망), 명시적 모델 (상태/관찰 분리), 시뮬레이터 (시뮬레이션 테스트), 하이브리드 (학습모델+규칙)&lt;/font&gt;
[ 활용 ]
* Dreamer v3, WFM, NWM

### [분야] WIPS (Wireless Intrusion Protection System)

**[정의]**

&lt;u&gt;무선네트워크(Wi-Fi)에&lt;/u&gt; 대한 침입을 탐지하고 차단하는 보안 시스템

**[핵심/키워드]**

[ 특징 ]
* 무선환경, IPS (탐치+차단), De-authentication Packet
[ 기능 ]
* 불법 AP, Rogue AP 탐지, 스푸핑 방어, 정책 위반 감시
[ 구성 ]
* Sensor, Server, Console, Management&lt;/font&gt;
[ 유형 ]
* Controller 기반 (AP + Controller)
* Sensor 기반 (전용센서 + 서버)

### [분야] RAID (Redundant Array of Independent Disks)

**[정의]**

여러 개의 물리 디스크를 하나의 논리 디스크처럼 구성하여 성능·신뢰성·가용성을 향상시키는 기술

**[핵심/키워드]**

[ 원리 ]
* Data Striping, Redundancy, Mirroring, Parity Protection&lt;/font&gt;
[ 특징 ]
* 성능향상, 신뢰성 및 가용성 향상, 높은 확장성
[ 유형 ]
* RAID 0 (Striping), RAID 1 (Mirroring), RAID 2 (Bit Striping, Hamming ECC), RAID 3 (Byte Striping, 전용 Parity), RAID 4 (Block Striping, 전용 Parity), RAID 5 (분산 패리티), RAID 6 (이중 패리티), RAID 0+1 (Striping -&gt; Mirroring), RAID 1+0 (Mirroring -&gt; Striping), RAID 5+0, RAID 5+1, RAID 6+0&lt;/font&gt;
[ 구성요소 ]
* RAID 전용 Controller, Cache Memory, Recording 방식, Mirroring, Hot-Swap
[ 방식 ]
* Software RAID, Hardware RAID

### [분야] AgentOps

**[정의]**

AI 에이전트의 관찰, 제어, 최적화 수행과 수명주기 관리에 초점을 맞춘 개발 및 운영 패러다임

**[핵심/키워드]**

[ 특징 ]
* 자율적, Agent 중심, 지속학습, 사전예방운영
[ 핵심구성 ]
* 구축 및 평가, 관찰가능성, 모니터링 / 알림, 디버깅도구, 비용 및 자원 관리, 거버넌스 및 규정 준수

### [분야] VPN (Virtual Private Network)

**[정의]**

터널링(Tunneling) 기법을 사용해 인터넷과 같은 &lt;u&gt;공중망에서 전용회선을 구성한 것과 같은 효과를&lt;/u&gt; 내는 가상 네트워크

**[핵심/키워드]**

[ 특징 ]
* 공용 NW -&gt; 사설 NW, 보안성 강화, 원격접속지원, 유연한 구성
[ 주요 기능 ]
* 암호화, 터널링, 무결성 보호, 사용자 인증, 원격접속 지원
[ 주요 프로토콜 ]
* Layer 2 (L2TP, PPTP, L2F, MPLS)
* Layer 3 (IPSec)
* Layer 4 이상 (SSL / TLS)&lt;/font&gt;
[ 추가 프로토콜 ]
* OpenVPN, WireGuard, IKEv2/IPSec
[ 구현기술 ]
* 터널링 (가상경로), 암호화 (데이터보호), 인증 (사용자 인증), 키관리 (키 분배/관리), 복수 프로토콜 (다양한 트래픽 처리)&lt;/font&gt;
[ 토폴로지 구성 유형 ]
* Point to Point, Hub and Spoke, Full Mesh, Partial Mesh, Overlay, Peer to Peer
[ 사이트 구성 유형 ]
* Lan to Lan (Site to Site), Lan to Client (Remote Access)

### [분야] 서버가상화 (Server Virtualization)

**[정의]**

물리 서버 자원을 하이퍼바이저를 통해 &lt;u&gt;논리적으로 분리·추상화하여&lt;/u&gt; 가상머신(VM) 형태로 제공하는 기술

**[핵심/키워드]**

[ 목적 ]
* 자원 활용 증가, 서버 통합, 운영 효율화, Scale out, 고가용성
[ 핵심요소 ]
* 하이퍼바이저, OS레벨, 가상자원 (vCPU, vNIC, vMemroy, vDisk)&lt;/font&gt;
[ 운영구조 ]
* 다중 VM, 자원 자동배분, 클러스터 기반 서버 가상화
[ 유형 ]
* 하이퍼바이저 (Type 1 (베어메탈/네이티브), Type2 (Host/Embedded)
* Type 1 (전가상화, 반가상화)
* OS (컨테이너)&lt;/font&gt;

### [분야] 머신 언러닝 (Machine Unlearning)

**[정의]**

이미 학습된 머신러닝 또는 딥러닝 모델에서 특정 데이터를 &lt;u&gt;선택적으로 제거하여, 마치 해당 데이터를 학습하지 않은 것처럼&lt;/u&gt; 만드는 기술

**[핵심/키워드]**

[ 특징 ]
* 개인정보와 모델 정합성 균형, 프라이버시 준수, 잊힐권리 준수
[ 목적 ]
* 법적 규제 (개인정보 제거), 비용절감 (재학습 최소화), 윤리적 (편향 제거), 업데이트 용이 (불필요 데이터 삭제)
[ 주요 기술 ]
* 알고리즘 (SISA, Fine tuning, Gradient Reversal, Approximate Unlearning, Exact Unlearning, Anti Sample Generation)
* 데이터 셋 (Retain Set, Forget Set)
* 시스템 (DP, Model Utility, Federated Unlearning)
* 측정지표 (Forgetting Metrics, Computational Efficiency)
* 효과 평가지표 (잔여데이터 정확도, 언러닝 시간, 망각률, 멤버십 추론 공격 성공률)&lt;/font&gt;

### [분야] 보안 운영체제 (Secure OS / Operating System)

**[정의]**

운영체제차원에서 내부자·악성행위·침입 위협으로부터 시스템을 보호하기 위해, 커널 수준에서 강제 접근제어, 무결성 보호, 감사 기능 등을 내장한 보안강화 운영체제

**[핵심/키워드]**

[ 특징 ]
* 보안강화 OS, 보안 커널, 강제접근제어, 최소권한, &lt;/font&gt;
[ 구성요소 ]
* 보안커널, 정책관리자, 무결성 보호 모듈, 감사로그 모듈, 보안도구&lt;/font&gt;
[ 주요기능 ]
* 보안기능 내재, 다계층 보안요소 내장
[ 보안커널 ]
* 격리성, 검증가능성, 완전성, 참조모니터 구현, TCB, TPM
[ 사례 ]
* SELinux, AppArmor

### [분야] 도커 (Docker)

**[정의]**

애플리케이션을 컨테이너(Container)로 패키징·배포·실행할 수 있게하는 컨테이너 플랫폼

**[핵심/키워드]**

[ 특징 ]
* 공유 (Host OS), 격리 (샌드박스), 이미지기반
[ Runtime 변화 ]
* LXC &gt; runc &gt; containered Kubernetis 런타임
[ 구성 ]
* Docker Engine, Docker Daemon, 과거 (LXC, libcontainer), 현재 (containered, runc), Docker Hub, Docker CLI, Docker Rest API, Docker Container, Docker Network, Docker Volumn, Buildkit&lt;/font&gt;
[ 동작과정 (배포) ]
* 소스코드 &gt; 이미지 빌드 &gt; 이미지 push &gt; 이미지 search &gt; 이미지 pull &gt; 컨테이너 run
[ 관리 ]
* Docker Swarm

### [분야] 바이브코딩 (Vibe Coding)

**[정의]**

자연어·음성 기반의 직관적 개발방식, 전통적인 &lt;u&gt;키보드 코딩 없이 AI 도구를 활용해&lt;/u&gt; 코드 생성·수정·통합하는 신개념 개발 패러다임

**[핵심/키워드]**

[ 특징 ]
* 자연어로 SW 구성, AI 코드 보조도구 연계, 의도전달 중심
[ 개발 생태계 변화 ]
* 비개발자 접근성 향상, AI 의존도 증가, 개발자 역할 변화
[ 주요기술 ]
* 자연어처리, 코드 생성 AI, 음성인식 (ASR), 멀티모달 인터페이스, 컨텍스트 유지기술, 실행 및 통합 플랫폼, 버전관리, CI/CD, 테스트 코드 자동생성, 시멘틱 코드검색&lt;/font&gt;
[ 동작 ]
1) 요구사항 / 규칙
2) AI 코드 생성
3) 공유 IDE / 실시간 협업
4) 테스트 / 배포
[ 구성 ]
* 코드 프롬프팅, 개발 플랫폼, 자연어 및 아이디어 입력, 코드 및 결과
[ 주요도구 ]
* 요구사항 / 문서 (Markdown, PRD, BRD, Mermaid)
* 개발환경 (Cursor, Windsurf, Replit, MCP)
* 협업/운영 (GitHub, CI/CD)

### [분야] EDR (Endpoint Detection and Response)

**[정의]**

단말에서 발생하는 이상 행위나 침해 징후를 탐지하고, 조사·분석·대응까지 수행하는 지능형 위협대응 솔루션

**[핵심/키워드]**

[ 특징 ]
* 행위기반 탐지, 추적, 대응, 사후대응 중심&lt;/font&gt;
[ 기능 ]
* 이상행위 탐지, 파일 및 프로세스 추적, 단말 격리, 자동 대응 / 경고
[ 가트너의 EDR 주요 기능 ]
* 예측 (Predict, 위협 사전 식별, 사전 평가)
* 탐지 (Detect, 이상탐지, 격리)
* 방어 (Prevent, 시스템 강화, 단말 격리)
* 대응 (Response, 치료, 정책 조정)&lt;/font&gt;
[ 동향 ]
* EDR을 넘어서 지능형 EDR, XDR, MDR 등 확장

### [분야] 쿠버네티스 (Kubernetes, k8s)

**[정의]**

컨테이너화된 애플리케이션을 자동 배포·스케줄링·확장·복구하는 오케스트레이션 플랫폼

**[핵심/키워드]**

[ 특징 ]
* 대규모 컨테이너 환경, 자동화, 표준화, 고가용성, Self-Healing
[ 구성요소 ]
* Master Node, Worker Node, Workload / Resource
* Master Node (API Server, etcd, Scheduler, Controller Manager, Cloud Controller Manager)
* Worker Node (Kubelet, Container Runtime, Kube-Proxy)
* Workload (Pod, ReplicaSet, Deployment, Service, ConfigMap / Secret, Ingress, Volumn)&lt;/font&gt;
[ 핵심 오케스트레이션 기능 ]
* Probe, Self Healing, Auto Scaling
[ 연관 ]
* 경량 --&gt; k3s, 제로기반 --&gt; k0s, CLI 관리 --&gt; k9s

### [분야] 네오 클라우드 (NeoCloud)

**[정의]**

학습 및 추론에 필수적인 고성능 &lt;u&gt;GPU를 대규모로 확보하여&lt;/u&gt; 특화된 AI 컴퓨팅 환경을 제공하는 차세대 클라우드 서비스

**[핵심/키워드]**

[ 부각배경 ]
* AI 폭증, GPU 인프라 필요성, 유연한 서비스 모델, 하이브리드 인프라
[ 기술요소 ]
* GPU 클러스터 (GPU, Instinct) 
* 고속 네트워킹 (Infiniband, NVLink, RoCE)
* GPUaaS (RunPod)
* AI SW 스택 (Docker, CuDA)
* 오케스트레이션 (Kubernetes, Teraform)
* 동적자원 (Autoscaler)

### [분야] SOAR (Security Orchestration, Automation and Response)

**[정의]**

보안 운영팀이 다양한 보안 시스템, 이벤트, 대응 프로세스를 자동화·통합·조정하여 효율적인 보안 위협 대응을 가능하게 하는 플랫폼

**[핵심/키워드]**

[ 특징 ]
* 자동화, 통합 대응, 신속 대응, 분석 효율, 효율적 위협 대응
[ 구성 ]
* SOA ( 보안 오케스트레이션 및 자동화)
* SIRP (보안사고 대응 플랫폼)
* TIP (위협 인텔리전스 플랫폼)&lt;/font&gt;
[ 주요기능 ]
* 오케스트레이션, 자동화, 사고대응, 플레이북 관리, 대시보드

### [분야] 데스크톱가상화 (Desktop Virtualization)

**[정의]**

사용자 데스크톱 환경을 중앙 서버 또는 클라우드에서 가상머신 형태로 실행, 사용자는 네트워크를 통해 원격접속하여 사용하는 기술
* Zero PC / Zero Client

**[핵심/키워드]**

[ 특징 ]
* 중앙집중관리, 디바이스 독립성
[ 구성 ]
* 클라이언트 (단말기)
* 접속관리 (세션 브로커 Session Broker)
* 인증/정책 (인증 서버 Authentication Server)
* 가상화 엔진 (하이퍼바이저 Hypervisor)
* 가상머신운영 (가상머신운영서버)
* 프로비저닝 (프로비저닝 시스템)
* 스토리지 (공유 스토리지)&lt;/font&gt;
[ 유형 ]
* VDI (개별 VM 데스크탑)
* RDS / RDSH (세션 단위 공유)
* DaaS (클라우드 제공)&lt;/font&gt;

### [분야] iPaaS (Integration Platform as a Service)

**[정의]**

클라우드, 온프레미스 환경에서 서로 다른 애플리케이션, 데이터, 서비스를 통합 (Integration)하기 위한 플랫폼 서비스

**[핵심/키워드]**

[ 특징 ]
* 통합 플랫폼 서비스, 노코드 / 로우코드, 실시간 데이터 처리, 보안 및 접근제어 기능
[ 주요기술 ]
* 클라우드 서비스, API G/W, 워크플로우 빌더, 메시지 큐, 이벤트 스트림, OAuth, TLS, ETL, 이벤트 브로커
[ 구성요소 ]
* 통합 흐름 실행, 통합 개발 및 수명주기 관리, 애플리케이션 흐름 관리 및 모니터링, 데이터 접근 보안수단, 필수 클라우드 기능 지원 도구&lt;/font&gt;

### [분야] CNAPP (Cloud Native Application Protection Platform)

**[정의]**

클라우드 네이티브 애플리케이션의 전체 수명주기 (개발~운영)에서 보안을 통합 관리하는 플랫폼

**[핵심/키워드]**

[ 특징 ]
* CWPP, CSPM 등 여러 보안 기능 통합 플랫폼, 한 번에 보호
* 클라우드 네이티브 보호, 전체 수명주기 커버, 실시간 위험 탐지
[ 구성요소 ]
* CSPM (자산 설정 오류 및 관리)
* CWPP (워크로드 보호)
* CIEM (계정 권한 통제)
* Container / Serverless 보안 (클라우드 네이티브 보호)
* IaC 보안 (인프라 보안)
* SBOM / Compliance (구성요소 식별 / 준수)&lt;/font&gt;

### [분야] 결함허용 (Fault Tolerance, FT / 내고장성)

**[정의]**

시스템 구성요소에 결함이 발생하더라도 서비스가 중단 없이 지속되도록 보장하는 기술

**[핵심/키워드]**

[ 목적 ]
* Zero downtime, 단일장애점 제거, 연속성 / 신뢰성 극대화
[ 핵심요소 ]
* 중복성 기반 이중화, Lockstep 실행, 동기식 복제
[ 결함 해결 ]
* 결함 탐지 &gt; 결함 진단 &gt; 결함 통제 &gt; 결함 복구&lt;/font&gt;
[ 구현 기술 ]
* HW (Duplication, Standby, TMR, WDT, Self-purging)
* DB (Rollback, Log File, Checkpoint, Shadow paging)
* SW (Check pointing, Recovery block, Conversation, DRB, N-Self checking, N-version)
* Data (Parity, M of N, Checksum, Berger code, Hamming ECC)&lt;/font&gt;

### [분야] CBDC (Central Bank Digital Currency)

**[정의]**

기존 현금의 기능을 디지털 형태로 구현한 국가 단위의 통화로 중앙은행이 발행하고 관리하는 법정 디지털 화폐

**[핵심/키워드]**

[ 특징 ]
* 국가/중앙은행, 현금-&gt;디지털 형태, 법정화폐
[ 거래방식 ]
* 분산원장 (허가, 비허가), 단일원장&lt;/font&gt;
[ 종류 ]
* 리테일 (범용) CBDC, 홀세일(기관용) CBDC&lt;/font&gt;
[ 기대효과 ]
* 비용감소, 위변조 방지, 실시간 화폐 이동 데이터 활용
[ 동향 ]
* 한국 (프로젝트 중단), 미국 (반 CBDC 법 통과로 금지), 유럽 (디지털 유로 프로젝트), 중국 (디지털위안 시범 서비스)

### [분야] 파일 카빙 (File Carving, FC)

**[정의]**

파일 시스템의 메타 데이터 없이, 디스크의 순수한 바이너리 데이터를 분석하여 파일을 복원하는 기술

**[핵심/키워드]**

[ 특징 ]
* 시그니처 기반 복원, 메터 데이터 미복원, 바이너리 데이터 분석
[ 단계 ]
1) 복구대상 식별
2) 유효성 검증 (시그니처, 구조체) / 연속성 판단 (연속 / 비연속)
3) 카빙 방법 결정&lt;/font&gt;
[ 기법 ]
* 시그니처 기반 (시작 종료 패턴 중심, Header / Footer, Header / RAM Slack)
* 구조체 기반 (데이터 포맷이나 규칙 중심, Header / File Size, File 구조 검증)&lt;/font&gt;

### [분야] 고가용성 (High Availability, HA)

**[정의]**

시스템 구성요소 장애 발생시에도 &lt;u&gt;서비스 중단시간을 최소화하여&lt;/u&gt; 지속적인 서비스 제공을 보장하는 기술 ·아키텍처

**[핵심/키워드]**

[ 목적 ]
* 단일 장애점 제거, 장애 발생 시 빠른 복구 및 빠른 전환&lt;/font&gt;
[ 구성요소 ]
* 기능 (클러스터링, Heart beat, Health check, Failover Manager, 이중화, 상태동기화, 공유 스토리지)
* 물리 (서버노드, 공유 스토리지, 네트워크 경로, 클러스터 소프트웨어)
* 운영/정책 (Failback, Rollback, RTO, RPO, SLA, 서비스 모니터링, 로그 / 이벤트 관리)
* 데이터 (데이터 복제, 데이터 일관성, 스냅샷 / 백업)
* 확장 (로드밸런서, Auto Scaling)
* 보안 (Heartbeat 네트워크 보안, RBAC)
* DR (DR Site, DR 오케스트레이터, WAN 최적화)&lt;/font&gt;

### [분야] STO (Security Token Offering)

**[정의]**

부동산, 미술품, 지식재산권 같은 실물 자산과 주식, 채권, 펀드같은 금융자산을 블록체인 기반 토큰과 연동해 발행한 &lt;u&gt;디지털 증권&lt;/u&gt;

**[핵심/키워드]**

[ 특징 ]
* 증권에 해당, 규제/감독 체계 안에서 발행/유통
[ 특징 ]
* 높은 유동성, 분할 소유 (조각투자), 비용감소 (스마트 컨트랙트), 투자자보호, 프로그래밍 가능성, 실물가치 근거
[ 동향 ]
* 법제화 추진 중

### [분야] OWASP (Open Web Application Security Project) Top 10 2025

**[정의]**

OWASP에서 웹 애플리케이션의 가장 중요한 보안위험 10가지를 선정하여 주기적으로 발표하는 목록의 2025년 버전

**[핵심/키워드]**

[ 특징 ]
* 웹 애플리케이션의 중요한 보안 위험 10가지
[ 10가지 항목 ]
* A01 (취약한 접근 통제, Broken Access Control)
* A02 (보안설정 오류, Security Misconfiguration)
* A03 (소프트웨어 공급망 실패, Software Supply Chain Failure)
* A04 (암호화 실패, Cryptographic Failures)
* A05 (인젝션, Injection)
* A06 (안전하지 않은 설계, Insecure Design)
* A07 (인증실패, Authentication Failures)
* A08 (소프트웨어 및 데이터 무결성 실패, Software or Data Integrity Failures)
* A09 (로깅 및 경고 실패, Logging and Alerting Failures)
* A10 (예외 조건의 오처리, Mishandling of Exceptional Conditions)

### [분야] HBM (High Bandwidth Memory)

**[정의]**

고성능 데이터 처리를 위해 DRAM 적층화 및 TSV 배선기반 데이터 이동 병목현상을 해소한 DRAM 적층형 고성능 메모리

**[핵심/키워드]**

[ 특징 ]
* 초고대역폭, 저전력, 고용량, 초고속 패키징, 고성능 AI / HPC 지원, TSV 적층, DRAM
[ 구성요소 ]
* 메모리 적층 (TSV, DRAM Die, Base / Login Die, Micro Bump)
* 칩셋 (SoC, PHY, Silicon Interposer, Package Substrate)&lt;/font&gt;
[ 적층화 기법 ]
* TSV (다층 통로), CoW (웨이퍼에 칩 부착), TCB (열압착), TC-NCF (비전도성, 특수필름), MR-MUF (액체성, 경화), 하이브리드 본딩 (동시접합)&lt;/font&gt;
[ 버전 ]
* HBM3E / HBM4

### [분야] 실물연계자산 (Real World Asset, RWA)

**[정의]**

부동산, 금, 예술품, 채권 등 실물 및 전통 금융 자산을 블록체인의 토큰으로 발행하는 기술

**[핵심/키워드]**

[ 특징 ]
* 유동성, 분할 투자, 실물 연계, 온체인 담보
[ 구성 ]
* 실물자산, 디지털 자산 (ERC-721, RWA 토큰, STO 토큰)
* 스마트 계약 (알트코인), 분산원장기술 (DLT, 블록체인, DAG)
* 합의알고리즘 (PoS, PoA), 오라클 (블록체인 오라클), 법적 프레임워크 (KYC / AML)
* 자산관리 플랫폼 (DeFi, 자산거래소)&lt;/font&gt;
[ 프로토콜 유형 ]
* RWA 토큰화 프로토콜 (실물 예치, 담보)
* RWA 담보대출 프로토콜 (RWA 토큰 담보, Vault)&lt;/font&gt;

### [분야] 가디언 에이전트 (Guardian Agent)

**[정의]**

신뢰할 수 있고 안전한 AI 상호작용을 지원하기 위해 다른 AI 에이전트를 감독하도록 설계된 AI에이전트

**[핵심/키워드]**

[ 특징 ]
* 다른 에이전트 감독 설계, 아넌한 AI 상호작용 지원
[ 발전단계 ]
1) 품질관리 (Qualtiy Control, 정확도 및 일관성 검증)
2) 관찰 (Observation, 이상행위 탐지)
3) 보호 (Protection, 자동 방어 / 종료)
[ 주요 영역 ]
* 보안 (Security), 관측가능성 (Observability), 필터링 및 모니터링 (Filtering and Monitoring), 다중에이전트 시스테 (Multi Agent System), 에이전트 오케스트레이션 (Agent Orchestration)&lt;/font&gt;
[ 활용 분야 ]
* 보안 운영, 인간 개입형 모니터링, 자가치유 프로세스, AI 신뢰 관리, 자율시스템

### [분야] TPU (Tensor Processing Unit)

**[정의]**

신경망 연산의 핵심인 행렬곱·벡터연산을 초고속으로 수행하도록 설계된 특수목적형 하드웨어

**[핵심/키워드]**

[ 특징 ]
* 행렬연산가속기 중심, 시스톨릭 어레이 (Systolic Array), 더 높은 연산밀도, 특수목적형 ASIC
[ 구성요소 ]
* 연산 (MXU, 시스톨릭 어레이, 벡터-스칼라 유닛)
* 메모리-데이터 (고대역폭 메모리, 온칩 버퍼-데이터)
* 정밀도-연산 (Mixed-Precision)
* 확장/연결 (TPU Pod, 고속 인터커넥트)
* 아키텍처 (ASIC 기반 AI 전용)
* 컴파일러 (컴파일러 최적화)&lt;/font&gt;
[ 버전 ]
* TPU v6e (Trillium) / TPU v7 (Ironwood, 추론 최적화 및 대규모 확장)

### [분야] 스테이블코인 (Stable Coin)

**[정의]**

일반적으로 지급 또는 결제 수단으로 사용할 목적으로 설계되어, 고정된 화폐가치(Pegging)로 전환되거나 상환될 수 있는 디지털 자산

**[핵심/키워드]**

[ 특징 ]
* 페깅, 고정된 화폐가치, 변동성 자산 확보
[ 유형 ]
* 법정화폐 담보형, 가상자산 담보형, 알고리즘 기반형, 실물자산 담보형&lt;/font&gt;
[ 위험성 ]
* 디페깅 (De-pegging), 운영/신뢰 리스크, 규제 리스크&lt;/font&gt;
[ 활용 ]
* 국가간 송금, 결제

### [분야] AI 레드팀 테스트(AI Red Team Test)

**[정의]**

* AI 모델 또는 시스템의 잠재적인 취약점, 편향, 사회적 해악, 보안 문제 등을 식별하기 위해 의도적으로 다양한 공격을 시도하고 한계를 시험하는 적대적인 탐색적 테스팅 방법
 * 공격자 관점에서 AI 시스템의 취약성·오용경로를 발굴하는 시나리오 기반 보안·안전성 평가 
* ISO/IEC 42119-7

**[핵심/키워드]**

[ 목적 ]
* 취약점 식별, 오남용 경로 탐지, 완화책 검증, 환각 등 문제 해소 
[ 주요 대상 ] 
* 입력(프롬프트) 처리, 출력(생성물) 안전성, API·인프라 보안, 데이터 유출·모델 인버전&lt;/font&gt;
[ 단계 ]
1) 위협 모델링 (자산·공격자·경로 정의)
2) 시나리오 설계 (실사용·오남용 기반)
3) 공격 수행 (프롬프트 인젝션·탈옥·데이터 추출·적대적 입력 등)
4) 결과 검증 및 완화 재검증 
[ 구성원 ]
* 보안 리드, ML 엔지니어, 데이터 엔지니어, 도메인 전문가, 법무·윤리 담당, QA/운영
[ 주요 테스트 ]
* 모델 테스트, 시스템 테스트
[ 모델 테스트 기법 ]
* 허위공격, 적대적 입력(Adversarial Input), 편향·유해성 유도 공격, Agent 오동작 유도
[ 시스템 테스트 기법 ]
* 데이터 포이즈닝(오염) 검출, 데이터 유출·권한 탈취 탐지, 가드레일 무력화 검증, 보안 경계 테스트, 공격 대응 능력 평가 
[ 산출물 ]
* 취약점 리포트 및 위험 가시화 보고서, 신규 가드레일·필터링 규칙 제안, 보안 대응·개선 방안, 신규 평가지표·테스트 케이스 
[ 표준, ISO/IEC42119-7&lt;/font&gt; ] 
* AI레드팀 테스팅에 대한 용어,절차,방법들을 정의한 AI레드팀에 대한 최초의 국제 공통 표준.
* ETRI에서 에디터 역할로 국제 공통 시험 절차 방법 구축 중

