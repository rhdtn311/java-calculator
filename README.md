## 📌 과제 설명

사칙연산이 가능한 계산기를 구현했습니다.

<br>

## 🧩 요구 사항과 구현 내용

연산

- [x]  더하기
- [x]  빼기
- [x]  곱하기
- [x]  나누기
- [x]  우선순위
- [x]  테스트 코드 작성
- [x]  계산 이력을 맵으로 데이터 저장기능 만들기
- [x]  정규식 사용

<br>

## 🎱 주요 클래스

- ******************Calculator******************
    - 계산 기능 및 계산기의 전체적인 동작을 수행합니다.
- **************Console**************
    - 입출력 기능을 담당합니다.
- **************Storage**************
    - 계산 이력을 저장합니다.
- **************************PostfixMaker**************************
    - 문자열 형태의 중위표기법을 리스트 형태의 후위표기법으로 변환합니다.
- ****************************InputValidator****************************
    - 사용자 입력값, 잘못된 계산식에 대해 검증합니다.

<br>

## ✔ PR 포인트 & 궁금한 점

- 가독성이 좋지 않는 코드를 많이 작성한 것 같은데 더 가독성 좋은 코드를 작성하기 위해서 제가 놓치고 있는 점이 있을까요 ??
- 현재 좀 더 기능이 분리 되어야 하는 클래스가 있을까요 ?
- 실제 기능을 위해서가 아닌 테스트 코드를 위해서 `Storage` 인터페이스에 `removeAll`이라는 메서드를 구현하였는데 좋지 않은 방식일까요..?
- `ListStorageTest`, `MapStorageTest` 코드 작성 시 `MapStroage`, `ListStorage`에 실제 데이터를 저장하는 자료구조가 `private` 접근제한자라 `findAll()` 메소드의 테스트코드를 작성할 때 `save()`라는 메소드를 사용하였습니다. 단위 테스트 간에 서로 영향을 미치는(?) 코드가 작성되었는데 좋지 않는 코드일까요?
