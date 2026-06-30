---
layout: post
title: "와탭, PLG, Pinpoint"
date: 2026-06-30
categories: Chat
tags: [Chat]
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

### 상세 내용

**1. 옵션 A: WhaTap (SaaS APM) 기반 통합 모니터링**

상용 솔루션인 와탭을 사용하면 구성이 간편하고, 한국어 지원 및 직관적인 통합 대시보드를 구축하기 매우 용이합니다.


**🎯 티어별 적용 방안**

- **인프라 (VM &amp; Docker) - 와탭 서버 모니터링 (SMS):**
- 각 VM(web, was, db 등)의 Host OS에 와탭 서버 모니터링 에이전트를 설치합니다.
- Docker Compose 환경이므로 서버 에이전트가 컨테이너들의 CPU, Memory 사용량 등의 메트릭을 함께 수집하도록 설정합니다.
- **애플리케이션 (Node.js, Spring Boot) - 와탭 APM:**
- **Web/ApiGateway (Node.js):** Node.js 패키지에 `whatap` 모듈을 설치하고, Dockerfile 또는 `docker-compose.yml`의 환경변수(WHATAP_HOME, WHATAP_SERVER_HOST 등)를 통해 APM 에이전트를 연동합니다.
- **WAS (Spring Boot):** Dockerfile 작성 시 와탭 Java Agent(`whatap.agent.jar`)를 포함시키고, `java -javaagent:/whatap/whatap.agent.jar -jar app.jar` 형태로 컨테이너를 실행하여 트랜잭션, 힙 메모리, DB 쿼리 소요 시간 등을 추적합니다.
- **데이터베이스 (PostgreSQL, Redis) - 와탭 DB 모니터링:**
- 별도의 모니터링용 VM(또는 관리영역 서버)에 DB 모니터링 에이전트를 설치하고, PostgreSQL 및 Redis 인스턴스의 엔드포인트로 접근하여 Active Session, Lock, Slow Query, Redis Hit Rate, Replication Lag(지연) 등을 수집합니다.

**2. 옵션 B: Prometheus 기반 오픈소스 모니터링 (클라우드 네이티브)**

라이선스 비용을 절감하고, 개발자/엔지니어 입맛에 맞게 커스터마이징이 필요할 때 사용하는 스택입니다. **Prometheus + Grafana + Loki / OpenTelemetry** 조합을 추천합니다.

**🎯 티어별 적용 방안 및 Exporter 구성**

 | **수집 대상** | **수집 도구 (Exporter / Agent)** | **모니터링 핵심 지표**

 | VM OS (Host)** | `node_exporter` | Host CPU, Memory, Disk I/O, Network Traffic
 | **Docker Compose** | `cAdvisor` | 개별 컨테이너별 자원 사용량 (OOM 킬 방지)
 | **Spring Boot (WAS)** | Spring Boot Actuator + `Micrometer` | JVM Heap, GC, Thread Pool, HTTP TPS, Error Rate
 | **Node.js (Web/API)** | `prom-client` (npm 패키지) | Event Loop 지연, Active Handles, Memory 사용량
 | **PostgreSQL (DB)** | `postgres_exporter` | Connection 수, Slow Query, TPS, **Replication Lag**
 | **Redis (Cache)** | `redis_exporter` | Memory Fragmentation, Hit/Miss Ratio, Evictions

- **분산 트레이싱 (APM 대체):** * 여러 마이크로서비스(Web -&gt; API GW -&gt; WAS -&gt; DB) 간의 요청 흐름을 추적하기 위해 **OpenTelemetry** 에이전트를 각 애플리케이션에 적용하고, **Tempo** 또는 **Jaeger** 백엔드로 데이터를 전송하여 Grafana에서 시각화합니다. (한국에서는 네이버가 만든 오픈소스인 **Pinpoint**도 Java/Node 환경에서 매우 훌륭한 대안입니다.)

**3. 로그 통합 모니터링 (Log Observability)**

도식화된 아키텍처 우측 하단에 **Cloud Log Analytics**가 명시되어 있습니다. 이를 적극 활용하거나, 별도의 로그 시스템을 구축해야 합니다.

- **클라우드 네이티브 활용:** VM과 컨테이너에서 발생하는 표준 출력(stdout) 및 파일 로그를 네이버 클라우드의 **Cloud Log Analytics** 에이전트를 통해 수집하여 통합 검색 및 알람을 구성합니다.
- **오픈소스 활용 (PLG Stack):** Prometheus 스택을 쓴다면, 각 VM에 **Promtail**을 설치하여 로그를 수집하고, **Loki** 중앙 서버로 전송한 뒤 Grafana에서 메트릭과 로그를 연동(Correlation)하여 트러블슈팅을 가속화합니다.

**4. 아키텍처 특화 필수 알람(Alert) 포인트**

아키텍처의 구성을 볼 때 다음 항목들은 반드시 알람(Slack, SMS, 이메일) 트리거로 설정해야 합니다.

1\. **Auto Failover 상태:** `rel-cdb master`에 장애가 발생하여 `standby`로 Failover 되는 이벤트는 최우선으로 감지되어야 합니다.

2\. **DB Replication Lag (복제 지연):** Read/Write가 분산되어 있으므로, Master와 Read Slave 간의 데이터 동기화 지연 시간(Lag)이 임계치를 초과하면 알람이 울려야 합니다.

3\. **NAT Gateway / Public LB 대역폭:** 모든 트래픽이 이 구간을 통과하므로, 클라우드 플랫폼에서 제공하는 **Cloud Insight**를 활용해 네트워크 병목(BPS/PPS) 및 5xx 에러율을 모니터링해야 합니다.

4\. **DR 존 연결 상태:** 장애 시 트래픽을 넘기기 위한 Global DNS와 DR 존 간의 헬스체크(Health Check) 상태를 상시 모니터링해야 합니다.

**💡 요약 및 추천:** 비용적 여유가 있고 빠른 구축과 직관적인 관리가 필요하다면 **[와탭 + Cloud Log Analytics]** 조합을 추천합니다. 반면, 인프라 제어권을 100% 가져가고 구성원들의 오픈소스 역량이 뛰어나다면 관리영역(MGMT) 서버 쪽에 **[Prometheus + Grafana + Loki]** 중앙 서버를 띄우고 각 타겟 VM에 Exporter를 배치하는 방식을 권장합니다.

