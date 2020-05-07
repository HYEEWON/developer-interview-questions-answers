# Backend Developer Interview Questions
백앤드 개발자 인터뷰 질문 모음과 팁 & 답변

### Table of Content
- [Basics](#basics)
- [OS](#os)
- [Network](#network)
- [Database](#database)
- [Datastructure](#datastructure)
- [Algorithm](#algorithm)
- [Etc](#etc)
- [Optional:Python](#python)
- [Optional:Django](#django)
- [Optional:Java](#java)
- [Optional:Spring](#spring)

### Basics
* 자기소개
  * 이력 중심으로 간단하게 설명하되 신입이라면 성장 욕구를 간단히 어필하는 문구를 넣어도 좋음
* 가장 성공적이었던 프로젝트가 무엇이고 왜 성공적이라고 생각하는지
  * 현재 지원한 공고에 맞는 프로젝트를 성공적인 프로젝트로 지정하여 말하는 것이 유리
* 우리 회사 서비스 중에 사용해본 것
  * 지원한 공고에 맞는 회사 기술 블로그를 분석하고 그와 연관된 서비스를 말하는 것이 유리 
* 지금까지 했던 프로젝트 중 하면서 어려웠던 부분과 극복한 방법
  * 기존에 미리 준비하고 답변하는 것이 유리하며 지원한 회사의 직무에 연관되어 있으면 더 좋음
* 최근 관심 있게 보고 있는 기술
  * 지원한 회사의 직무에 연관되어 있으면 유리
* 이전 직장에서 아쉬웠던 부분과 왜 이직하려는지
  * 이직하고자 하는 회사만의 분명한 장점을 생각해놓고 답변하는 것이 좋음

  
### OS
* 프로세스와 스레드의 차이
  * 프로세스는 프로그램의 실행 상태로 운영체제로부터 자원을 할당받아 실행하고 스레드는 프로세스 안에서 프로세스로부터 자원을 받아 실행
  * 프로세스는 `코드/데이터/스택/힙` 메모리 영역을 기반하지만, 스레드는 프로세스의 코드/데이터/힙 메모리 영역을 공유하고 `개별적인 스택`을 기반으로 함


### Network
* TCP와 UDP의 차이
  * TCP는 `신뢰성을 보장하는 연결형 프로토콜`로 `흐름제어, 혼잡제어, 오류제어`를 제공
  * UDP는 `신뢰성을 보장하지 않는 비연결형 프로토콜`로 흐름제어, 혼잡제어, 오류제어를 제공하지 않음 
  
  
### Database
* Index를 사용하는 이유와 장점 및 단점
  * 인덱스는 데이터베이스의 `검색 속도`를 위해 사용하는 추가적인 자료구조로 테이블 내의 칼럼들로 정의
  * 인덱스를 사용하면 검색이 빨리지지만 테이블의 데이터가 추가, 삭제, 수정이 자주되는 경우 인덱스도 변경해야 하여 성능이 오히려 저하될 수 있음


### Algorithm



### Etc
* 객체와 클래스의 차이
  * 
* 객체지향의 5대 원칙
  * 
* 스크립트 언어와 컴파일 언어의 차이
  * 컴파일 언어는 컴파일러를 통해 사전에 컴파일 되어 기계어 상태로 실행되고 스크립트 언어는 컴파일 단계 없이 인터프리터에 의해 실행 단계해서 한 줄씩 기계어로 번역하여 실행
  * 일반적으로 컴파일 언어가 스크립트 언어에 비해 빠르고 안정적임
* 동기식과 비동기식의 차이
  * 동기식은 요청에 대한 응답을 기다린 후 응답이 오면 실행하는 방식이고 비동기식은 요청에 대한 응답을 기다리지 않고 실행하는 방식
  * 동기식은 구성이 단순하나 멀티태스킹이 불가능하고 비동기식은 멀티태스킹이 가능하나 요청량이 많아질 경우 부하 컨트롤과 데이터의 일관성 유지 등 추가적인 처리가 필요
* 블락킹과 비동기의 차이
  * 블락킹과 비동기 모두 응답을 기다리지 않는 공통점이 있지만, 재실행 시점이 비동기는 요청에 대한 응답이라는 관점이고 블락킹은 함수 호출의 리턴이라는 관점에서 다름
* Redis와 MongoDB
  * Redis는 No SQL 방식을 사용하는 인메모리 데이터베이스로 `Key-Value` 형식으로 데이터를 저장하며 주로 캐쉬로 사용
  * MongoDB는 NO SQL 방식을 사용하는 데이터베이스로 JSON같은 구조의 `Document` 형식으로 데이터를 저장
* 디자인 패턴
  * 소프트웨어 코드 작성 시에 생기는 공통적인 문제를 해결하는데 도움이되는 코드 패턴
* 디자인 패턴 중 싱글톤 패턴
  * 전체 프로그램에서 단 1개의 객체를 생생하고 공유하는 코드 패턴


### Python
* Generator와 사용 시의 장점
  * Iterator를 생성해주는 루틴으로 `yield` 키워드를 통해서 만드는데 Generator는 한번에 모든 데이터를 메모리에 적재할 필요가 없어서 메모리 효율이 높고 계산 결과가 필요할  때 수행되므로 수행 시간 꼭 필요한 시간까지 늦츨 수 있음
* Decorator와 사용 시의 장점
  * 
* Python Garbage Collection 동작 방식
  * 각각의 객체마다 `reference count`를 갖고 있고 몇 곳에서 객체를 참조하는지를 나타내는데 인터프리터가 계속 이를 확인하다가 이 count가 0이 되는 경우 그 객체를 삭제
*  GIL과 GIL을 보완하는 방법
  * 파이썬은 하나의 스레드만이 인터프리터의 제어권을 가질 수 있는 개념인 GIL(Global Interpreter Lock)은 멀티 코어 환경에서도 어느 시점에서나 1개의 스레드만 실행될 수 있기 때문에 `threading`이 아닌 `multiprocessing` 모듈을 통해 스레드 단위가 아닌 프로세스 별로 인터프리터 락을 잡아 보완해야한다.


### Django



### Java
* JVM과 Java 프로그램 실행 과정
  * JVM은 Java Virtual Machine의 약자로 자바 프로그램을 실행하는 역할을 하고 프로그램이 시작되면 컴파일러를 통해 바이트 코드로 변환하고 변환된 파일을 JVM에 로딩하여 실행
* Java에서 Garbage Collection이 필요한 이유에 대해서 설명
  * 자바는 메모리를 명시적으로 해제하지 않기 때문에 GC를 통해서 필요없는 객체를 지우는 작업을 수행
* JVM 메모리 영역 구조
  * 크게 `메소드 영역, JVM 스택, JVM 힙`으로 나뉘며 JVM 힙은 `Young Generation, Old Generation, Permanent Generation`으로 나뉘고 Young Generation은 `Eden, Survivor0, Survivor1`으로 나뉨
* Java Garbage Collection 동작 방식
  * 새롭게 생성된 객체는 Young의 Eden 영역으로 들어가게 되고 Eden 영역이 다 차면 Minor GC가 발생하여 참조 횟수에 따라 증가하는 `age bit`를 보고 불필요한 객체를 삭제하고 생존한 객체는 S0으로 이동
  * Minor GC가 발생할 때마다 각각 Young 영역의 객체들은 삭제와 이동을 하게되는데 (Eden -> S0 / S0 -> S1)
  * S1이 가득 차면 필요한 객체는 OLD 영역으로 이동하고 OLD 영역이 가득차면 Major GC를 통해서 값을 삭제
  * GC가 실행될 때마다 `STOP THE WORLD`가 발생하여 프로그램이 중지
* Overriding과 Overloading
  * 오버라이딩은 부모 클래스에 존재하는 메서드를 하위 클래스에서 재정의하는 것이고 오버로딩은 같은 메서드 이름을 갖게 하지만 시그니처가 다르게 정의하는 것
* 추상 클래스와 인터페이스
  * 추상 클래스는 반드시 구현해야하는 추상 메소드를 1개 이상 갖고 있는 클래스이고 인터페이스는 추상 메소드만 갖고 있는 개념으로 추상 클래스는 1번만 상속받을 수 있지만 인터페이스는 여러번 상속 가능
* private, protected, public 키워드
  * 

### Spring