

### 이모탈 서비스(Immortal Service)란?
##### - &nbsp; 죽지않는 서비스이다.
##### - &nbsp; 안드로이드 서비스(포그라운드, 백그라운드, 바인드) 중 "포그라운드"를 사용한다.


### 이모탈 서비스를 사용해야 할 때(=서비스가 죽지 말아야 할 경우)
##### 1. 앱을 종료 했을 때 -> 기본 서비스를 사용하면 막을 수 있다.
##### 2. 폰을 재시작 했을 때 -> 폰 재시작이 이벤트를 받아 서비스를 재시작
##### 3. Task Kill을 했을 -> startForeground 를 통해서 서비스를 죽지 않게 함.

<br/><br/>


  

<!-- ## 항목
* [리눅스 기본 명령어](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_basicCommand.md)
* [리눅스 Su와 Su - 의 차이점](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_Su.md)
 -->
