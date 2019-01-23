# Ajax


## Ajax 란?

- AJAX (Asynchronous JavaScript And XML)
  1. 표현 정보를 위한 HTML, CSS.
  2. 동적 화면 출력 및 표시 정보와의 상호작용을 위한 DOM, JavaScript.
  3. 웹 서버와 비동기적으로 데이터를 교환하고 조작하기 위한 XML, XSLT, XMLHttpRequest.

라는데..


## 출처의 내용을 읽고, 내 느낌대로 적어보면..

기존 웹 애플리케이션은 <Form>(html) 태그 속 Submit 을 요청 하나로 보고 요청에 따라 데이터로 응답해준다.
일반적으로 한 사이트의 페이지 정보는 유사한 경우가 많은데, Submit 으로 받은 요청을 받으면 그에 맞는 페이지 데이터를 처음부터 끝까지 다시 보내준다.
그렇게 되면 이미 가지고 있는 중복데이터를 보내야하는 소모가 일어난다.

이것을 최소화하기 위해 Ajax 에서는 요청이 들어오면 요청에 필요한 데이터만 처리해 보내준다. 그 만큼 응답 시간과 무게가 가벼워지고, 웹 서버 처리량도 줄여준다.


## 그래서 Ajax의 내용을 정리한 것이 아래 내용이다.

### *장점*
- 페이지 전환이 빠르다.
- 비동기 요청이 가능하다.
- 수신하는 데이터 양이 줄어들고, 클라이언트에게 처리를 위임할 수 있다.

### *단점*
- Ajax를 쓸 수 없는 브라우저에 대한 문제가 있다.
- HTTP 클라이언트의 기능이 한정된다.
- 페이지 이동이 없는 통신으로 인한 보안상의 문제가 있다.
- 지원하는 Charset(스타일 시트에 쓰이는 문자)이 한정되어 있다.
- 스크립트로 작정되어, 디버깅이 용이하지 않다.
- 과한 요청이 들어오면 서버 부하가 늘 수 있다.
- 다른 도메인과는 통신이 불가능하다.


출처의 내용을 거의 그대로 요약했다..



[출처](https://ko.wikipedia.org/wiki/Ajax)