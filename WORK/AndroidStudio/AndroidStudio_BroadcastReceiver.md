

### 브로드캐스트리시버(BroadCastReceiver)란?
##### - &nbsp; 4대 컴포넌트 중 하나이다.
##### - &nbsp; 각종 앱에서 발생하는 방송(이벤트)을 캐치 한 후 리시버로 처리 할 수 있도록 해준다.
##### - &nbsp; "방송하기 -> 수신하기" 두 개가 하나의 사이클로 동작된다.
##### - &nbsp; 정적리시버와 동적리시버로 나뉜다.
<br/><br/>

#### 정적리시버
* 한번 등록되면 해제할 수 없다.
* Manifest에 리시버를 등록하는 방식으로 정적리시버를 등록한다.
* 해당 앱이 설치될 때 자동으로 등록된다.

#### 동적리시버
* 앱이 실행되는 중에만 명령을 실행한다.
* 전원을 껐다 켜면 리시버 동작이 멈춘다.
  

<!-- ## 항목
* [리눅스 기본 명령어](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_basicCommand.md)
* [리눅스 Su와 Su - 의 차이점](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_Su.md)
 -->
