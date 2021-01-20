# 속성 API

속성은 HTML에서 태그명만으로는 부족한 부가적인 정보라고 할 수 있다. 이 속성을 어떻게 제어하는가 알아보자. 속성을 제어하는 API는 아래와 같다. 각각의 기능은 이름을 통해서 충분히 유추할 수 있을 것이다.

- Element.getAttribute(name)
- Element.setAttribute(name, value)
- Element.hasAttribute(name);
- Element.removeAttribute(name);

### attribute vs property

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <p id="target">Hello world</p>

    <script>
      var target = document.getElementById("target");

      // attribute 방식
      target.setAttribute("class", "important");

      //property 방식
      target.className = "important";

      // 위의 두 방식다 같은 결과를 만든다.
    </script>
  </body>
</html>
```

![image](https://user-images.githubusercontent.com/66653324/105115347-f3eb8b00-5b0b-11eb-86bb-9b64849051ac.png)

하지만 항상 같은 결과가 나오는 것은 아니다.

다음의 경우를 살펴보자

![image](https://user-images.githubusercontent.com/66653324/105115450-2c8b6480-5b0c-11eb-91cd-2429b86ce771.png)
