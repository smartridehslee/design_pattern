# prototype_pattern
프로토타입패턴

1.개요
- 프로토타입은 실제 제품을 만들기에 앞서 테스트를 위한 샘플 제품을 만드는데 이때, 샘플 제품을 프로토 타입이라고 한다.
- 객체를 생성하는데 비용이 많이 들고 비슷한 객체가 이미 있는 경우에 사용되는 생성 패턴중 하나이다.
- 프로토타입 패턴은 원본 객체를 새로운 객체에 복사하여 필요에 따라 수정하는 메커니즘을 제공한다.
- 시나공
- 원본 객체를 복제하는 방법으로 객체를 생성하는 패턴
- 일반적인 방법으로 객체를 생성하며, 비용이 큰 경우 주로 이용함

2.사용성
- 코드를 복사해야 하는 구현 클래스에 의존하지 않아야 하는 경우 프로토타입 패턴을 사용할 수 있다.
- 객체를 초기화 하는 방식만 다를뿐 서브클래스의 수를 줄이려는 경우 프로토타입 패널을 사용할 수 있다.
- 프로토타입 패턴은 db에서 빈번하게 데이터를 가져올때 그 데이터가 항상 똑같은 값을 반환하는 경우 유용하게 사용 할 수 있다.
- db에 접근하는데 사용하는 자원 비용이 객체를 복사하는 비용보다 훨씬 크다. 그래서 이 패턴을 사용한다. 

3.장단점

 #장점
 - 구현 클래스에 직접 연결하지 않고 객체를 복사할 수 있다.
 - 프로토타입이 미리 정의되어 있기 때문에 중복되는 초기화 코드를 제거할 수 있다.
 - 복잡한 오브젝트를 보다 편리하게 만들수 있디
 
 #단점
 - 순환 참조가 있는 복잡한 객체를 복제하는 것은 매우 까다로울 수 있다.

5.사용 라이브러리
 - 자바 Object 클래스의 clone 메소드와 Cloneable 인터페이스 
 - shallow copy와 deep copy
 - ModelMapper
