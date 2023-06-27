# 웹서버와 웹애플리케이션 서버
## 웹 - HTTP 기반
- html, text
- image, 음성, 영상, 파일
- JSON, XML(API)
- 등의 모든 형태의 데이터 전송가능
- 서버간에 데이터를 주고 받을 때도 대부분 http 사용
  
&nbsp;

&nbsp;

### 웹 서버(Web Server)
- http 기반으로 동작
- 정적 리소스 제공, 기타 부가기능
- 정적(파일) HTML, CSS, JS, 이미지, 영상
- EX) NGINX, APACHE
  
&nbsp;

### 웹 애플리케이션 서버(WAS - Web Application Server)
- http 기반으로 동작
- 웹서버 기능 포함 +(정적 리소스 제공가능)
- 프로그램 코드를 실행해서 애플리케이션 로직 수행
  - 동적 HTML, HTTP API(JSON)
  - 서블릿, JSP, 스프링 MVC
- EX) 톰캣(Tomcat) Jetty, Undertow

