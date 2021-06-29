# DAO / DTO / VO 차이점

🧡 DAO

Data Access Object 데이터베이스의 data에 접근하기 위한 객체

데이터베이스의 CRUD(생성/조회/수정/삭제) 기능을 수행하는 메서드들로 구성된 자바빈 객체. 

싱글턴 형태로 생성하여 주로 사용하며, 데이터베이스 제어를 위해 빈도있게 사용하는 모듈


🧡 DTO

Data Transfer Object  데이터 전송 객체

Controller, View.. 등 계층간 데이터 교환을 위한 객체들

GETTER, SETTER 메소드만 가진 클래스


🧡 VO

Value Object

Controller, View.. 등 계층간 데이터 교환을 위한 객체들

내용물이 값 자체를 의미하기 때문에 read Only 특징을 가지고 있음


🧡 그렇다면 VO와 DTO 의 차이점은?

- 데이터 전송을 강조하면 DTO,
- 데이터베이스등에 데이터 유출입에 관여하거나 값을 일시적으로 가지고있는 역할을 강조하면 VO

DTO는 가변의 성격을 가진 클래스이며 데이터 전송을 위해 존재한다.(getter/setter)

VO는 값 그 자체의 의미를 가진 불변 클래스(Read-Only)를 의미한다.(getter만 존재)

DTO는 인스턴스 개념이라면 VO는 리터럴 개념.

회사마다 DTO, VO 사용하는 방식이 다르기때문에 회사에 맞추면 된다고 함!!
