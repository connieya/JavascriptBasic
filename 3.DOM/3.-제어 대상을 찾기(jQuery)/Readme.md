# 제어 대상을 찾기

jQuery를 이용하면 DOM을 사용하는 것 보다 훨씬 효율적으로 필요한
객체를 조회할 수 있다. jQuery는 객체를 조회할 때 CSS 선택자를 이용한다.

## jQuery의 기본 문법

jQuery의 기본 문법은 단순하고 강력하다.

```javascript
$("li").css("color", "red");
```

$()는 jQuery의 함수이다. 이 함수의 인자로 CSS 선택자(li)를 전달하면 jQuery 객체라는 것을
리턴한다. 이 객체는 선택자에 해당하는 엘레먼트를 제어하는 다양한 메소드를 가지고 있다.

위의 그림에서 css는 선택자에 해당하는 객체들의 style에 color:red로 변경한다.

## DOM 과 jQuery 비교

`DOM`

```javascript
var lis = document.getElementsByTagName("li");

for (var i = 0; i < lis.length; i++) {
  lis[i].style.color = "red";
}
```

`jQuery`

```javascript
$("li").css("color", "red");
```

---

`DOM`

```javascript
var lis = document.getElementsByClassName("active");

for (var i = 0; i < lis.length; i++) {
  lis[i].style.color = "red";
}
```

`jQuery`

```javascript
$(".active").css("color", "red");
```

---

`DOM`

```javascript
var lis = document.getElementsById("active");

lis.style.color = "red";
lis.style.textDecoration = "underline";
```

`jQuery`

```javascript
$("#active").css("color", "red").css("textDecoration", "underline");
```

위와 같이 jQuery css 속성을 .으로 연결 하는 것을 chaining 이라고 한다.
