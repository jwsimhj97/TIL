### IntentFilter란?
##### - &nbsp; 인텐트의 작업, 데이터 및 카테고리를 기반으로 어느 유형의 인텐트를 수락하는지 지정한다.
<br/><br/>

### IntentFilter의 특징
##### - &nbsp; 명시적, 암시적으로 나뉜다.
##### - &nbsp; 앱의 매니페스트에 있는 < intent-filter > 요소에서 정의하고, 인느 대응되는 앱 구성 요소에서 중첩된다.
##### - &nbsp; 여러 가지 종류의 인텐트를 처리하고자 하되 특정 조합의 작업, 데이터, 카테고리 유형으로만 한정하고자 할 때는 여러 인텐트 필터를 생성해야 한다.
<br/>

#### 암시적 인텐트
* 인텐트가 인텐트 필터 중 하나를 통과한 경우에만 앱 구성 요소에 암시적 인텐트를 전달.(어느 앱을 사용할지 선택하도록 하고자 할때)

#### 명시적 인텐트
* 항상 자신의 대상에게 전달.(구성요소가 어떤 인텐트 필터를 선언하든 무관)
<br/><br/>  

### IntentFilter의 하위요소
##### - &nbsp; < action > : name 속성에서 허용된 인텐트 작업을 선언한다. 문자열 값이어야 한다.
##### - &nbsp; < data > : 허용된 데이터 유형을 선언한다. 하나 이상의 속성을 사용하여 데이터 URI와 MIME유형을 나타낸다.
##### - &nbsp; < category > : name 속성에서 허용된 인텐트 카테고리를 선언한다. 문자열 값이어야 한다.




<!-- ## 항목
* [리눅스 기본 명령어](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_basicCommand.md)
* [리눅스 Su와 Su - 의 차이점](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_Su.md)
 -->
