### 브로드캐스트(BroadCast)란?
##### - &nbsp; 로컬 LAN 상에 붙어있는(브로드캐스트 도메인 안에 있는) 모든 네트워크 장비들에게 보내는 통신
##### - &nbsp; ex) 스마트폰에서 전원 충전 및 해제, 비행기모드 돌입, 앱 설치완료 등등의 이벤트를 말한다.
<br/><br/>

#### 브로드캐스트 list
* ACTION_BOOT_COMPLETED : 부팅이 끝났을 때 (RECIVE_BOOT_COMPLETED 권한 등록 필요)
* ACTION_CAMERA_BUTTON : 카메라 버튼 눌렸을 때
* ACTION_DATE_CHANGED, ACIONT_TIME_CHANGED : 폰의 날짜, 시간이 수동으로 변했을 때 (설정에서 수정했을 때)
* ACTION_SCREEN_OFF, ACTION_SCREEN_ON : 화면 ON, OFF
* ACTION_AIRPLANE_MODE_CHANGED : 비행기 모드
* ACTION_BATTERY_CHANGED, ACTION_BATTERY_LOW, ACTION_BATTERY_OKAY : 배터리 상태 변화
* ACTION_PAKAGE_ADDED, ACTION_PACKAGE_CHANGED, ACTION_PACKAGE_DATA_CLEARED, ACTION_PACKAGE_INSTALL, ACTION_PACKAGE_REMOVED, ACTION_PACKAGE_REPLACED, ACTION_PACKAGE_RESTARTED : 어플 설치/제거
* ACTION_POWER_CONNECTED, ACTION_POWER_DISCONNECTED : 충전관련
* ACTION_REBOOT, ACTION_SHUTDOWN : 재부팅/종료
* ACTION_TIME_TICK : 매분마다 수신
* android.provider.Telephony.SMS_RECEIVED : sms수신 (RECEIVE_SMS 권한 필요)



## 관련내용
* [브로드캐스트리시버란?](https://github.com/jwsimhj97/TIL/blob/main/WORK/AndroidStudio/AndroidStudio_BroadcastReceiver.md)
