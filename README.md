## `CoolTime`: 공용세탁기의 잔여시간을 애플리케이션으로 실시간 확인가능한 시스템
> **Project Period** : 2019.10.15 ~ 2019.11.29   
> **Description** : 교내 기숙사 세탁기는 공용세탁기로 사용하는 사람이 많다. 그로 인해 잦은 고장이 일어났고 세탁하는 양에 따라 타이머가 정확하지 않은 문제들이 빈번히 발생하였다. 실제로 이를 직접 여러 번 겪어보았고 불편함을 해소시키고자 이 시스템을 구현하였다.

1. Application

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<메인화면>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<내 타이머>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<실시간 사용 현황>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<설정><br>
&nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/50947775/106421815-c3f39e80-64a0-11eb-9624-d4251efa0df2.jpg" width="150" height="300">&nbsp; <img src="https://user-images.githubusercontent.com/50947775/106422558-26996a00-64a2-11eb-9c87-f9fbc7f9be1e.jpg" width="150" height="300"> &nbsp;<img src="https://user-images.githubusercontent.com/50947775/106422438-edf99080-64a1-11eb-82ae-807c6a841fb7.jpg" width="150" height="300"> &nbsp; <img src="https://user-images.githubusercontent.com/50947775/106422708-66605180-64a2-11eb-9cf5-4712e13a67e5.jpg" width="150" height="300">

* 메인화면   
애플리케이션을 동작시키면 가장 먼저 나타나는 페이지로 사용자는 모든 화면 및 설정에 접근 가능하다.<br>
* 내 타이머   
현재 저장된 세탁기가 없다면 0시0분으로 고정된다.   
현재 저장된 세탁기가 있다면 남은 시간이 실시간으로 출력된다.<br>
* QR코드   
접근 즉시 리더기 실행된다.   
QR코드를 읽으면 내 타이머로 세탁기의 시간이 자동으로 이동한다.   
세탁기의 값이 이미 존재하는 경우 새로 할당된다.<br>
* 실시간 사용 현황   
옷 이미지 클릭 시 하단에 사용가능 여부 내용을 확인할 수 있다.   
색이 있는 옷 이미지는 사용 중인 세탁기이며, 클릭 시 남은 시간 확인 가능하다.   
색이 없는 옷 이미지는 사용 가능한 세탁기이다.<br>
* 설정   
'알림 켜기'를 켜놓은 경우 설정한 시간에 알람이 울린다.   
'남은 자리 알림'을 켜놓은 경우 현재 남은 세탁기가 1개 이상 존재할 때 노티피케이션으로 알려준다.   
'알림음 선택'을 통해 사용자가 원하는 알림음으로 변경 가능하다.<br>

2. Raspberry Pi   
&nbsp;<img src="https://user-images.githubusercontent.com/50947775/161921909-b38a378c-cd44-434a-98cf-f7ff5c7abafc.jpg" width="300" height="200">   
세탁기의 타이머를 구현하기 위해 라즈베리파이에 세그먼트를 연결하여 구성하였다.

## Result   
[![세탁기 예약 시스템](https://img.youtube.com/vi/rt-ju-J1BGk/0.jpg)](https://www.youtube.com/embed/rt-ju-J1BGk?t=0s)

## Environment   
AndoidStudio : 애플리케이션 구현환경   
Firebase : 실시간 데이터 통신환경   
Python : 라즈베리파이 동작 실행환경   

## Contact
email: khyunji9@naver.com
