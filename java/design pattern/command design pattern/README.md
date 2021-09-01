## Command 디자인 패턴

새로운 코드를 추가할 때 기존코드를 손 대지 않는 것이 깔끔하다. 손 대더라도 최소한으로 대야한다. 버그가 생길 가능성이 있기 때문이다.

이를 해결하기 위해서 나온게 Command 디자인 패턴이다.

Command 디자인 패턴은 하나의 명령 처리를 하나의 메서드가 담당하고 있다면 메서드를 별도의 클래스로 분리한다. 즉 기존의 클래스에 손 안대면서 추가할 수 있으며 유지보수에 용이하다.

Q. 클래스가 늘어나는데요?

A. 클래스 파일이 늘어나서 불편한거보다 Command 패턴을 적용시킴으로써 얻는 이점이 더 크다. (클래스가 늘어나는 것은 감수해야한다)
서블릿이 전형적인 커멘드 패턴의 한 예라고 할 수 있다.

![커멘드 디자인 패턴 1](https://user-images.githubusercontent.com/86590036/131596243-19eae41e-246c-4014-8ee0-c6320a3f3fb2.jpg)

![커멘드 디자인 패턴 2](https://user-images.githubusercontent.com/86590036/131596269-02e0bcc6-ebe4-4417-a29f-31fb8392dd92.jpg)

- 공통분모가 없다면 generalization 할 필요없다
  그리고 abstract 클래스 만들때 각각 클래스에서 따로 사용하는 부분이 있으면 넣지 않는다.

- 서브클래스에 사용하지 않고 외부클래스에서 사용하는 기능은 슈퍼클래스에 두지 말고 별도의 클래스를 만들어 분리하는것이 낫다.

-커맨드 패턴을 적용 >> 마지막 인터페이스로 설정한다.