# String, StringBuffer, StringBuilder

## String

특징

1. 불변(Immutable)
2. 문자열을 조작하는 경우 유용하게 사용 할 수 있다.
문자열, 숫자, char 등은 concat 할때 StringBuffer, StringBuilder를 사용할 수 있다. 단, 복잡한 경우 의미가 있고 단순한 경우에는 +연산자를 통해 처리한다.
3. String 객체는 한번 생성되면 할당된 메모리 공간이 변하지 않는다
+연산자 또는 concat 메서드를 통해 기존에 생성된 String 클래스 객체 문자열에 다른 문자열을 붙이면 새로운 String 객체를 만든 후 새 String 객체에 연결된 문자열을 저장하고, 그 객체를 참조하도록 한다(기존 객체가 제거되면 Java의 가비지 컬렉션이 회수) → 성능이 좋지 않음.
4. 동기화에 신경쓰지 않아도 되기 때문에(Thread-safe), 내부 데이터를 자유롭게 공유 가능하다.

## StringBuffer, StringBuilder

1. 변함(mutable)
2. 문자열 연산 등으로 기존 객체의 공간이 부족하게 되는 경우, 기존의 버퍼 크기를 늘리며 유연하게 동작한다.

## StringBuffer

1. 각 메서드 별로 Synchronized Keyword가 존재하여 멀티 스레드 환경에서도 동기화를 지원한다.

## StringBuilder

1. 동기화를 보장하지 않는다.(단일 스레드 환경이라면 권장)

## 정리

**String은 짧은 문자열을 더할 경우 사용합니다.**

**StringBuffer는 스레드에 안전한 프로그램이 필요할 때나, 개발 중인 시스템의 부분이 스레드에 안전한지 모를 경우 사용하면 좋습니다.**

**StringBuilder는 스레드에 안전한지 여부가 전혀 관계 없는 프로그램을 개발할 때 사용하면 좋습니다.**

출처:

[https://12bme.tistory.com/42](https://12bme.tistory.com/42)

[길은 가면, 뒤에 있다.]