# MVC 패턴이란?
모델(Model), 뷰(View), 컨트롤러(Controller)로 이루어진 디자인 패턴이다.  

### MVC 패턴의 장점
재사용성과 확장성이 용이하다.

### MVC 패턴의 단점
애플리케이션이 복잡해질수록 모델과 뷰의 관계가 복잡해진다.  

<br><br>

## 모델(Model)
애플리케이션의 데이터인 데이터베이스, 상수, 변수 등을 뜻한다.  
뷰에서 데이터를 생성하거나 수정하면 컨트롤러를 통해 모델을 생성하거나 갱신한다.

## 뷰(View)
모델을 기반으로 사용자가 볼 수 있는 화면을 뜻한다.  
inputbox, checkbox, textarea 등 사용자 인터페이스 요소를 나타낸다.  
변경이 일어나면 컨트롤러에 전달한다.

## 컨트롤러(Controller)
하나 이상의 모델과 뷰를 잇는 다리역할을 하며 이벤트 등 메인로직을 담당한다.
모델이나 뷰의 변경사항이 생기면 이를 해석하여 각각의 구성요소에 해당 내용에대해 알려준다.

<br><br>
  
### 대표적인 라이브러리
- 리액트
