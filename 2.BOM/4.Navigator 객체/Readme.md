# Navigator 객체

브라우저의 정보를 제공하는 객체다.
주로 호환성 문제등을 위해서 사용한다.

![image](https://user-images.githubusercontent.com/66653324/104979180-fcc65900-5a46-11eb-80e9-acf8dbc98cb9.png)

### 크로스브라우징(cross browsing)

W3C , ECMA 국제 기구에서

인터넷익스플로어, 파이어폭스, 크롬 , 사파리 ,오페라와 같은
브라우저의 상황에 맞게 구현해준다.

![image](https://user-images.githubusercontent.com/66653324/104979357-6e060c00-5a47-11eb-87a2-77d29fe36ce3.png)

넷스케이프사와 인터넷 익스플로어 의 이벤트가 다르다

그래서 웹 표준이 필요하다.

### 기능

아래 명령을 통해서 이 객체의 모든 프로퍼티를 열람할 수 있다.

```
console.dir(navigator);
```

#### appName

웹브라우저의 이름이다. IE는 Microsoft Internet Explorer,
파이어폭스, 크롬등은 Nescape로 표시한다.

```
console.dir(navigator.appName)

```

#### appVersion

브라워저의 버전을 의미한다.

```
console.dir(navigator.appVersion)
```

5.0 (Windows NT 10.0; Win64; x64)
AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36

#### userAgent

브라우저가 서버측으로 전송하는 USER-AGENT HTTP 헤더의 내용이다. appVersion과 비슷하다.

```
console.dir(navigator.userAgent)
```

![image](https://user-images.githubusercontent.com/66653324/104979893-afe38200-5a48-11eb-9a50-c1ad48294184.png)

#### platfrom

브라우저가 동작하고 있는 운영체제에 대한 정보다.

```
console.dir(navigator.platform)


```

---

## 기능테스트

![image](https://user-images.githubusercontent.com/66653324/104980057-0cdf3800-5a49-11eb-8326-0031d7bb406c.png)
