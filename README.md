# js_tictactoe

자바스크립트로 틱택토 게임 만들기

**순서도**

1. html/css를 만든다.
2. 게임 시작 버튼과 틱택토 게임 보드 (3 x 3)를 만든다.
3. 게임 시작 버튼을 누르면 모든 내용을 초기화 한다.
4. x, o의 위치를 기록한다.
5. x, o를 화면 보드에 표시한다. (현재 턴인 사람)
6. 클린한 칸이 빈칸이여야 입력이 가능하다.
7. 턴을 바꿔준다.
8. 이겼는지 비겼는지 확인한다.
9. 결과가 나왔으면 (이기거나 비기거나) 결과 표시 후 게임종료
10. 아니면, 계속 게임 진행

제로초 강의 참고 -> 이차원 배열로 만듬.
(Web Dev Simplified나 Clever Programmer은 1차원 배열 사용.-> 이럴 경우 코드가 더 복잡할 수 있다.)

**새롭게 알게 된 내용**

CSS

- css variables (적용가능 O)
- ::after ::before (적용가능 X)
- nth-child (적용가능 O)

Javascript

- every/some
- flat

이벤트 버블링 : 한 요소에 이벤트가 발생하면, 해당 요소 -> 부모 -> 최상단 조상 요소를 만날때까지 요소 각각에 할당된 핸들러 동작
이벤트가 발생한 가장 안쪽의 요소는 타깃(target)요소라 불리고, event.target을 사용해 접근 가능
event.target vs. this(=event.currentTarget) 차이점:
- event.target은 실제 이벤트가 시작된 '타깃'요소. 버블링이 진행되어도 변하지 않음
- this 는 '현재'요소. 현재 실행 중인 핸들러가 할당된 요소를 참조

이벤트 위임
1. 컨데이너에 하나의 핸들러 할당
2. 핸들러의 event.target을 사용해 이벤트 발생한 요소 위치 확인
3. 원하는 요소에서 이벤트가 발생하면 이벤트를 핸들링함



**다음 할 것**

리액트 클래스 컴포넌트로 틱택토 만들기

참고자료

1. https://www.youtube.com/watch?v=Y-GkMjUZsmM&t=1985s
2. https://www.youtube.com/watch?v=VjjZ2MaX0Ts&t=7072s
3. https://www.youtube.com/watch?v=gP9p8jUpKWo&list=PLcqDmjxt30RvEEN6eUCcSrrH-hKjCT4wt&index=74
