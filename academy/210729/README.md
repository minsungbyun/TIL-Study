## 24일차(2021-07-29,목)
- 자바 객체지향 문법(eomcs-java/com.eomcs.oop)
	- ex05: h ~ * : 상속 문법(계속)
	- ex06: a ~ c : 다형성(다형적 변수, 오버로딩, 오버라이딩)

## 알게 된 개념
- 메모리 설계도 = 새 데이터 타입 정의
- 데이터(project) vs 기능묶음(업무)(ProjectHandler) 어떤 것에 중심이냐에 따라 클래스를 따로 짠다.
- 데이터를 추상화, 기능을 추상화
- 실세계 => 데이터로 추상화 (환자 정보를 데이터로 저장)

>물리적 : 환자 , 제품(Product)<br>
개념적 : 주문 , 날짜<br>
물리적,개념적인 것을 추상화시킨다.

- API문서 >> 문서화
    - 자신이 짠 코드를 문서화하면 가장 좋다. 
    - 나 이외에 다른 사람이 내가 만든 코드를 유지보수 한다면?

- 자바는 다중상속을 허용하지 않는다.

- 생성자는 한 번만 호출된다. this()나 super()

- overriding = 재정의

- 처음에 짜놓았는데 두 클래스의 공통적인 부분을 발견 >> 추출

* 처음부터 객체지향 프로그래밍을 잘하려고 노력하지 말라 > 리팩토링을 수행하면서 점점 더 유지보수가 좋은 객체지향 프로그래밍 코드로 발전시키면 된다.

1. Specializtion
2. Generalization

- 자식 인스턴스는 부모 인스턴스의 멤버를 가지고 있지만
- 부모 인스턴스는 자식 인스턴스의 멤버를 가지고 있지 않다.

- 형변환(type casting)으로 컴파일러를 속일 수는 있지만,
 - 실행할 때 오류가 발생할 것이다.
     => 속이지 말라!
- ClassCastException = 형변환 잘 못했을 때

- 파라미터 변수의 타입이 클래스라면 - 인스턴스 및 자식(서브) 클래스의 인스턴스 주소를 넘겨줄 수 있다.

- 다형성의 목적
    - 적은 코드로 다양하게 유연하게 사용하기 위해서    융통성 있게

- 오버로딩 오버라이딩

- 필드 오버라이딩은 그냥 새 필드를 추가한 것과 같다.
- 가능한 슈퍼 클래스의 필드와 같은 이름을 만들지 말라!