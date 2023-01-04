

### 이모탈 서비스(Immortal Service)란?
##### - &nbsp; 죽지않는 서비스이다.
##### - &nbsp; 안드로이드 서비스(포그라운드, 백그라운드, 바인드) 중 "포그라운드"를 사용한다.
<br/><br/>

### 이모탈 서비스를 사용해야 할 때(=서비스가 죽지 말아야 할 경우)는 언제인가?
##### 1. 앱을 종료 했을 때 -> 기본 서비스를 사용하면 막을 수 있다.
##### 2. 폰을 재시작 했을 때 -> 폰 재시작이 이벤트를 받아 서비스를 재시작
##### 3. Task Kill을 했을 -> startForeground 를 통해서 서비스를 죽지 않게 함.
<br/><br/>

#### code 예시
> 메인 서비스를 A라고 한다면, 서브 서비스 B를 만들어서 서로서로 감시하여 onDestroy()가 호출된다면, <br/>
AlarmManager를 통해 다시 서비스를 킨다. <br/>
따라서 서비스 A가 모종의 이유로 죽으면, AlarmManager가 호출되어 서비스B가 실행되고 다시 서비스A가 실행된다.<br/>
반대로, 서비스 B가 죽는다면 서비스A를 통해 서비스B가 다시 실행된다.

```
// Service A
class ServiceA : Service() {
    override fun onStartCommand() {      
        if (/**intent?.getStringExtra("type")이 B이면*/){
            startService(serviceB)
        }
    }

    override fun onDestroy() {
        // 알람 매니저 호출
    }

    private fun callAlarmManger() {
        // 알람 매니저 등록
    }
}

class AlarmReceiver : BroadcastReceiver() {
    override fun onReceive(context: Context, intent: Intent) {
        if(/**버전 오레오 이상이면*/){
            intent.putExtra("type", "A")
            startForegroundService(serviceB)
        }else {
            startService(serviceA)
        }
    }
}
```


```
// Service B
class ServiceB : Service() {
    override fun onStartCommand() {      
        if (/**intent?.getStringExtra("type")이 A이면*/){
            startService(serviceA)
        }
    }

    override fun onDestroy() {
        // 알람 매니저 호출
    }

    private fun callAlarmManger() {
        // 알람 매니저 등록
    }
}

class AlarmReceiver : BroadcastReceiver() {
    override fun onReceive(context: Context, intent: Intent) {
        if(/**버전 오레오 이상이면*/){
            intent.putExtra("type", "B")
            startForegroundService(serviceA)
        }else {
            startService(serviceB)
        }
    }
}
```

  

## 참조
* https://jwl-97.github.io/post/Immortal_service_20210301/
<!-- * [리눅스 Su와 Su - 의 차이점](https://github.com/jwsimhj97/TIL/blob/main/WORK/Linux/Linux_Su.md)
 -->
