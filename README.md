# junior-cs-study-for-interview
신입 백엔드 개발자 기초 CS 스터디

### 스터디원

| ![](https://github.com/haero77.png?size=80) | ![](https://github.com/Tnfls99.png?size=80) |                             ![](https://github.com/hwankim123.png?size=80)                             | ![](https://github.com/dlxortmd987.png?size=80) |
|:-------------------------------------------:|:-------------------------------------------:|:------------------------------------------------------------------------------------------------------:|:-----------------------------------------------:|
|     [김선호](https://github.com/preferkim)     |      [이수린](https://github.com/Tnfls99)      |                                  [김 환](https://github.com/hwankim123)                                  |                     [이택승](https://github.com/dlxortmd987)                     |

<br>

### 진행방식

- 현재 repo를 개인 깃헙으로 fork 뜹니다.
- [일정표](https://github.com/devcourse-study/junior-cs-study-for-interview/blob/main/etc/%EC%8A%A4%ED%84%B0%EB%94%94%20%EC%A7%84%EB%8F%84%ED%91%9C.md)를 확인하고, 다음 스터디 일자에 맞는 진도를 공부합니다.
- 면접 질문에 대한 답안을 작성하고,다음 스터디 시작 전까지 본인 깃허브 닉네임에 해당하는 branch 로 PR을 올립니다.
  - **PR을 올리지 않았을 경우 벌칙 스택이 하나 증가합니다.**
  - 벌칙 스택이 3개 되었을 경우 다른 스터디원들에게 커피 쿠폰을 돌립니다. (벌칙 스택은 초기화됩니다.)
- 모의면접
  - 랜덤으로 지원자 2명을 선정합니다. 남은 2명은 면접관 역할을 수행합니다.
    - 면접관은 지원자 중 한 명을 골라, 무작위로 질문을 합니다.
  - 면접이 끝났을 경우 면접관과 지원자의 역할을 바꾸어 진행합니다.



<br>

# 스터디 주제

## 1. Java

### Java 기초
- Java 의 장단점
- 데이터 타입
  - Wrapper Class
    - Boxing vs Unboxing
  - Call by Reference, Call by Value
- 접근제어자
- 클래스 vs 객체 vs 인스턴스
- static 키워드
  - static 멤버 vs non static 멤버
  - static class vs static method
    - main 메서드가 static 인 이유
  - static 컴파일 과정
- 오버로딩과 오버라이딩
- 인터페이스와 추상 클래스
  - 클래스의 단일 상속과 인터페이스의 다중 구현
- Exception
  - Checked Exception vs Unchecked Exception
- final 키워드 (final/finally/finalize)
- 제네릭
- 리플렉션
- 직렬화 vs 역직렬화
- Synchronized & Thread Safe
  - Sync vs Async
- 어노테이션
- Java 8
  - Stream
  - Lambda
    - 익명 함수와 람다
  - Optional

### Java 컬렉션
- 컬렉션 프레임워크
  - 프레임워크
- equals() & hashcode()
  - `==` vs `equals()`
  - hashcode
- String
  - String vs StringBuilder vs StringBuffer
  - `new` vs `""`
- Map / Set / List 와 각각의 구현체
  - List
    - ArrayList vs LinkedList
  - Map
    - HashTable vs HashMap vs LinkedHashMap vs TreeMap
    - HashMap vs ConcurrentHashMap
  - Set
    - List vs Set

### JVM / GC
- JDK, JRE, JVM 의 차이
- 자바 컴파일 과정
- JVM 구조
  - JVM 구성 요소
  - JVM 실행 과정
  - JVM 메모리 구조
- 클래스 로더와 동적로딩
- 가비지 컬렉션 동작원리
  - Java9 default GC

### 객체 지향 프로그래밍
- 객체
- 객체지향 프로그래밍
  - 객체지향 프로그래밍 vs 절차지향 프로그래밍
- OOP 5대 원칙 SOLID
- OOP 4가지 특징

<br>

### 2. Database

- 관계형 데이터베이스
  - 데이터베이스를 사용하는 이유 
  - RDB의 개념과 장단점
  - 키의 종류
- 인덱스
  - 인덱스 개념, 필요성
  - 인덱스를 어느 column에 사용할까
- 인덱스의 자료구조
  - `hash table`, `b-tree`, `b+tree` 
  - 인덱스가 `hash table` 이 아닌 `b+tree`로 구현된 이유
- Join
  - left outer join vs inner join
- 정규화
  - 정규형의 종류
  - 이상 현상
- View
- 트랜잭션
  - 트랜잭션 개념
  - ACID
  - Lock
- 트랜잭션 격리수준
  - DeadLock
- NoSQL
  - NoSQL 개념
  - RDB vs NoSQL

### 3. OS

- Process & Thread
  - Process 개념
    - Process 메모리 영역
    - Process State: Running, Ready, Wait
  - Multi Process
    - PCB(Process Control Block) 
    - Context, Context Switch
  - Thread 개념
    - Process Vs. Thread
  - Multi Thread
  - Multi Process Vs. Multi Thread
  - IPC(Inter Process Communication)
    - 공유 메모리와 메시지 전달 모델
  - Multi Process/Thread 환경의 동기화 문제해결
    - Mutex, Semaphore
  - Deadlock
- Memory
  - Paging
    - Memory Fragmentation
  - Segmentation
    - Paging Vs. Segmentation
    - Paged Segmentation
  - 가상 메모리
    - Demand Paging
    - 페이지 교체 알고리즘(replacement algorithm)
    - LRU, LFU

### 4. Spring & JPA

### Spring Core

- Spring Framework
  - Framework
  - `Spring` Vs. `Spring Boot` Vs. `Spring MVC`
- DI(Dependency Injection)
  - 생성자 주입을 지향하는 이유
- IoC(Inversion of Control)
  - 스프링 컨테이너
  - 싱글톤 컨테이너
- 스프링 빈
  - 빈 생명주기 콜백
  - 빈 스코프
- 컴포넌트 스캔
  - `@ComponentScan`, `@Component`
  - `@Controller`, `@Service`, `@Repository`
- POJO

### Spring MVC

- WAS, WS
  - Tomcat
- MVC 패턴
- Servlet
- Dispatcher Servlet
  - 요청 흐름
- RequestMapping Handler Adapter 
  - 구조 이해
- 스프링 MVC의 어노테이션
- 스프링 예외처리와 `@ExceptionHandler`

### Spring 심화

- AOP
  - JDK Dynamic Proxy
  - CGLIB
- ThreadLocal
- 필터와 인터셉터

### Spring Test

- DDD, TDD
  - 테스트 커버리지 (JACOCO)
- 단위, 통합, 인수 테스트
  - SpringBoot 계층별 테스트 방법
- Junit4 vs Junit5
- Test Double
  - Stub
  - Mock
  - Fake

### JPA 

- JDBC, Spring JDBC
  - Connection Pool
  - DataSource
- Sql Mapper(MyBatis)
- JPA, Hibernate
  - ORM
- 영속성 컨텍스트
  - OSIV
- 즉시/지연 로딩
  - 프록시
  - N + 1 문제
- 단뱡향/양방향 매핑
  - Join vs Fetch Join
  - 고아객체
- 상속관계 매핑
  - @MappedSuperclass
  - 임베디드 타입
- `@Trasactional`
  - 동작원리

### 5. Network

- OSI 7계층과 TCP/IP 4계층
- TCP/UDP
  - 3way-handshake, 4way-handshake
  - 흐름제어, 혼잡제어, 오류제어
- HTTP
  - HTTP status code
  - HTTP METHOD
- HTTP 1.1 VS HTTP 2.0
- HTTPS
- REST API
- CORS
- COOKIE & SESSION
- JWT
- DNS
- Blocking/Nonblocking&Synchronous/Asynchronous
- 웹 통신의 흐름
  - www.example.com을 입력했을 때?

### 6. Data Structure

> 추가 예정 

---
**참고**
> - https://github.com/ham-study/cs-study-for-interview
> - https://github.com/VSFe/Tech-Interview
> - https://github.com/JaeYeopHan/Interview_Question_for_Beginner
