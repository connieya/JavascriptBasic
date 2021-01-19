# HTMLElement

getElement\* 메소드를 통해서 원하는 객체를 조회했다면, 이 객체들을 대상으로 구체적인 작업을 처리해야한다.

<br/>
이를 위해서는 획득한 객체가 무엇인지 알아야한다. 그래야 적절한 메소드나 프로퍼티를 사용할 수 있다.

### 상속

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <a href="http://opentutorials.org" id="anchorss">opentutorials</a>

    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li id="list">JavaScript</li>
    </ul>

    <input type="button" value="button" id="button" />

    <script>
      var target = document.getElementById("list");

      console.log(target.constructor.name); // HTMLLIElement

      target.type = "square";

      var target = document.getElementById("anchorss");

      console.log(target.constructor.name); // HTMLAnchorElement

      target.target = "_blank";
      target.href = "http://www.naver.com";

      var target = document.getElementById("button");

      target.style.backgroundColor = "pink";
      console.log(target.constructor.name); // HTMLInputElement

      // 위의 코드를 보면 getElementById라도 객체가 다르다.
      // 그렇기 때문에 각 각의 객체가 가지고 있는 프로퍼티도 다르다.
      // 즉 기능이 다르다!!!

      // 간단한 예로 a 태그에는 href도 있고 target 속성도 있지만
      // li 태그에는 없다잉~~~~
    </script>
  </body>
</html>
```

위의 코드에 나오는

- HTMLLIElement
- HTMLAnchorElement
- HTMLInputElement

모두 `HTMLElement`를 상속 받고 있다. 일명 자식이다

# DOM Tree

모든 엘리먼트는 HTMLElement의 자식이다. 따라서 HTMLElement의 프로퍼티를 똑같이 가지고 있다. 동시에 엘리먼트의 성격에 따라서 자신만의 프로퍼티를 가지고 있는데 이것은 엘리먼트의 성격에 따라서 달라진다. HTMLElement는 Element의 자식이고 Element는 Node의 자식이다. Node는 Object의 자식이다. 이러한 관계를 DOM Tree라고 한다. 이 관계를 그림으로 나타내면 아래와 같다.

![image](https://user-images.githubusercontent.com/66653324/105002321-690b8180-5a74-11eb-9941-9e3c774f183c.png)
