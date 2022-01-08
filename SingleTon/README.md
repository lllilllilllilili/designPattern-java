## 디자인 패턴을 사용하는 이유

- 소프트웨어를 재상용할 수 있고, 유연하고, 확장성 있고, 유지보수가 용이하게 만드는 것은 매우 어려운 일임
- 코드 한줄 고치는데 멤먼스가 10 사람이 붙는다면? ⇒ 다른 개발 & 유지보수를 못하게 되는것 > 비용 발생

## solid

- SRP (Single Responsibility Principle)
    - 하나의 클래스는 하나의 기능만 구현
- OCP (Open/Closed Principle)
    - 인터페이스 or 추상클래스를 통해 접근
- LSP (Liskov substitution Principle)
    - 하위 클래스는 상위 클래스로 교체할 수 있어야 한다.
        - 너무 당연한 얘긴데, subject class가 존재하는것을 의미한다.
        - IS-A
- DIP(Dependency Inversion Principle)
    - 의존관계는 구체적인것에 비해 추상적인것에 의존한다.
- ISP(Interface Segregation Principle)
    - 제공하는 기능에 대한 인터페이스에만 종속적이어야 한다.

## class diagram

- abstract, interface = 이탈릭체
    
    ![스크린샷 2022-01-08 오후 3.07.19.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a563edcc-2547-4ed8-b94e-412ca98a6e8f/스크린샷_2022-01-08_오후_3.07.19.png)
    
- Generalization (일반화)
    - 서브 클래스 → 슈퍼 클래스 (Generalize, 일반화)
        - - - - - - -
    - 슈퍼 클래스 → 서브 클래스 (Specialize, 구체화)
        - ————
- Realization (실체화)
- 집합과 합성의 차이
    - 집합 (일부분이 되는 관계)
    - 합성 (하나가 삭제되면 다른 하나가 존재할 수 없다.)
    - is-a v s has-a
        - is-a : 일반적인 상속 관계를 의미
            - 알부분의 관계를 형성하고 있기 때문에 부모 클래스가 변경되면 같이 변경되는 위험성 존재 그러나 설계가 단단해질 수 있다는 장점
        - has-a : 클래스안에서 구현클래스를 들고있는것을 의미
            - 객체의 느슨한 결합이 특징, 변경사항에 is-a 관계보다 크리티컬 위험이 적다.
- 의존관계
    - - - - - - - >

![스크린샷 2022-01-08 오후 3.40.10.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2d6d2472-cf0a-489a-81b7-3266ba47a8cb/스크린샷_2022-01-08_오후_3.40.10.png)

## 싱글톤 패턴

- 실습

## Java Reflection

- 실습