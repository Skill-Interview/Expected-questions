# 객체 지향 프로그래밍( OOP )

## OOP의 4가지 특징

### 1. 추상화 
List 구체적인 사물들의 공통적인 특징을 파악해서 이를 하나의 개념(집합)으로 다루는 것 /
인터페이스로 클래스들의 공통적인 특성(변수, 메소드)들을 묶어 표현하는 것

### 2. 캡슐화 
정보 은닉(information hiding): 필요가 없는 정보는 외부에서 접근하지 못하도록 제한하는 것 /
실제로 구현 부분을 외부에 드러나지 않도록 하는 것 /
변수와 메소드를 하나로 묶음 /
데이터를 외부에서 직접 접근하지 않고 함수를 통해서만 접근 /
ex) public, private, protected
public : 클래스 외부에서 접근 가능
private : 클래스 내부에서만 접근 가능
protected : 상속받은 자식 클래스에서만 접근 가능

### 3. 상속 
자식 클래스가 부모 클래스의 특성과 기능을 물려받는 것 /
기능의 일부분을 변경하는 경우 자식 클래스에서 상속받아 수정 및 사용함 /
상속은 캡슐화를 유지, 클래스의 재사용이 용이하도록 해 준다.

### 4. 다형성 
서로 다른 클래스의 객체가 같은 메시지를 받았을 때 각자의 방식으로 동작하는 능력 /
어떤 변수,메소드가 상황에 따라 다른 결과를 내는 것 /
* 오버로딩(Overloading) : 하나의 클래스에서 메소드의 이름이 같지만, 파라메터가 다른 것 
* 오버라이딩(Overriding) : 부모 클래스의 메소드를 자식 클래스의 용도에 맞게 재정의하여 코드의 재사용성을 높임


## OOP의 5대 원칙 (SOLID)

1. S: 단일 책임 원칙(SRP, Single Responsibility Principle)
객체는 단 하나의 책임만 가져야 한다.
2. O: 개방-폐쇄 원칙(OCP, Open Closed Principle)
기존의 코드를 변경하지 않으면서 기능을 추가할 수 있도록 설계가 되어야 한다.
3. L: 리스코프 치환 원칙(LSP, Liskov Substitution Principle)
일반화 관계에 대한 이야기며, 자식 클래스는 최소한 자신의 부모 클래스에서 가능한 행위는 수행할 수 있어야 한다.
4. I: 의존 역전 원칙(DIP, Dependency Inversion Principle)
의존 관계를 맺을 때 변화하기 쉬운 것 또는 자주 변화하는 것보다는 변화하기 어려운 것, 거의 변화가 없는 것에 의존하라는 것이다.
5. D: 인터페이스 분리 원칙(ISP, Interface Segregation Principle)
인터페이스를 클라이언트에 특화되도록 분리시키라는 설계 원칙이다.

출처 : [https://gmlwjd9405.github.io/2017/10/01/basic-concepts-of-development-java.html](https://gmlwjd9405.github.io/2017/10/01/basic-concepts-of-development-java.html)
