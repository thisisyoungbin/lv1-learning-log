# 우아한 테크코스 레벨1 학습로그


***


# **LOTTO**
## [TDD] 단위 기능별 테스트 - 3
### 내용
각 도메인 구현 전에 기능별 테스트코드 작성 후 구현
ex) Lotto, LottoGame, LottoNumber 등

## [OOP] 원시값 포장 및 일급 컬렉션 사용 - 3
### 내용
LottoNumber와 Money 원시값 포장
Lotto, Lottos 일급컬렉션 사용

## [OOP] Enum Class 활용 - 3
### 내용
당첨개수를 비교해 등수를 정하는 Rank를 Enum 클래스를 활용해 구현

## [JDK] Stream API 활용 - 3
### 내용
반복문 사용을 지양하며 최대한 많은 곳에 Stream API를 활용

## [JDK] EntrySet 활용 - 2
### 내용
LottoGameResult에서 Map으로 받은 게임 결과를 EntrySet을 활용해 결과 출력

## [OOP] Interface를 활용한 전략 패턴 활용 - 4
### 내용
로또 생성을 위해 LottoGenerator 인터페이스 사용
테스트 코드와 실제 production 코드에서 각 Lottogenerator를 구현한 FixedGenerator, RandomGenerator 활용

## [OOP] 정적 팩토리 메서드 사용 - 2
### 내용
View에서 객체를 생성해서 컨트롤러로 넘겨주던 로직을 정적 팩토리 메서드를 통해 도메인에서 직접 객체 생성하도록 활용
ex) Money, LottoAmount, Lottos, Lotto

## [OOP] 캐싱 활용 - 2
### 내용
일정한 수만큼 필요한 LottoNumber를 캐싱한 후 꺼내올 수 있도록 활용
처음에 배열로 캐싱했으나 Map을 활용하면서 유효성 검증이 더 쉬워졌다.


***


# **BLACKJACK**
## [TDD] 단위 기능별 테스트 - 2
### 내용
각 도메인 구현 전 테스트를 먼저 작성한다.
가능한 모든 부분들에 대해 테스트 주도 개발을 진행하려 했으나 그렇지 못한 부분들이 있어 아쉽다.

## [OOP] 상속과 composition - 4
### 내용
추상 클래스인 Participants를 User와 Dealer가 상속받는다.

## [OOP] Enum Class 활용 - 3
### 내용
카드의 Suit, Value를 Enum 클래스를 활용해 구현한다.
참가자들의 승무패 여부를 WinOrLose Enum 클래스를 이용해 구현한다.
참가자들이 카드를 더 받을 수 있는지, 블랙잭인지 상태를 알 수 있도록 Status를 Enum 클래스를 이용해 구현한다.

## [JDK] Stream API 활용 - 3
### 내용
collect, findAny, map 등 다양한 Stream API를 활용해 코드를 작성한다.

## [JDK] 함수형 인터페이스 활용 - 2
### 내용
BiPredicate를 활용해 딜러와 유저의 점수를 비교한다.
supplier를 활용해 예외처리한다.


***


# **CHESS**
## [TDD] 테스트 주도 개발- 4
### 내용
각 도메인 구현 전 테스트를 먼저 작성한다.
기물들의 이동에 대한 테스트 코드를 작성하고, 구현한다.


## [OOP] Enum Class 활용 - 4
### 내용
Board를 구성하는 Column, Row를 enum을 활용해 구현한다.
Command를 enum을 활용해 구현한다.
기물들이 가질 수 있는 움직임을 enum을 활용해 구현한다.
기물들을 enum을 활용해 구현한다.

## [JDK] Stream API 활용 - 3
### 내용
보드판 위의 기물들의 점수를 stream API를 활용해 구한다.
기물들의 이동전략을 찾기 위해 stream API를 활용한다.

## [JDK] 함수형 인터페이스 활용 - 2
### 내용
BiConsumer를 활용해 각 명령에 따라 다른 행동을 하고, 상태를 변경한다.

## [OOP] 전략 패턴 활용 - 3
### 내용
기물들은 각각 다른 이동 전략을 갖고 있다.

## [OOP] DTO 활용 - 2
### 내용
도메인에서 DTO를 생성해 컨트롤러에게 전달한다.
DTO를 활용해 출력 형식를 만들어 출력한다.

## [OOP] Interface를 활용한 상태 패턴 활용 - 4
### 내용
GameState를 구현한 Ready, Running, Finished 상태가 존재한다.
Command가 들어올 때 상태마다 동작을 한다.


## [DB] MySql을 이용한 DB 활용 - 3
### 내용
Mysql 쿼리문을 이용해 DB에 데이터를 저장, 수정, 삭제, 조회 할 수 있다.

## [OOP] Dao 를 활용한 데이터 접근 - 2
### 내용
ChessGameDao 클래스를 활용해 DB에 접근 가능하다.

## [WEB] 스파크 프레임 워크를 이용한 웹 서버 구현 - 3
### 내용
스파크 프레임워크를 활용해 웹 서버를 구현한다.
요청에 따른 응답을 통해 체스게임을 웹에서 실행할 수 있다.
