# WEB1 - HTML & INTERNET 2번째

---

## 기본 문법 - 태그

기획서를 다시 열어보자.

![기획](https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7594.jpeg)

이런 모양의 웹페이지를 한 번에 만들 수는 없고, 부분적으로 구현하면서 전체적으로 완성해야한다.

html에 'Hypertext Markup Language (HTML) is the standard markup language for creating web pages and web applications.' 라고 내용을 추가한 후 저장

##### 

- 글씨를 '**볼드체**' 로 쓰기 위한 문법

```html
<strong>creating web pages</strong>
```

<strong>creating web pages</strong>



- 글씨를 ''<u>밑줄</u>' 로 쓰기 위한 문법

```html
<u>creating web pages</u>
```

<u>creating web pages</u>



- 중첩해서 사용할수도 있다.

```html
<strong>creating <u>web</u> pages</strong>
```

<strong>creating <u>web</u> pages</strong>



이러한 것들을 HTML에서는 문법적으로 **태그**라고 부른다.

이 외에도 HTML의 태그는 매우매우매우 많다.



##### ※ 한글이 깨질 때

`<meta charset="utf-8">` 을 추가한다.

파일을 저장하면 UTF-8로 저장이 된다. 웹 브라우저에게 UTF-8로 페이지를 열라고 명령하는 것이다.



## 혁명적인 변화

[W3C](<https://www.w3.org/>) -> 국제민간표준화기구 홈페이지

웹은 W3C에 소속된 여러 기업과 기관들의 논의를 통해서 만들어지고 있다.



`<h1></h1>` 이 뭘까?

The `<h1>` to `<h6>` tags are used to define HTML headings. `<h1>` defines the most important heading. `<h6>` defines the least important heading.

heading은 제목이라는 뜻이다. `<h1>`부터 `<h6>`까지, 제목을 나타내는 태그이고, `<h1>`이 가장 큰 제목, `<h6>`이 가장 작은 제목을 나타낸다.



- 제목 나타내기

```html
<h1>안녕</h1>
<h2>안녕</h2>
<h3>안녕</h3>
<h4>안녕</h4>
<h5>안녕</h5>
<h6>안녕</h6>
```

<h1>안녕</h1>
<h2>안녕</h2>
<h3>안녕</h3>
<h4>안녕</h4>
<h5>안녕</h5>
<h6>안녕</h6>



##### 여담

인터넷과 검색 기술이 발달하면서, 모든 정보를 빠르게 찾아낼 수 있는 시대가 왔다.

1분 내에 찾을 수 있는 지식은 아는 것과 다름없다.



## 통계에 기반한 학습

오늘날의 HTML은 약 150개가 넘는 태그가 존재한다.

아래의 그래프는 전 세계에 있는 웹페이지들이 몇 종류의 태그로 이루어져 있는지를 보여준다.

![통계](https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7623.png)

이에 따르면 약 26개의 태그를 사용하는 사이트가 가장 많다는 것을 알 수 있다.



아래 그래프는 태그별 인기도이다.

![태그별 인기도](https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7624.png)

여기서 벌써 `<h1>`, `<h2>` , `<h3>`, `<strong>`을 알고 있다. 많이 했네!

이론상 26개만 잘 숙지해도 웹페이지를 만드는 데에 아무 문제가 없다는 것이다.



## 줄바꿈

코드에서 엔터를 쳐도 실행화면에서는 줄바꿈이 되지 않는다.

줄바꿈을 하기 위해서는 줄바꿈을 해주는 태그가 필요하기 때문이다.



- 줄바꿈

```html
안녕하세요?<br>
만나서 반갑습니다.<br>
안녕하세요?
만나서 반갑습니다.
```

안녕하세요?
만나서 반갑습니다.
안녕하세요? 만나서 반갑습니다. 



`<br>`이라는 태그는 무언가 감싸야하는 내용이 없기 때문에 `</br>`이 존재할 필요가 없다.



- 단락 표현

```html
<p>계절이 지나가는 하늘에는 가을로 가득 차있습니다</p>
<p>나는 아무 걱정도 없이 가을속의 별들을 다 헤일듯합니다</p>
```

계절이 지나가는 하늘에는 가을로 가득 차있습니다

나는 아무 걱정도 없이 가을속의 별들을 다 헤일듯합니다



또 `<p></p>`라는 단락을 나누는 태그도 존재한다.

단락을 표현할 때는 줄바꿈 태그보다는 단락을 나누는 태그가 더 좋은 선택이다.

그 이유는 단락에 단락 태그를 사용하는 것이 웹페이지를 더 가치있게 해 주기 때문이다.



하지만 단락 태그는 단락 사이의 간격이 고정되어 있기 때문에 시각적으로 자유도가 제한되어 있다.

그것을 극복하게 해 주는게 바로 CSS이다.



`<p style="margin-top:45px;">`



라는 것을 `<p>`태그 대신 넣어주면, `<p>`태그 위쪽에 45px만큼의 여백(margin)이 생긴다.

CSS는 나중에 할 것이니 일단 제쳐두자.



위에 태그별 인기도를 보면, `<p>`태그와 `<br>`태그는 각각 81.5%, 70.3%의 빈도를 보인다.

잘 기억해두자.