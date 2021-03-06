# 1강 Framework 개념

#### SW 재사용 방안

1. Copy&Paste

2. Method (function)

3. Class (Inheritance)

4. AOP (Aspect Oriented Programming: 관점 지향 프로그래밍)

   ➡ OOP의 연장선

   > OOP (Object Oriented Programming: 객체 지향 프로그래밍)

   ➡ 핵심 기능과 공통 기능을 분리시켜 사용



#### 디자인 패턴의 정의

* 과제를 해결하기 위한 방법 중 하나

* 개발과정에서 발견된 노하우를 축적하여 이름을 붙여 이후 재사용하기 좋은 형태로 특정 규약을 묶어 정리한 것
* 사용하는 이유?
  - 요구사항 변경에 대한 소스코드의 변경 최소화
  - 팀 프로젝트 진행시 범용적인 코딩 스타일 적용 가능
  - 인수인계하는 경우 직관적인 코드 사용 가능



#### 프레임워크의 정의

* 비기능적 요구사항(성능, 보안, 확장성, 안정성 등)을 만족하는 구조, 구현된 기능을 안정적으로 실행하도록 제어해주는 잘 만들어진 구조의 **라이브러리 덩어리**
* 사용하는 이유?
  * 비기능적 요구사항을 제공하기 때문에 개발자가 기능적인 요구사항에 집중할 수 있게 해줌
  * 디자인패턴과 마찬가지로 반복적으로 발견되는 문제 해결을 위한 특화된 솔루션 제공



#### 디자인패턴 - 프레임워크 관련성

* 디자인 패턴은 프레임워크의 핵심적 특징
* 개발자는 프레임워크의 기반 코드를 확장하여 사용하며 자연스럽게 그 프레임워크에서 사용된 패턴을 적용할 수 있게 된다



#### 프레임워크의 구성요소와 종류

1. IoC (Inversion of Control: 제어의 역전)

   * 인스턴스 생명주기 관리를 개발자가 아닌 컨테이너가 대신 해준다는 뜻

   * **프레임워크는 컨테이너 역할을 한다** 

     => 개발자가 할 일을 프레임워크가 대신 해준다 = 제어의 역전

   * 프레임워크의 동작 원리의 제어 흐름이 일반적인 프로그램의 흐름과 반대로 동작하므로 IoC라고 설명한다

   * Spring 컨테이너는 IoC를 지원, **메타데이터(XML설정)**를 통해 beans를 관리, 어플리케이션의 중요 부분 형성

   * Spring 컨테이너는 관리되는 beans들을 **의존성 주입**을 통해 IoC 지원

2. Class Library

   * 프레임워크는 특정 부분의 기술적인 구현을 라이브러리 형태로 제공

     > **프레임워크 vs 라이브러리**
     >
     > 프레임워크 ➡ 프레임워크 코드가 유저 코드를 호출
     >
     > 라이브러리 ➡ 유저코드가 라이브러리를 호출

3. Design pattern

   * 디자인 패턴 + 라이브러리 = 프레임워크

