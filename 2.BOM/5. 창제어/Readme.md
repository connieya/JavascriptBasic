# 창 제어

window.open 메소드는 새 창을 생성한다.
현대의 브라우저는 대부분 탭을 지원하기 때문에 window.open은
새 창을 만든다.

### 창 제어 상호작용

windowOpen.html 참고

# 보안

### 팝업 차단

![image](https://user-images.githubusercontent.com/66653324/104988915-a3692480-5a5c-11eb-8db8-a014da763b44.png)

같은 도메인일 경우 (ex. 두개의 창 모두 localhost) open도 허용하고
작업도 할 수 있음

근데 만약 다른 도메인일 경우
ex) 새창의 도메인이 opentutorial.org

제한을 줘야한다. 그러지 않으면 악의적으로 작업에 방해를 줄 수 있다.
