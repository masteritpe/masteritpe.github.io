---
layout: post
title: "WritingDrill_Rounds_10"
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

### [알고리즘] 알고리즘 시간복잡도 (Time Complexity)

**[정의]**

입력 크기 n에 따라 알고리즘이 수행하는 연산 횟수로 알고리즘의 수행시간 평가하는 척도

**[핵심/키워드]**

* 수행시간 평가, 컴파일+실행시간
* 접근법 : 빅오, 오메가, 세타
* 노테이션표기:O(1),oO(logon),oO(n),oO(nlogon),oO(n²)

### [CA/OS] 인터럽트(Interrupt)

**[정의]**

컴퓨터시스템 외부, 내부, SW적인 원인으로 CPU가 처리하던 프로그램을 중단하고 컴퓨터 제어를 특수사건이나 환경을 처리할 수 있도록 보내는 제어신호

**[핵심/키워드]**

전원 이상, 기계 착오, 외부 신호, 입출력, 프로그램 검사(트랩), SVC(SuperVisor Call)
 
 인터럽트 요청(IRQ), 인터럽트 처리루틴(IPR), 인터럽트 벡터, 인터럽트 서비스 루틴(ISR) 
 
 SW적 방식(폴링), 직렬연결(Daisy-Chain), 병렬연결(Multiple Interrupt)

### [알고리즘] Soline(솔린) 알고리즘

**[정의]**

각 단계에서 모든 정점을 연결하는 포리스트를 만들고 이를 연결하는 최소 신장 트리

**[핵심/키워드]**

1) 간선 중심 : 크루스칼 방식 
 2) 노드 중심 선택: 프림방식
3) 솔린 : 컴포넌트 중심

### [알고리즘] 퀵정렬 (Quick Sort)

**[정의]**

기준 값(피봇) 을 중심으로 작은 요소는 왼쪽, 큰 요소는 오른쪽으로 분할(partition) 하여
재귀적으로 정렬을 수행하는 알고리즘

**[핵심/키워드]**

* pivot, 분할과 정복
 * 시간복잡도 : O(n^2)
 * 공간복잡도 : O(log n)
 * pivot : 첫번째, 중간, 랜덤 선택

### [CA/OS] 교착상태(Deadlock)

**[정의]**

- 다중 프로그램 환경에서 두 개 이상의 프로세스가 서로 상대방의 자원을 요구하면서 양쪽 모두 작업 수행을 할 수 없는 대기상태

**[핵심/키워드]**

발생조건: 상점비환
① 상호배제② 점유와 대기
③ 비선점④ 환형대기
&lt;해결방안&gt;
① 예방 : 점유자원 해제 후 새 자원 요청
② 회피 : 은행가 알고리즘, Wait-Die/Wound-Wait
③ 발견 : 자원할당 그래프
④ 회복 : 프로세스 Kill, 자원선점

### [CA/OS] 프로세스(Process)

**[정의]**

메모리에 로드 되어 CPU에 의해 실행되고 있는 실행되고 있는 프로그램

**[핵심/키워드]**

프로그램 코드(텍스트), 데이터(전역/정적), 힙, 스택, 프로세스 제어 블록(PCB)

### [알고리즘] 비선형 자료구조 (Non Linear Data Structure)

**[정의]**

데이터가 계층적 또는 복잡하게 연결되어 있는 구조로 하나의 요소가 여러 요소와 관계를 가질 수 있는 형태

**[핵심/키워드]**

* 비선형, M : N, 다양한 관계 표현
 * 유형 : Tree, Graph

### [CA/OS] 뱅커스 알고리즘(Banker's Algorithm)

**[정의]**

교착상태 회피기법
-운영체제는 자원의 상태를 감시하고 사용자 프로세스는 사전에 자기작업에서 필요한 자원의 수를 제시하는 교착상태 회피 알고리즘

**[핵심/키워드]**

* 상태 
Safe: 모든 프로세스 할당가능 
UnSafe: 모든 프로세스 할당 불가
판단불가: 일부 프로세스만 할당 가능

### [알고리즘] 배열 리스트 (Array List)

**[정의]**

인덱스를 이용해 요소에 빠르게 접근할 수 있으며, 크기를 자동으로 조절하는 기능을 가질 수 있는 배열을 기반으로구현된 선형 자료구조

**[핵심/키워드]**

* 연속된 메모리 +자동 크기 확장
* 순차 저장, 동적 크기, 배열 + 리스트
* 특징 : 순차적 접근, 랜덤엑세스, O(1)

### [CA/OS] 우선순위 역전

**[정의]**

- 우선순위가 높은 타스크가 READY상태로 바뀌었지만,더 낮은 우선순위 타스크가 CPU를 점유하고 있어 실행되지 못하는 상태

**[핵심/키워드]**

* 원인 : 공유 자원 사용, 선점형 스케줄링, 중간 우선순위
태스크의 개입
*해결 : 우선순위 상속 , 우선순위 올림, 랜덤 부스팅

### [알고리즘] 트리정렬 (Tree Sort)

**[정의]**

데이터를 이진 탐색 트리에 삽입한 후,중위 순회(Inorder Traversal)를 통해 정렬된 결과를 얻는 비교 기반 정렬 알고리즘

**[핵심/키워드]**

* 비교 기반 정렬
*이진 탐색 트리 활용
*중위 순회
*불안정 정렬

### [알고리즘] 프림 (Prim) 알고리즘

**[정의]**

하나의 정점에서 시작하여 인접한 간선 중 가장 가중치가 작은 간선을 선택해 전체 정점을 연결하는 방식의최소 신장 트리 알고리즘

**[핵심/키워드]**

* 정점(V) 중심, 확장, 그리디(탐욕) 알고리즘
 * 절차 : 정점(V)선택, 최소비용간선(E), 트리추가, 반복
 * 사이클에 대한 탐지 불필요

### [CA/OS] Race Condition

**[정의]**

- 두 개 이상의 프로세스(또는 스레드) 가 동시에 같은 자원에 접근하거나 변경하려고 할 때, 수행 순서에 따라 결과가 달라지는 오류 상황
- 동시에 같은 자원을 두 개 이상의 프로세스가 경쟁적으로 사용하려는 상황

**[핵심/키워드]**

* 해결방안
① 상호배제(SW방법, HW방법)
② 동기화: 세마포어, 모니터, 스핀락

### [CA/OS] 스레싱(Thrashing)

**[정의]**

- 가상메모리에서 페이지 부재가 비정상적으로 많이 발생하여 페이지 교체에 따른 프로세스 처리가 급격히 저하되는 현상

**[핵심/키워드]**

* 발생원인 
- Locality 부족성(리소스 부족)CPU 성능부족, 저용량 메모리 
- 부적절한 페이지 교체: 요구기반 페이지, 페이지 교체문제 
- 과도한 멀티프로그래밍: 다중 프로세스, 할당 프로세스

### [CA/OS] 상호배제(Mutual Exclusive)

**[정의]**

- 둘 이상의 프로세스 또는 스레드가 공유 자원에 동시에 접근하지 못하도록 보장하는 원칙

**[핵심/키워드]**

* 경쟁조건 방지
* 충돌 방지
* 임계 영역 보호
* 성능 저하 가능성

### [알고리즘] 크루스칼 (Kruskal) 알고리즘

**[정의]**

그래프에서 간선을 가중치 오름차순으로 선택하여,사이클이 생기지 않도록 연결함으로써 최소 신장 트리를 구성하는알고리즘

**[핵심/키워드]**

*간선 중심(선택 기준)
*사이클 방지(조건)
* 정렬 기반(선행 과정)
*그리디 알고리즘

### [CA/OS] 세그먼테이션 오류(Segmentation Fault)

**[정의]**

- 프로그램이 운영체제로부터 할당 받지 않은 메모리 영역(예: NULL 포인터,해제된 메모리, 배열 범위 초과 등)에 접근하려 할 때 발생하는 오류

**[핵심/키워드]**

* 발생원인
잘못된 포인터참조
배열 인덱스오류
메모리 해제 오류

### [알고리즘] 최소신장트리(Minimal spanning tree) 알고리즘

**[정의]**

모든 정점을 포함하고 순환되지 않으면서 가중치의 합이 최소화가 되는 신장 트리

**[핵심/키워드]**

대표적인 MST 알고리즘
 - 크루스칼(Kruskal) 
 - 프림(Prim)

### [알고리즘] 다익스트라 (Dijkstra) 알고리즘

**[정의]**

양의 가중치 방향 그래프에서 하나의 출발 정점으로부터 모든 정점까지의 최단 경로를 구하는 알고리즘

**[핵심/키워드]**

* 최단경로, 그리디 알고리즘
 * 가중치 제약, 단일 출발점, 우선순위 큐 사용

### [CA/OS] 세마포어(Semaphores)

**[정의]**

- 공유 자원에 대한 접근을 제어하기 위해 사용되는 정수 기반 동기화 도구

**[핵심/키워드]**

초기화: s=1
P연산: s--, s=0
V연산: s++, s=1
유형 : 이진 세마포어, 카운터 세마포어

### [알고리즘] 동적계획법 (Dynamic Programming)

**[정의]**

복잡한 문제를 작은 부분 문제로 나누고, 그 결과를 저장하여 중복 계산을 피하는 최적화 알고리즘 기법

**[핵심/키워드]**

* 부분 → 전체, 
* 반복문제 , 한 번만 계산저장(memoization) 효율성 높임
 *Top-down(재귀 +메모이제이션)
* Bottom-up (반복문 기반 테이블 채우기)

### [알고리즘] Bellman-Ford 알고리즘

**[정의]**

모든 간선을 최대 (정점 수 - 1)번 반복하며, 음수 가중치를 허용하는 단일 출발점 최단 경로 알고리즘

**[핵심/키워드]**

* 음수 가중치 허용(음수 간선 처리 가능)
* 음수 사이클 탐지 가능(사이클 여부 확인)
* 모든 간선 반복(신뢰성 확보)

### [CA/OS] 뮤텍스(Mutex)

**[정의]**

- 하나의 쓰레드 또는 프로세스만 임계영역에 진입할 수 있도록 상호배제를 보장하는 락(Lock) 객체

**[핵심/키워드]**

* 소유 개념 있음
* 획득한 스레드만 해제 가능
* BusyWaiting없이 블로킹 기반 대기

### [알고리즘] 버블정렬 (Bubble Sort)

**[정의]**

인접한 두 개의 원소를 비교하여 서로 교환(swap)하는 방식을 반복적으로 수행하는 정렬 알고리즘

**[핵심/키워드]**

* 인접 비교
 * 시간복잡도 : O(N^2)
 * 공간복잡도 : O(1)

### [CA/OS] 스핀락

**[정의]**

락(Lock)이 해제될 때까지 CPU를 점유한 채 루프를 반복하며 기다리는 락 기법

**[핵심/키워드]**

- Busy Waiting(바쁜 대기) 일종
- 락부담이 적고 사용시간이 짧은 경우 사용

### [CA/OS] 교체정책

**[정의]**

제한된 공간을 가진 저장 장치에서 어떤 데이터를 제거할지를 결정하는 전략

**[핵심/키워드]**

- FIFO: 가장 먼저 들어온 페이지 교체
- LFU: 사용빈도가 가장 적은 페이지 교체
- LRU: 가장 오랫동안 사용되지 않은 페이지 교체
- OPT: 가장 오랫동안 사용되지 않을 페이지 교체

### [알고리즘] 문자열 탐색

**[정의]**

텍스트 문자열 안에서 주어진 패턴 문자열을 찾아내는 문제 또는 알고리즘

**[핵심/키워드]**

- 원시적 탐색 
 - 오토마타 매칭 
 - 카프-라빈 
 - KMP 
 - 보이어-무어

### [알고리즘] KMP(Knuth-Morris-Pratt) 탐색

**[정의]**

패턴의 접두사-접미사 정보를 미리 계산한 실패함수(π배열)을 이용해,불일치 시 비교를 되돌리지 않고 점프함으로써 선형 시간에 문자열을 탐색하는 알고리즘

**[핵심/키워드]**

* 접두사접미사 구조 활용
* 텍스트 인덱스 되돌림 없음
* 중복 비교 제거
* 패턴 전처리 기반

### [CA/OS] 단편화(Fragmentation)

**[정의]**

- 주기억 장치 상에서 프로그램에 의해 사용되지 못하고 낭비되는 부분적인 기억 공간을 의미

**[핵심/키워드]**

- 내부 단편화: 작업 할당후 남은 공간
- 외부 단편화: 분할이 작아 작업 할당이 불가한 공간

### [알고리즘] 카프-라빈 탐색

**[정의]**

해시 함수를 이용해 텍스트에서 패턴의 해시값과 같은 부분 문자열을 빠르게 탐색하는 알고리즘

**[핵심/키워드]**

* 빠른 후보 찾기
*롤링 해시 사용(이전해시로 다음해시 계산 )
*대규모 문자열 탐색에 유리

### [CA/OS] CXL(Compute eXpress Link)

**[정의]**

CPU와 연결된 다양한 가속기 장치 간의 통합 메모리공간, 고속 및 저지연 통신을 지원하기 위한 PCIe기반의 개방형 표준 인터커넥트 기술

**[핵심/키워드]**

*저지연 고대역폭 메모리 지원 
* CXL.io, CXL.cache, CXL.memory 
* Type1~Type3 
*CXL 1.0 ~ 3.0 (현재는 3.1 표준)

### [CA/OS] HBM(High Bandwidth Memory)

**[정의]**

고성능 데이터 처리를 위해 DRAM적층화 및 TSV배선 기반 데이터 이동 병목 현상을 해소한 DRAM적층형 고성능 메모리

**[핵심/키워드]**

HBM: 1세대, 4단 적층, 최대 128GB/s 대역폭
 HBM2: 대역폭, 속도 개선 (256GB/s 이상)
 HBM2E: 8단 적층, 고속화, 최대 460GB/s
 HBM3: 대역폭 800GB/s 이상, AI·HPC 최적화
 HBM3E: 향상된 속도(1TB/s 이상), 차세대 AI 모델 대응 
 
 3D TSV, 적층 DRAM, 인터포저, 폭넓은 I/O 채널, 저전력 설계, 고속 신호 처리 및 버퍼링 회로

### [알고리즘] AVL (Adelson-Velsky and Landis) Tree

**[정의]**

모든 노드에서 왼쪽과 오른쪽 서브트리의 높이 차이(BalanceFactor)가 1이하가 되도록 자동으로 균형을 맞추는 이진 탐색 트리(BST)의 확장 구조

**[핵심/키워드]**

* 좌우 1이하, balance factor, 자동균형
*시간 복잡도(삽입/삭제/탐색 : O(logn))
*회전 연산 존재(LL/LR/RL/RR)

### [CA/OS] 파이프라인 해저드

**[정의]**

- 파이프라인의 성능을 저해하는 요인
- CPI(Clock per Cycle)가 1이 되는것을 방해하는 요소

**[핵심/키워드]**

구조적, 데이터, 제어

### [알고리즘] 연결 리스트 (Linked List)

**[정의]**

데이터를 저장하는 노드들이 포인터를 통해 순차적으로 연결된 선형 자료구조

**[핵심/키워드]**

* 동적 확장(O(1)) 
* 삽입/삭제 유리(O(1))
* 접근 느림(O(n))
* 포인터 필요

### [알고리즘] 보이어무어 탐색

**[정의]**

패턴의 오른쪽부터 왼쪽으로 비교하면서,불일치 발생 시 두 가지 규칙(Bad Character,Good Suffix)을 이용해 패턴을 한 번에 여러 칸 건너뛰는 고속 문자열 검색 알고리즘

**[핵심/키워드]**

* 우측에서 왼쪽으로 비교
* 불일치 시 점프
* 탐색 효율 높음

### [CA/OS] DMA(Direct Memory Access)

**[정의]**

메모리 버퍼, 포인터, 카운터를 사용하여 장치 제어기가 CPU의 개입 없이 DMA컨트롤러를 이용하여 I/O 장치와 메모리 사이의 데이터를 전송하는 입출력 방식

**[핵심/키워드]**

* 인터럽트 최소화, 데이터 직접 전송
*동작모드 : 버스트모드 Burst Mode, 싸이클스틸링Cycle Stealing Mode , 인터리브드(Interleaved)

### [CA/OS] 서버 가상화(Virtualization)

**[정의]**

서버의 물리적 자원(CPU,메모리,Disk등)들을 논리적 통합하여,하나의 서버를 통해 서비스를 받는 것처럼
느껴지게 하는 기술

**[핵심/키워드]**

*(온디맨드,실시간성,확장성,멀티터넌시)
 
 *하이퍼바이저 가상화(Type-1), 전가상화(Type-1), 반가상화(Type-1), OS 레벨 가상화(Type-2)

### [알고리즘] 백트래킹(Backtracking)

**[정의]**

가능한 모든 경우를 탐색하면서 조건에 맞지 않으면 즉시 되돌아가는(가지치기) 방식의 완전 탐색 알고리즘

**[핵심/키워드]**

N-Queen 문제
스도쿠(Sudoku) 풀이

### [CA/OS] 하이퍼컨버지드(Hyper-Converged)

**[정의]**

서버, 스토리지, 네트워크, 가상화 기능을 하나의 통합 시스템으로 구성한 소프트웨어 중심 통합 어플라이언스에 SDDC 합쳐진 개념

**[핵심/키워드]**

*SDDS (Software Defined Data Center) 
* 유연성,확장성,자동화

### [CA/OS] NW Storage(Network Storage)

**[정의]**

다양한 NW기반 환경을 이용하여 데이터의 입출력 및 스토리지를 관리하는 기술

**[핵심/키워드]**

DAS, NAS, SAN, IP-SAN

### [알고리즘] 분할정복알고리즘(Divide and Conquer)

**[정의]**

큰 문제를 작은 부분 문제로 나눈 뒤,각 부분을 독립적으로 해결하고,그 결과를 합쳐서 전체 문제를 해결하는 기법

**[핵심/키워드]**

① 분할(Divide)
② 정복(Conquer)
③ 결합(Combine)

### [CA/OS] 무어의 법칙

**[정의]**

마이크로프로세서의 집적도는 18개월마다 2배씩 증가함을 증명한 이론

**[핵심/키워드]**

* 모어 댄 무어(More than Moore)
:  전통적인 무어의 법칙(Moore’s Law) 한계를 인식하고, 트랜지스터의 집적도 외적인 기술 확장을 통해 반도체의 성능과 기능을 향상시키는 패러다임

### [알고리즘] R-Tree (Rectangle Tree)

**[정의]**

점, 선, 면, 도형 등 다양한 다차원 공간 데이타 객체를 저장하고 검색하기 위한 다차원 인덱스 구조

**[핵심/키워드]**

* 완전 균형 트리
* MBR을 계산 , Entry로 저장

### [알고리즘] Red-Black Tree

**[정의]**

균형 유지를 위해 노드에 색상(레드 또는 블랙)을 추가하여 동작하는 자기 균형 이진 탐색 트리(Self-Balancing Binary Search Tree)

**[핵심/키워드]**

* 데이터의 삽입 및 삭제 시 트리의 균형을 유지하여 탐색, 삽입, 삭제 시 모두 시간 복잡도 O(log n)를 보장

### [CA/OS] RAID(Redundant Array of Independent Disks)

**[정의]**

처리속도, 데이터 보호를 목적으로 여러 DISK를 중복성을 가진 하나의 논리적인 Disk(Array)로 변환하는 저장 장치

**[핵심/키워드]**

RAID 0(스트라이핑, 성능↑), RAID 1(미러링, 복구용이), RAID 2(비트 단위 ECC, 거의 사용 안함), RAID 3(패리티+바이트 단위 분산), RAID 4(고정 패리티 디스크), RAID 5(분산 패리티, 성능·복구 균형), RAID 6(이중 패리티, 복구 안정성↑), RAID 0+1(성능+미러, 성능 위주), RAID 1+0(미러+성능, 복구 위주)

### [CA/OS] TLB(Translation Look-aside Buffer)

**[정의]**

가상 주소를 물리 주소로 변환할 때 사용하는 페이지 테이블 접근 시간을 줄이기 위한 고속 캐시 메모리

**[핵심/키워드]**

MMU 내에 위치, 
 TLB에서 해당 가상 페이지 번호 검색
 TLB Hit → 물리 주소 바로 반환
 TLB Miss → 페이지 테이블 접근 후 TLB에 캐싱 
 Page Fault -→ 디스크에서 메모리로 로딩

### [CA/OS] MMU(MemoryManagementUnit)

**[정의]**

- 프로그램 상의 논리적 주소를 실제 물리적 주소로 변환하여 실행시키는 장치

**[핵심/키워드]**

- TLB가 없으면 MMU는 메모리에 항상 두 번 접근(TLB는 MMU의 속도 향상을 위한 구성요소)

### [CA/OS] Wait-Die 기법

**[정의]**

타임스탬프 기반으로 먼저 시작한 트랜잭션(노인)이 기다릴 수 있고, 늦게 시작한 트랜잭션(청년)은 강제 종료(die)시키는 교착상태 회피 기법

**[핵심/키워드]**

*비선점 방식 
*간단한 구현
* 타임스탬프(시작 시각) 기준

### [CA/OS] Wound-Wait 기법

**[정의]**

타임스탬프 기반으로 먼저 시작한 트랜잭션이 늦게 시작한 트랜잭션을 강제 종료(wound)하고 자원을 선점하는 교착상태 회피 기법

**[핵심/키워드]**

*선점 방식
 *타임스탬프 큰 트랜잭션만 대기 허용
 *교착 상태 방지

### [알고리즘] 위상정렬(Topological Sort)

**[정의]**

- 방향 그래프(Directed Graph)에서 정점들을 선후 관계(순서)를 고려해 나열하는 방식

**[핵심/키워드]**

- 진입차수 0인 노드부터 모든 간선이 제거될 때까지 수행 
- 깊이 우선(DFS) 기반

### [CA/OS] 캐시메모리(Cache Memory)

**[정의]**

CPU와 주기억장치의 속도 차이 따른 성능저하를 줄이기 위해, CPU와 주기억장치 사이에 설치한 고속 기억장치

**[핵심/키워드]**

사상(mapping) , 교체(replacement), 쓰기정책, 캐시일관성

### [CA/OS] Round Robin

**[정의]**

모든 프로세스에 동일한 시간 할당량(Time Quantum,Time Slice)을 순서대로 부여하여,타임슬라이스가 끝나면 강제로 CPU를 회수하고 다음 프로세스에게 넘기는 선점형 스케줄링 방식

**[핵심/키워드]**

시간 할당량 기반 분할
선점형 스케줄링
공정성 보장
문맥 교환 증가

### [CA/OS] 멀티 스레드 (MultiThread)

**[정의]**

하나의 프로세스 내에서 여러 실행 흐름(스레드)을 동시에 수행하는 방식

**[핵심/키워드]**

- 병렬 처리 가능(멀티코어 동시 실행),응답성 향상(UI/서버 지연 최소화),메모리 공유(자원 복사 없이 빠른 접근),
- 컨텍스트 스위칭 빠름(전환 효율 높음),경량 구조(적은 비용 다수 스레드 운영),동기화 필요(충돌 방지 관리 )

### [CA/OS] 커널(Kernel)

**[정의]**

운영체제의 핵심 (Core)으로,하드웨어 자원 직접 제어하고,  시스템 기능을 직접 관리하는 소프트웨어

**[핵심/키워드]**

- CPU,메모리,파일,장치 등 자원 직접 제어
-  시스템 호출 처리 
- 보안 및 보호 기능 수행

### [CA/OS] TCB(Thread Control Block)

**[정의]**

- 스레드의 상태,실행 정보,자원 포인터 등을 저장하는 커널 공간의 제어 블록

**[핵심/키워드]**

- 운영체제가 스레드를 스케줄링하고 관리하기 위해 사용하는 핵심 자료구조
- TCB정보 (스레드 ID, 스레드 레지스터, 상태) , 커널영역, 사용자 영역으로 구성

### [알고리즘] 그리디 알고리즘 (Greedy Algorithm)

**[정의]**

특정 순간 최적해를 구하기 위해 최적성과 효율성 개선을 통해 최적의 해를 도출하는 알고리즘

**[핵심/키워드]**

탐욕 선택 속성(Greedy Choice Property)
최적 부분 구조(Optimal Substructure):

### [알고리즘] 다차원 검색 트리

**[정의]**

공간 정보의 다차원 자료화를 위해 복수 필드를 동시에 키로 사용하는 파일

**[핵심/키워드]**

* 다차원 자료, 복수 키, 공간질의
 * 유형 : PAM, SAM
 * PAM : K-D tree, Quad tree
 * SAM : R tree, R+ tree, R* tree
 * Pivot : VP tree, M tree

### [알고리즘] Quad Tree

**[정의]**

- 2차원 공간을 4개의 사분면(quadrant)으로 재귀적 분할하여 표현하는 트리 기반 자료구조

**[핵심/키워드]**

* 2차원 공간 분할
* 고속 탐색
* 공간 효율성
* 유연한 구조
* 다양한 활용

### [알고리즘] 다중 연결 리스트 (Multi-Linked list)

**[정의]**

양방향 및 다중 방향 검색이 가능하도록 선행 노드 포인터 크기를 유연하게 변경 가능한 연결 리스트

**[핵심/키워드]**

- 하나의 노드에 2개 이상 포인터 존재(서로 다른방향/기준으로 연결)
- 2차원/다차원 연결 구조 표현
- 희소 행렬,분류 트리,2D리스트

