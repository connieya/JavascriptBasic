# Location 객체

Location 객체는 문서의 주소와 관련된 객체로 Window 객체의 프로퍼티다. 이 객체를 이용해서 윈도우의 문서 URL을 변경할 수 있고, 문서의 위치와 관련해서 다양한 정보를 얻을 수 있다.

![image](https://user-images.githubusercontent.com/66653324/104977954-29c53c80-5a44-11eb-8a8e-bbf1b0ecdd1f.png)

## 현재 윈도우의 URL 알아내기

```javscript

console.log(location.toString());
console.log(location.href);

alert(location)

```

## URL Parsing

location 객체는 URL을 의미에 따라서 별도의 프로퍼티로 제공하고 있다.

```javscript
console.log(location.protocol, location.host, location.port, location.pathname, location.search, location.hash)

```

![image](https://user-images.githubusercontent.com/66653324/104978797-0ac7aa00-5a46-11eb-948d-52360d6626b8.png)

## URL 변경하기

아래 코드는 현재 문서를 http://egoing.net 으로 이동한다.

```
location.href = 'http://egoing.net';
```

```
location = 'http://egoing.net`;
```

현재 문서를 리로드 한다.

```
location.reload
```
