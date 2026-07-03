---
layout: post
title: "WritingDrill_Rounds_4"
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

### [데이터베이스] 데이터 품질 인증제도(DQ인증)

**[정의]**

- 과학기술정보통신부가 지정한 데이터 품질 인증기관이 ①데이터 내용, ②데이터 관리체계를 진단하고 수준을 평가해 품질을 인증하는 제도
 &lt;관련법령&gt;:「데이터 산업진흥 및 이용촉진에 관한 기본법」제20조 

 - DQC인증은 2022년 폐지. 2023년 DQ인증제도로 공식 전환
 - DQ인증은 '데이터 내용 + 관리체계' 품질 인증으로 확대 및 구체화

**[핵심/키워드]**

* 인증대상
  - 데이터 내용 : 데이터 내용 및 구조 (정형, 비정형, 반정형, AI학습용) 
  - 데이터 관리체계 : 프로세스, 인력, 조직, 기술 등 관리체계의 성숙도 평가
 
* 심사 내용 
  - 데이터 내용 :  완전성, 유효성, 일관성, 정확성, 접근성, 유일성
  - 데이터 관리 체계 : 
    ㄴ  Plan(계획), Do(통제), Check(보증), Act(개선), 정보 및 기술, 지원 제공 프로세스, 지원 및 교육
 
* 인증 등급 
  - 데이터 내용 :  
    ㄴ 구조 유형 : Complex-Type,  Normal-Type, Simple-Type
    ㄴ 내용 : A Class(99%), B Class(97%), C Class(95%)
  - 데이터 관리 체계 :  혁신화, 예측화, 체계화, 관리, 도입(인증안함)

### [데이터베이스] Database

**[정의]**

여러 사용자와 응용 시스템이 공유할 수 있도록 조직적으로 통합하여 저장·관리하는 데이터의 집합체

**[핵심/키워드]**

- 특징 : 통합성,저장성, 운영성, 공용성, + 실시간 접근성, 무결성 유지

### [데이터베이스] 몽고DB(MongoDB)

**[정의]**

문서(Document) 지향 NoSQL 데이터베이스로, JSON 유사 구조의 데이터를 유연하게 저장하며 스키마 없이 동적 구조를 지원하는 고성능 DB

**[핵심/키워드]**

Application / Driver, mongos

 mongod (Shard), Shard Key
 └─ datastore
 └─ oplog (Primary만) 

 Replica Set, mongod (Config Server)

### [데이터베이스] 레디스(Redis)

**[정의]**

Key-Value 구조의 인메모리 데이터 저장소로, 빠른 속도와 다양한 자료구조를 지원하는 오픈소스 NoSQL 데이터베이스

**[핵심/키워드]**

- 활용 : 캐시, 세션관리, 순위, Pub/Sub, 메시지 큐 

- Redis Server, Client, RDB(Auto Save) 또는 AOF(Append Only File)
 Replication, Sentinel, Cluster

### [데이터베이스] NoSQL 모델링 패턴

**[정의]**

전통적 관계형 모델과 달리 분산 처리, 비정형 데이터에 최적화된 방식 적용하여, 스키마 유연성과 확장성을 고려해 데이터 구조를 효율적으로 설계하는 기법

**[핵심/키워드]**

Denormalization(반정규화), Aggregation
 (집계 기반 구조), Application Side Join (클라이언트 측 조인)
 , Atomic Aggregation, (원자성 집계), Index Table(인덱스 테이블)
 , Composite Key Table(복합 키 테이블)

### [데이터베이스] ISO/IEC 11179(Metadata Registry

**[정의]**

데이터의 의미와 구조를 명확히 정의하여 데이터 공유와 상호운용성 확보하기 위해 메타데이터를 정의하고 관리하기 위한 원칙과 구조를 제공하는 표준

**[핵심/키워드]**

- 주요원칙 : 정확성 (Accuracy), 일관성 (Consistency)
 확장성 (Extensibility)  

 - 파트구성 : Framework(프레임워크), Classification
 (분류), Registry Metamodel, (레지스트리 메타모델)
 Data Definitions(데이터 정의), Naming and Identification
 (명명 및 식별), Registration(등록), Data Set Registration
 (데이터셋 등록)

### [데이터베이스] 데이터 아키텍처(Data Architecture)

**[정의]**

조직의 데이터를 전사적 관점에서 통합·관리·활용하기 위해 데이터의 구조, 표준, 흐름, 저장 방식 등을 정의하고 설계하는 체계

**[핵심/키워드]**

Data Principle
DA Framework
DRM(Data Reference Model)
Data Governance

### [데이터베이스] 오브젝트 스토리지 (Object Storage)

**[정의]**

대용량 비정형 데이터(이미지, 영상, 로그 등) 저장에 최적화 되어, 데이터를 파일 단위가 아닌 오브젝트 단위(데이터 + 메타데이터 + 고유 식별자로 )로 저장하는 스토리지 방식

**[핵심/키워드]**

&lt;주요 기능&gt; 
  - 오브젝트 검색(빠른 식별자 검색), 버전 관리(이전 복구), 수명 주기 정책(자동화된 데이터 관리), 
  - 접근 제어(보안 강화), 다중 리전 복제(재해 복구 대비), 로깅/모니터링(감사 추적

### [데이터베이스] R Tree

**[정의]**

N차원의 공간 데이터를 효과적으로 저장하고 지리정보와 관련된 질의를 빠르게 수행 할 수 있는 자료 구조

**[핵심/키워드]**

- SAM, MBR 
- 질의 방법 : 교차 질의 (Intersection), 포함 질의 (Containment), 근접 이웃 질의 (Nearest Neighbor)
 - R+Tree, R*Tree

### [데이터베이스] 비트맵(Bitmap) 인덱스

**[정의]**

컬럼의 각 값에 대해 비트 벡터를 만들어, 해당 값이 존재하는 행의 위치를 비트로 표시하는 인덱스 방식

**[핵심/키워드]**

낮은 분포도, 빠른 AND/OR연산, 컬럼 값(Key Value), 

ROWID 목록, 비트맵(Bitmap), 인덱스 블록, 인덱스 헤더, 비트 연산기

### [데이터베이스] B* TREE

**[정의]**

B-Tree의 공간 낭비 및 과도한 분할·병합 연산 문제와, B+Tree의 탐색 효율성은 유지하면서 중복 키 문제를 개선한 고성능 인덱스 구조

**[핵심/키워드]**

분할 (Split), 차용 (Borrow / 재분배), 병합 (Merge), 분산 (Redistribute), 최소 2/3 이상 채움(분할 후 노드 채움율)

### [데이터베이스] 선형 해싱 (Linear Hashing)

**[정의]**

디렉토리 없이, 데이터 삽입이 늘어날수록 버킷을 순차적으로 하나씩 분할하며 확장하는 방식

**[핵심/키워드]**

동적해싱, 확장해싱, 버킷 (Bucket),
 오버플로우 영역(Overflow Area),
 분할 포인터 n(Next Split),버킷 수 M
 ,초기 해시 함수 h(k),보조 해시 함수 h′(k),
 분할 (Split),재해시 (Rehash),확장 (Expansion),
 해시 테이블,(Hash Table)

### [데이터베이스] 파티셔닝(Partitioning, 분할, 파티션 분할)

**[정의]**

하나의 테이블이나 인덱스를 물리적으로 여러 개의 작은 단위(파티션)로 나누어 저장하고 관리하는 기법으로, 데이터 양이 많을 때 성능 향상과 관리 효율을 높이기 위한 데이터베이스 구조 최적화 방식

**[핵심/키워드]**

수직/ 수평 분할(샤딩) 

범위 분할 (Range Partitioning)
목록 분할 (List Partitioning),
해시 분할 (Hash Partitioning)
복합 분할(Composite Partition - Range + Hash), 
복합 분할(Composite Partition - Range + List)

### [데이터베이스] 다중버전 동시성 제어(MVCC: Multi-Version Concurrency Control)

**[정의]**

데이터의 여러 버전(복사본)을 생성하여 관리함으로써, 읽기 작업은 이전 버전, 쓰기 작업은 새로운 버전에 접근하도록 하여 락 없이도 트랜잭션 간 동시성과 일관성을 유지하는 동시성 제어 기법

**[핵심/키워드]**

병행제어, 동시성, 
&lt;종류&gt; 
- 버전 체이닝 방식(이전 값 저장) : 이력을 체인 형태로 연결, 트랜잭션 ID(TXID)
- Undo 기반 방식(Rollback Segment/Undo) : SCN(System Change Number
    ㄴ SCN, 스냅샷투올드에러, Undo 크기 조정

### [데이터베이스] 락(Locking)

**[정의]**

트랜잭션이 데이터베이스 객체(예: 레코드, 테이블, 페이지 등)에 동시에 접근하는 것을 제어하기 위해 Lock(잠금)을 설정하여, 데이터의 일관성과 무결성을 보장하는 동시성 제어 기법

**[핵심/키워드]**

- 특징 : 교착 상태/가아/연쇄 복귀 발생 가능, 락 단위(DB, 테이블, .. 속성), 
- 공유락, 배타락, 락 양립성, 비관적/낙관적 락, 2PL(비관)

### [데이터베이스] 그림자페이지(Shadow Paging)

**[정의]**

데이터를 직접 수정하지 않고, 새로운 페이지를 생성한 후 교체하는 방식으로 장애 발생 시 자동 복구가 가능한 회복 기법

**[핵심/키워드]**

현재 페이지 테이블(Current Page Table), 그림자 페이지 테이블 (Shadow Page Table), 
 장애 발생 시 (복구 과정) : 현재 테이블 삭제(메모리), 그림자 테이블 -→ 현재 테이블

### [데이터베이스] 팬텀 리드(Phantom Read)

**[정의]**

데이터 베이스 조회 시, 동일한 쿼리를 반복 실행할 때 결과가 달라지는 현상(트랜잭션 병행제어의 문제점)

**[핵심/키워드]**

원인 : 다른 트랜잭션이 데이터 삽입/삭제 
 현상 : 잘못 된 데이터 조회 
 해결 : Repeatable Read 또는 Serializable 격리 수준 적용

### [데이터베이스] 이력 데이터 모델링

**[정의]**

데이터의 변경 이력을 관리하기 위한 모델링 기법으로, 데이터가 특정 시점 또는 기간별로 어떻게 변경되었는지를 저장하고 추적하는 데이터 모델링 기법

**[핵심/키워드]**

변경이력, 데이터 무결성 
 변경/발생/진행, 시점/선분, 내부스냅샷 이력/ 1:M 스냅샷 전체 이력/ 1:M 스냅샷 과거 이력/
 1:M 스냅샷 군집 전체 이력/ 1:M 스냅샷 군집과거 이력

### [데이터베이스] CRUD Matrix

**[정의]**

데이터(Entity)와 프로세스(Process) 간의 관계를 분석하는 매트릭스로, 특정 프로세스가 데이터에 대해 수행하는 C(Create), R(Read), U(Update), D(Delete) 작업을 명확히 정의하는 방법

**[핵심/키워드]**

상관모델링, 엔터티, 프로세스 

 &lt;검증&gt; 
  - 엔터티 : 모든 Entity Type에 CRUD가 한 번 이상 표기,
 모든 Entity Type에 “C”가 한 번 이상 존재하는가,
 모든 Entity Type에 “R”이 한 번 이상 존재하는가
  - 프로세스 : 모든 단위 프로세스는 하나 이상의 Entity Type에 표기,
 두 개 이상의 단위 프로세스가 하나의 Entity Type을 생성

### [데이터베이스] 제4차 정규화

**[정의]**

한 관계에 둘 이상의 독립적 다중값 속성이 존재하여 릴레이션을 분해하는 과정

**[핵심/키워드]**

- 다치 종속성 : 각각 여러 값을 독립적으로 갖는 상황(다중값)을 분리 
- 삽입이상, 사원번호/기술코드/프로젝트 코드, 
 - 관계있는 속성끼리 분리 후 테이블 생성

### [데이터베이스] BCNF(Boyce-Codd Normal Form)

**[정의]**

일반속성이 결정자 속성을 결정하는 상황인 결정자 함수종석성을 제거하여 모든 결정자가 후보키가 되도록 정규화하는 과정

**[핵심/키워드]**

강한 제3정규화(Strong 3NF) 
 고객아이디, 인터넷 강좌 -→ 담당강사번호 
 담당강사번호 -→ 인터넷 강좌 
 &lt;결과&gt; 
 - 고객아이디, 담당강사번호 
 - 담당강사번호, 인터넷 강좌

### [데이터베이스] 암스트롱 공리(Armstrong’s rules)

**[정의]**

데이터베이스 정규화 과정에서 속성 간의 관계를 유도할 때, 함수종속의 성질을 유도해 낼 수 있는 추론 규칙

**[핵심/키워드]**

- 함수적 종속성, 정규화, 정당/완전
- 추론규칙 : 재귀/증가/이행/연합/분해/가이행 
- 페포

### [데이터베이스] 슈퍼/서브 타입(Super/Sub Type)

**[정의]**

엔티티의 작성 시 대부분의 속성이 비슷하고 일부만 다른 여러 엔티티들을 하나로 묶어 통합하는 경우 수행하는 확장형 데이터모델링

**[핵심/키워드]**

조건 : 서브타입간 상호 배타, 구분자 필요 

- 슈퍼/서브타입, 통합/세분화, 상화배타/중첩 
 - OneToOne Type(Identity), Plus Type(Rolldown), Single Type(Rollup)

### [데이터베이스] 자기참조 관계(Self-Referencing Relationship)

**[정의]**

계층형 데이터 모델링을 위해, 동일 Entity 타입 내에서 자기가 자신의 인스턴스를 참조하는 구조 및 모델링 기법

**[핵심/키워드]**

- 재귀적(계층형) 구조, 1차 정규화 대상, 
-  1:1  자기참조관계, 1:M 자기참조관계, M:N자기참조관계 
- N:M 해소 : 엔터티 타입 분리, 주식별자 통합, 병렬 관계

### [데이터베이스] 개념적 모델링(Conceptual Modeling)

**[정의]**

조직의 비즈니스 요구사항과 핵심 프로세스를 반영하여 실제 업무 환경에서 발생하는 주제영역, 핵심데이터 집합과 관계를 추상화하는 작업

**[핵심/키워드]**

1\. 주제영역 선정
 1\. 핵심 데이터 집합 선정 (Entity 도출)
 2\. 관계 설정 (Cardinality 정의)
 3\. 핵심 속성 정의 (Attribute 식별)
 4\. 식별자 정의 (Identifier 설정)

### [데이터베이스] 정적SQL(Static SQL)

**[정의]**

실행 시점에 변경되지 않는 고정된 SQL 문으로, 실행 계획이 사전에 결정되어 있어 효율적이고 성능이 최적화된 SQL

**[핵심/키워드]**

컴파일 된 SQL, 권한확인/접근경로계산/임시 저장계획 사용/SQL실행 
 소프트파싱

### [데이터베이스] 데이터 제어어(DCL: Data Control Language)

**[정의]**

여러 사용자가 무결성과 일관성을 유지하며 문제없이 공유할 수 있도록, 내부적으로 필요한 규칙이나 기법을 정의하는 데 사용하는 데이터 언어(무결성, 보안, 회복, 동시성 보장

**[핵심/키워드]**

TCL : COMMIT,ROLLBACK,SAVEPOINT 
 DCL : GRANT, REVOKE

### [데이터베이스] 관계해석

**[정의]**

E.F. Codd가 제안한 프레디킷 해석(Predicate Calculus, 논리식 기반의 수학적 표현)에 기초한 데이터 질의 방식이며, 원하는 데이터(What)를 명시하는 비절차적(Declarative) 언어

**[핵심/키워드]**

- 튜플 관계 해석(Tuple Relational Calculus, TRC) 
  ㄴ 튜플(행) 단위로 
- 도메인 관계 해석(Domain Relational Calculus, DRC) 
   ㄴ 개별 속성(컬럼) 값의 조건을 기반  

&lt;표기법&gt; 
- 연산자: OR 연산(∨), AND 연산(∧), NOT 연산(¬)
- 정량자: 전칭 정량자(∀), 존재 정량자(∃)

### [데이터베이스] 트리거(Trigger)

**[정의]**

특정 이벤트(INSERT, UPDATE, DELETE 등)가 발생할 때 자동으로 실행되는 데이터베이스 객체

**[핵심/키워드]**

&lt;유형&gt; 
 BEFORE 트리거
 AFTER 트리거
 INSTEAD OF 트리거
 행(Row) 수준 트리거
 문장(Statement) 수준 트리거 
 &lt;작성 규칙&gt; 
 이벤트(Event)
 조건(Condition)
 액션(Action)
 트리거 시점(Timing)
 대상(Table or View)

### [데이터베이스] 무결성 제약조건(Integrity Constraints)

**[정의]**

잘못된 데이터 입력이나 조작을 방지하여 데이터의 신뢰성을 보장하기 위해, 일관성과 정확성을 유지하기 위해 적용하는 규칙

**[핵심/키워드]**

도메인 무결성, 릴레이션 무결성

### [빅데이터 분석] 교차표분석

**[정의]**

두 범주형 변수간의 연관관계를 볼때 교차표(분할표)를 작성하여 변수들간 관계를 분석하는 기법

**[핵심/키워드]**

- 적합도 검정 , 독립성 검정, 동질성 검정 
 - 승산비 , 상대위험도(Relative Risk)

### [빅데이터 분석] 탐색적 데이터 분석(EDA, Exploratory Data Analysis)

**[정의]**

데이터 분석과정에서 수집된 데이터 입력 시 데이터의 구조, 특성, 패턴 등 넓은 시각에서 직관적으로 이해 및 관찰한 후 연구자의 가설 수립을 위한 분석 기법

**[핵심/키워드]**

1) 저항성 
 2) 잔차의 해석 
 3) 데이터의 재표현 
 4) 데이터의 현시성

### [빅데이터 분석] 회귀분석

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

### [빅데이터 분석] ANOVA/분산분석 (Analysis Of Variance)

**[정의]**

독립집단 3개 이상의 집단간 평균이 서로 차이가 있는지 확인하기 위한 검정 방법

**[핵심/키워드]**

* 통계량 : f =  MSE/MSE 
* 일원 분산분석, 이원 분산분석, 반복측정분산분석, 이원반복측정분산분석 

사후검정 
 - 튜키 HSD, 쉐페, 던칸, 본페로니, 피셔LSD

### [빅데이터 분석] 베이즈 정리

**[정의]**

사전적 확률을 구한후 확률에 영향을 미치는 변수의 확률을 반영하여 사후 확률을 구하는 방법 

𝑃(𝐴1|𝐵)=  P(B|A1)P(A1)/P(B) = (𝑃(𝐴1∩𝐵) / 𝑃(𝐵)

**[핵심/키워드]**

사전확률, 조건부확률, 사후확률
 확률의 곱셈법칙
 전확률, 확률계산, 베이즈 정리

### [빅데이터 분석] 모수통계, 비모수통계

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

### [빅데이터 분석] 연관규칙(Association Rule)

**[정의]**

특정사건들이 동시에 발생하는 빈도로 상호간의 연관성을 표현하는 규칙

**[핵심/키워드]**

지지도 
신뢰도 
향상도(Lift)

### [빅데이터 분석] 유클리디안 거리 (Euclidean Distance)

**[정의]**

벡터 공간 내 두 노드 사이의 직선 거리를 이용하여 유사도를 산출하는 벡터 거리 기반 유사도 측정법

### [빅데이터 분석] 벡터 데이터베이스 (Vector Database)

**[정의]**

대량의 고차원 데이터 저장 및 조회 위해 컨텐츠 벡터 임베딩 및 쿼리 벡터 유사도 비교 기반 신속하게 인덱싱하는 데이터베이스

**[핵심/키워드]**

- 임베딩 벡터, 벡터 인덱스(ANN : HNSW, IVF, PQ등), 저장 엔진, 유사도 함수, 메타데이터 저장소

### [빅데이터 분석] 상관관계 분석

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

### [빅데이터 분석] 데이터 거버넌스 (Data Governance)

**[정의]**

데이터 자산을 관리하고 활용하기 위한 정책, 프로세스, 표준, 역할 및 책임을 정의하고 실행하는 체계

**[핵심/키워드]**

* 분석 관리 체계
 * 대상 : 마스터데이터, 메타데이터, 데이터사전, 빅브라더
 * 구성 : 원칙, 조직, 프로세스
 * 체계 : 표준화, 관라체계, 저장소 관리, 관리활동

### [빅데이터 분석] 카프카(kafka)

**[정의]**

- 실시간 데이터 처리, 비동기 메시징, 데이터 파이프라인 구축을 위해 사용되는 고성능 메시지 브로커 

- 브로커 중심의 단일 계층 구조 
 
Kafka → 고성능 스트리밍 처리에 강점, 구조 단순하지만 확장 시 관리 복잡.
Pulsar → 저장 분리형 구조로 내구성·확장성 우수, 멀티테넌시·큐/스트림 통합 환경에 적합.(브로커와 BookKeeper가 분리)

**[핵심/키워드]**

* 발행, 구독 중심, 분산구조, 실시간처리 

* 구성 :producer, broker, message, topic, partition, consumer, offset, zookeeper 

- 데이터 모델  : 토픽, 파티션

### [빅데이터 분석] 판다스(pandas)

**[정의]**

데이터조작과 분석을 위한 오픈소스 라이브러리로서 데이터 처리와 구조화된 데이터를 다루는데 최적화된 도구

**[핵심/키워드]**

* 파이썬, 데이터 처리 및 구조, 
 * 구조 : 시리즈, 데이터 프레임
 * 기능 : 결측값처리, 데이터 필터링, 다양한 형식, 시계열 데이터, 넘파이 통합

### [빅데이터 분석] CRISP-DM (Cross-Industry Standard Process for Data Mining)

**[정의]**

1996년 다수의 기업(IBM, Daimler 등)이 공동 개발한 4개의 프로세스 모델을 적용하여 6단계로 데이터 마이닝을 분석할 수 있는 방법론

**[핵심/키워드]**

* 6단계 분석 방법론
 * 4개 프로세스 : 최상위, 일반화, 세분화, 프로세스
 * 6단계 : 업무이해, 데이터이해, 데이터준비, 모델링, 평가, 배포

### [빅데이터 분석] 독립표본 t-검정  (Independent t-test)

**[정의]**

두 개의 독립적인 집단 간의 평균 차이를 검정하기 위한 통계적 방법 

- 서로 독립인 두 모집단의 모분산이 알려져 있지 않고, 두 모집단의 각각의 표본 크기 작은 경우(또는 𝑛1, 𝑛2<30) 𝑡분포를 이용하여 검정 하는 방법

* 가정사항 : 독립성, 정규성, 등분산성
 - 서로 다른 두 집단 간 t-검정
 - 두 집단이 같은 모집단에서 나왔는지를 평균값을 기준으로 비교하는 가설검정 방법 


<둥분산, 이분산 에 따라 통계량 산정 방법 상이>

### [빅데이터 분석] 대응표본 t-검정  (Paired t-test)

**[정의]**

같은 집단에서 두 번 측정된 값(또는 짝지어진 두 집단 : 이전 이후)의 평균 차이를 비교하는 통계적 검정 방법 

* 가정사항 : 정규성
 * 하나의 모집단 내부 두 집단 간 t-검정

### [빅데이터 분석] 재현 데이터 (Synthetic Data)

**[정의]**

실제 데이터를 분석한 결과와 유사한 결과를 얻을 수 있도록 인공적으로 재현하여 생성한 가상데이터

**[핵심/키워드]**

* 가상 데이터, 실제 데이터 유사
 * 유형 : 완전, 부분, 하이브리드
 * 생성기법 : 베이지안, 기계학습, 차등정보보호기반
 * 절차 : 원본수집, 기법적용, 합성데이터확보, 유용성 평가, 익명성 평가, 활용

### [빅데이터 분석] 데이터 레이크 (Data Lake)

**[정의]**

대규모의 다양한 원시 데이터 세트를 기본 형식으로 저장하는 데이터 레파지토리

**[핵심/키워드]**

* 대규모 데이터, 다양한 형태, schema-on-read
 * 절차 : 수집, 조직, 분석, 제공
 * 계층 : raw, processed, curated

### [빅데이터 분석] 데이터 메시 (Data Mesh)

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

### [빅데이터 분석] 결측값 (Missing Value)

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

### [빅데이터 분석] 차원축소 (Dimensionality Reduction)

**[정의]**

- 고차원 데이터에서 중복되거나 불필요한 변수(특징)를 제거하고, 데이터의 본질적인 구조를 유지하면서 저차원 공간으로 변환하는 과정.

**[핵심/키워드]**

* 특성 축소, 성능 유지
 * 유형 : 피처 선택, 피처 추출
 * 기법 : 주성분분석, 요인분석, 특이값분해, 다차원척도법, 판별분석, t-SNE

### [빅데이터 분석] 불균형 데이터 (Imbalanced Data)

**[정의]**

각 변수가 가진 데이터에서 각 집단에 속하는 데이터의 수가 동일하지 않은 상태의 데이터

**[핵심/키워드]**

* 집단간 데이터 불균형
 * 해결 : 오버샘플링, 언더샘플링
 * 오버샘플링 : 랜덤, 스모트, 보더라인 스모트, 아다신
 * 언더샘플링 : 랜덤, 토멕링크, CNN, OSS

### [빅데이터 분석] 산포도 (Dispersion)

**[정의]**

데이터가 중심경항치를 중심으로 얼마나 밀집되어 있거나 흩어져 있는지를 나타내는 척도

**[핵심/키워드]**

* 흩어진 정도
 * 유형 : 범위, 사분위수, 편차, 분산, 표준편차, 변동계수

### [빅데이터 분석] 이산확률분포 (Discrete Probability Distribution)

**[정의]**

확률 변수가 가질 수 있는 값이 셀 수 있는 (유한하거나 무한하지만 가산적인) 경우의 확률 분포

**[핵심/키워드]**

* 셀 수 있는 값, 이산확률변수, 확률질량함수, 이산누적분포함수
 * 유형 : 이산균등, 베르누이, 이항, 포아송, 기하, 음이항, 초기하

### [빅데이터 분석] 포아송 분포 (Poisson Distribution)

**[정의]**

- 단위 시간 또는 공간 내에서 발생하는 사건의 개수를 모델링하는 이산확률분포 

- 단위 시간/공간 내 발생 건수를 셈
- 사건은 서로 독립적
- 단위 내에서 평균 발생률(λ)은 일정
- 희박한 사건에 적합 (드물지만 일정하게 발생)
- 이항분포의 극한형태 

 * 가정 : 독립성, 비례성, 비집락성

### [빅데이터 분석] 표준정규분포 (Standard Normal Distribution)

**[정의]**

표준화 확률변수 Z에 의해 변환 과정을 거쳐 평균이 0이고 표준편가 1로 정리된 정규분포 

* 평균 0, 표준편차 1 정규분포 
* 종모양/ 좌우 대칭 
 * Z-값, Z분포표
 * 기댓값 0, 분산 1

### [빅데이터 분석] 점추정 (Point Estimation)

**[정의]**

표본자료를 이용하여 모수의 참값이라고 추정되는 하나의 값을 결정하는 추정 기법

**[핵심/키워드]**

* 단일 값 추정
 * 4가지 준거 : 불편성, 유효성, 일치성, 충분성
 * 벙법 : 평균제곱오차, 적률법, 최대가능도

### [빅데이터 분석] 추론통계 (Inferential Statistics)

**[정의]**

모집단으로부터 샘플을 추출, 분석하여 그 결과로부터 모집단에 대한 특성을 추론하는 과정

**[핵심/키워드]**

* 샘플 → 모집단
 * 표본기반 모집단, 통계적 가정
 * 기법 : 가설검정, 점추정, 구간추정, 회귀분석, 분산분석

### [빅데이터 분석] 텍스트 마이닝 (Text Mining)

**[정의]**

비정형 텍스트 데이터에서 유용한 정보, 패턴, 지식을 자동으로 추출하고 발견하는 과정

**[핵심/키워드]**

* 기법 : 정보 추출, 문서분류(군집화), 문서요약, Concept Linkage:, Question Answering, Topic Tracking
 * 절차 : 데이터 수집/클리닝/반환 > 전처리 > 정보추출 > 클러스터링/범주화 > 요약/검색
 * 전처리 : 토큰화, 불용어, 형태소, 어간/어미, 대소문자 통일
 * 표현 : BoW, TF-IDF, Word Embedding, Doc2Vec
 * 마이닝 : 분류, 군집, 토픽모델링, 감성분석

### [빅데이터 분석] 다중공선성  (Multicollinearity)

**[정의]**

회귀분석에서 독립변수들 간에 
 강한 상관관계가 나타나는 문제

**[핵심/키워드]**

ρ(Xi, Xj) ≈ ±1
 확인(산포도, 상관계수, 허용/공차, 
 분산팽창지수(VIF >=10))
 해결(무시, 변수제외, 변수통합, 
 FA, PCA, Ridge)

### [인공지능] Drop Out(드랍아웃)

**[정의]**

심층 신경망의 과적합을 방지하기 위해 은닉층의 일부 노드를 무작위로 비활성화 시켜 정규화(성능 일반화) 하는 신경망 학습 기법

**[핵심/키워드]**

*효과 : 과적합 방지, 앙상블 효과, 학습성능 향상  

* 드랍아웃 유형 
  - 표준 드랍아웃 (Standard Dropout) 
  - Spatial Dropout : CNN에 사용 
  - Variational Dropout : RNN에 사용 
  - Fast Dropout : 계산 비용 감소 
  - Ad-hoc Dropout : 가중치에 적용

### [인공지능] 지식증류(Knowledge Distillation)

**[정의]**

대규모 모델(교사 모델, Teacher Model)이 학습한 지식을 소규모 모델(학생 모델, Student Model)로 전이하여, 성능은 최대한 유지하면서 모델의 크기와 계산 복잡도를 줄이는 기술

**[핵심/키워드]**

LLM성능향상, 모티모달(융합 모듈), 경량화 
 - Teacher / Student 모델 
 - Soft Labels 학습(Temperature 조절 -→ 클래스 확률분포) 
 - Soft Labels 모방 
  ① Distillation Loss(KL Divergence) : Teacher와 Student 모델 출력의 차이
  ② Student Loss(L1/L2 Norm) : 실제 레이블과 Student 모델 출력의 차이

### [인공지능] 생성형 AI데이터품질관리가이드 v2.0 1) 데이터구축과정 2) 품질지표

**[정의]**

- 생성형 AI 데이터 품질관리 가이드라인은 생성형 인공지능(Generative AI) 학습에 활용되는 데이터의 정확성, 다양성, 대표성, 안전성, 법적 준수성을 확보하기 위한 표준 지침서 

- 1.0(초거대AI데이터) -→ 2.0(-LLM, LMM, 합성데이터의 특성 및 품질관리 지표 추가)

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

### [인공지능] Q-러닝(Q-Learning)

**[정의]**

환경과 상호작용하며 Q-값을 업데이트하여 최적 정책을 학습하는 모델 프리 강화학습

**[핵심/키워드]**

모델프리, Value-Based, Off-Policy 
 
 Q-함수 (Q-Function, Q(s,a))
 Q-테이블 (Q-Table)
 벨만 방정식 (Bellman Equation)
 할인율 (Discount Factor, γ)
 학습률 (Learning Rate, α)
 탐색 전략 (Exploration Strategy)
 Epsilon-Greedy 탐색
 
 Q-테이블 크기가 너무 커짐 -→ DQN, DDQN, SARSA

### [인공지능] XAI(eXplainable AI)

**[정의]**

사용자가 인공지능 시스템의 동작과 최종 결과를 이해하고 올바르게 해석하여 결과물이 생성되는 과정을 설명 가능하도록 해주는 기술

**[핵심/키워드]**

알고리즘의 조작 가능성, 의사결정의 편향성 , 머신러닝 AI에 대한 신뢰성 입증 한계 <= 해결 목표 
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

### [인공지능] 빈발패턴성장 알고리즘(FP-Growth, Frequent Pattern)

**[정의]**

분석해야 할 데이터가 증가하면서, 선험적 규칙(Apriori) 알고리즘의 연산 속도를 개선한, 트리(Tree) 구조 기반의 연관규칙 알고리즘(빈발 패턴 집합 탐색, 즉 빈발품목 생성)

**[핵심/키워드]**

- 중복된 트랜잭션을 하나의 트리 경로로 결합 
- 데이터를 압축하여 저장 → FP-Tree를 사용 
 
- 최소 지지도 기반 선택 -→ 빈도 수 기반 정렬 -→ FP-Tree생성 -→ 트리 시작 및 확장 -→ 빈발품목 집합 도출

### [인공지능] SVM  (Support Vector Machine)

**[정의]**

데이터 포인트를 고차원 공간에서 분리하는 최적의 결정경계(Decision Boundary)를 찾아주는 지도 학습(Supervised Learning) 알고리즘

**[핵심/키워드]**

* 구성요소
  - Margin
  - Support Vector
  - Hyper-plane 
  - 하이퍼 파라미터 : C(Regularization Parameter), 허용 오차 (ξ)
 , Epsilon (ε, SVR에서 사용) = 𝜀-Tube (Epsilon-Tube)
 
 * 학습 유형 : 분류, 회귀 
 * 분류 설정 
  - 좁은 마진(큰 C값), 오분류 허용 X (하드 마진) 
  - 넓은 마진(작은 C값), 오분류 허용 O (소프트 마진) 
 
 * 비선형 처리 -→ Kernel 함수(=커널트릭) 이용 
  - 선형, 다항, RBF, 시그모이드

### [인공지능] KNN(K-Nearest Neighbor)

**[정의]**

새로운 데이터 포인트(Test Data)가 주어졌을 때, 기존 학습 데이터(Training Data)와의 거리를 측정하여 가장 가까운 K개의 이웃을 찾고, 다수결 또는 평균을 이용하여 예측하는 비모수적(Non-Parametric) 지도 학습 알고리즘 

- Lazy Learning, 비모수적 모델

**[핵심/키워드]**

- 분류 문제: 가장 많은 속성을 가진 클래스로 분류 (다수결 투표)
- 회귀 문제: K개의 이웃의 평균값을 사용하여 예측
 - 비모수적 모델, 메모리기반학습(레이지 러닝: 학습 불필요)

 &lt;절차&gt;
 - 거리 계산 -→ 가장가까운 k개 데이터 선택 -→ 보팅(분류), 평균(회귀)
 * 장점
  간단하고 효과적, 기본적인 분포가정 필요없음, 학습과정 빠름
  * 단점
  모든 데이터와 거리계산 필요, 새로운 인사이트를 얻는데 제한

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

### [인공지능] Agent2Agent(A2A)

**[정의]**

- JSON-RPC 2.0 기반 메시징을 활용하여  서로 다른 AI Agent 간의 통신 및 협업을 위한 표준 프로토콜

**[핵심/키워드]**

&lt;설계원칙&gt; 
- 에이전트 능력 수용, 기존 표준 기반 개발, 기본 보안 보장, 장기 실행 작업 지원, 모달리티 독립적 설계 

&lt;동작 과정&gt; 
- - 발견 → 요청 → 처리 → 상호작용 → 완료/알림 단계로 동작하며 

&lt;핵심요소&gt; 
- 에이전트 메타 정보: Agent Card, Agent Discovery
- 통신 주체: A2A 서버, A2A 클라이언트
- 작업 단위: Task(작업), Task Lifecycle
- 메시지 구조: Message, Part, Artifact
- 통신 및 확장 기능: 통신 프로토콜, Streaming, Push Notifications, 고급 기능

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
 양자화 및 이진화 (Quantization & Binarization)
 가중치 공유 (Weight Sharing)
 파라미터 효율적 미세 조정 (PEFT, Parameter Efficient Fine-Tuning)
 희소성 유도 (Sparsity Induction)
 지연된 가중치 업데이트 (Delayed Updates)

### [인공지능] 이미지 캡셔닝(ImageCaptioning)

**[정의]**

- 이미지에서 객체, 배경, 동작 등의 시각적 요소를 분석한 후, 이를 자연어 문장으로 설명하는 기술

**[핵심/키워드]**

&lt;구성요소&gt; 
- 이미지 특징 추출기, 언어 모델, 어텐션 메커니즘, 디코더(캡션 생성기), 데이터셋 

&lt;유형&gt; 
- 오토 캡셔닝, 휴먼 캡셔닝, 맥락 기반 캡셔닝, 객체 레벨 캡셔닝, 질의 응답 캡셔닝, 스토리텔링 캡셔닝, 구조화된 캡셔닝, Dense 캡셔닝, Sparse 캡셔닝

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
 5️⃣ 모델 업데이트 및 재배포(Global Model Update & Redistribution) 
 
 모델 결합 알고리즘 
 -FedSGD (Federated Stochastic Gradient Descent)
 - FedAvg (Federated Averaging)
 - FedProx (Federated Proximal)
 - FedOpt (Federated Optimization)
 - FedMA (Federated Matched Averaging)
 - FedBN (Federated Batch Normalization)
 - FedGKT (Federated Gradient Knowledge Transfer)
 - FedReID (Federated Learning for Person Re-identification)

### [인공지능] 규제화(Regularization)

**[정의]**

- 손실 함수에 추가 항을 적용하여 모델의 복잡도를 줄이고, 과적합을 방지하는 기법 
 
 - 모델이 훈련 데이터에 과도하게 최적화되지 않도록 가중치나 구조를 조정하여 일반화 성능을 향상시키는 기법
 
 - 과정합 방지, 손실함수에 규제 적용, 모델 복잡도 감소

**[핵심/키워드]**

- L2(Ridge) : 가중치 축소, 모든 가중치를 0에 가깝게 유지

- L1(Lasso) : 희소성 유도, 특정 가중치가 0이 되도록 유도

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
 &lt;GNN 방법론&gt; 
 Spectral GNN : 주파수 도메인에서 변환
 Spatial GNN : 직접 이웃 노도 정보 학습 
 
 &lt;Spectral GNN&gt; 
  -GCN (Graph Convolutional Network)
 - ChebNet (Chebyshev Graph Convolutional Network)
 - Spectral CNN 
 &lt;Spatial GNN&gt;
 - GraphSAGE (Graph Sample and Aggregate)
 - GAT (Graph Attention Network)
 - MPNN (Message Passing Neural Network)
 - GIN (Graph Isomorphism Network)

### [인공지능] DBSCAN Clustering (Density-based spatial clustering of applications with noise)

**[정의]**

- 데이터 포인트의 밀도를 이용해 군집을 형성하고, 이상치(Noise)를 효과적으로 식별하는 비지도학습 알고리즘
 
 - 반달모양(Moon-Shaped) 비구형 데이터 셋 군집

**[핵심/키워드]**

&lt;하이퍼파라미터&gt; 
  - MinPoints, Epsilon 
 
 &lt;탐색 기준&gt; 
  - 코어, 노이즈, 보더 
 
 &lt;단점 및 해결 알고리즘&gt; 
  - 하이퍼파라미터 설정에 민감, 밀도 다른 경우 군집 어려움 -→ OPTICS 알고리즘(유동적 Epsilon 사용) 

OPTICS (Ordering Points To Identify the Clustering Structure)

### [인공지능] 오토마타 이론 (AutomataTheory)

**[정의]**

- 형식 언어(Formal Language)와 입력을 받아 상태를 변경하는 수학적 모델을 연구하는 학문
- 컴퓨터 과학에서 알고리즘, 언어 인식, 계산 가능성을 분석하는 이론

**[핵심/키워드]**

&lt;구성요소&gt; 
- 오토마톤, 상태(State), 형식 언어(Formal Language), 전이 함수(Transition Function), 입력(Input)과 출력(Output)

결정적 유한 오토마타 (DFA) , 비결정적 유한 오토마타 (NFA) 

오토마톤 → 오토마타 → 유한 오토마톤 → 스택 오토마톤 → 튜링머신

### [인공지능] 메타휴리스틱스 (Metaheuristics)

**[정의]**

- 최적화 문제를 해결하기 위한 상위 개념의 탐색 기법 이며, 완전 탐색(Exhaustive Search) 대신 근사 최적해(Approximate Solution)를 찾는 알고리즘 
- 다양한 문제 도메인에 적용 가능한 일반화된 최적화 기법

**[핵심/키워드]**

&lt;주요 기법&gt; 
- 단일 해 기반 기법: 시뮬레이티드 어닐링(SA), 탭 서치(TS), 확률적 탐색(Randomized Search)
- 집단 기반 기법: 유전자 알고리즘(GA), 개미 군집 최적화(ACO), 입자 군집 최적화(PSO)
- 하이브리드 기법: GRASP(Greedy Randomized Adaptive Search Procedure), MA(Memetic Algorithm)

### [인공지능] AI윤리 (AIEthics)

**[정의]**

- 인공지능 관련 이해관계자들이 준수해야 할 보편적 사회 규범 및 관련 기술

**[핵심/키워드]**

- 3대 기본 원칙 : ▲인간 존엄성 원칙 ▲사회의 공공선 원칙 ▲기술의 합목적성 원칙
- 10대 핵심 요건 : 1) 인권 보장 2) 프라이버시 보호 3) 다양성 존중 4) 침해금지 5) 공공성 6) 연대성 7) 데이터 관리 8) 책임성 9) 안전성 10) 투명성

### [인공지능] GPUaaS (GPUasaService)와 네오클라우드

**[정의]**

GPUaaS (GPU as a Service)
- 클라우드 또는 호스팅 환경에서 고성능 GPU 자원을 필요에 따라 임대 형태로 제공하는 서비스 모델 

네오클라우드 (Neo Cloud)
- AI 연산, 특히 GPU 집중 워크로드에 특화된 클라우드 인프라 또는 서비스 형태

**[핵심/키워드]**

GPUaaS (GPU as a Service)
- 클라우드 GPU 임대
- 온디맨드 서비스
- 사용량 기반 과금
- 고성능 연산(HPC·AI 학습·추론)
- 비용 효율성
- 확장성 및 유연성

네오클라우드 (Neo Cloud)
- 차세대 AI 클라우드 인프라
- GPU 집중형 서비스
- 고성능·저지연 분산 데이터센터
- AI 학습·추론 최적화
 -GPU 자원 다변화(CoreWeave, Lambda 등)
- 비용 절감 및 빠른 확장성

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
- 피지컬 AI 개발 F/W: LWM, Tokenizer, 디지털트윈, 메타버스, AI 가속기
- 데이터베이스: 벡터DB
- 서비스: 자율주행차, 휴머노이드 로봇

### [인공지능] 국가 AI역량 강화 방안

**[정의]**

4대 AI 플래그십 프로젝트(인공지능 3대 강국(AI G3) 도약) -→ 국가 AI역량 강화 방안  

&lt;정의&gt; 
- 국가 차원의 인공지능(AI) 경쟁력 확보를 위한 종합 전략으로, AI 인프라·기술·인재·산업 생태계를 전방위적으로 강화하기 위한 정부 주도 정책 방안

**[핵심/키워드]**

① AI컴퓨팅 인프라 확충
-단기(즉시~단기): 중앙·지자체·민간 협력 기반 3단계 AI 마스터플랜 이행
-중기(2026년): 최첨단 GPU 1만개 규모의 국가 AI컴퓨팅센터 구축
-장기(2030년): 국산 AI반도체 50% 이상 도입 목표
-재정 구조 혁신: 민간 투자 활성화 및 정부 R&D(30~50%), 투자펀드(15~35%) 조성

② 차세대 AI모델 개발
-독자 AI모델 개발·고도화를 위한 생성형 AI 연구개발 집중 지원
-초거대 AI 모델 및 AI 반도체 최적화 기술 개발 추진
-글로벌 경쟁력 확보형 AI 모델 개발 생태계 구축

③ AI전환 가속화
-공공·산업 전반 AI 서비스 확산: 교육·의료·행정·산업 분야에 AI 접목
-AI전환 지원 플랫폼 구축: 중소기업·지자체 대상 AI 활용 지원
-AI 신뢰성·윤리성 확보: 데이터 품질, 보안, 신뢰성 인증체계 강화

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

