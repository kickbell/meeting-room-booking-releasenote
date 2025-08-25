# 회의실 예약 구독하기 가이드 문서

회의실 예약 프로그램 1.3.0v(2025.08.25)부터 구독하기 기능이 지원됩니다. 구독하기 기능은 [https://icalendar.org/RFC-Specifications/iCalendar-RFC-5545/](https://icalendar.org/RFC-Specifications/iCalendar-RFC-5545/) 표준을 통해 지원되고 있습니다.

> **iCalendar**
>
> 캘린더 데이터 교환을 위한 제안된 인터넷 표준 (RFC 5545)으로, 1998년 IETF(인터넷 기술 표준화 기구)에 의해 최초 정의되었고 [RFC 5545](https://www.google.com/search?q=https://www.google.com/search%3Fsca_esv%3D9687d88dd609da73%26cs%3D0%26sxsrf%3DAE3TifNWNf2wPvGPq4RDyVWs40c2gyqFGw%253A1756110180585%26q%3DRFC%2B5545%26sa%3DX%26ved%3D2ahUKEwi1g9CbxKWPAxXq5DQHHZI1L1sQxccNegQIAhAC%26mstk%3DAUtExfBOz8GTH5vWpoa9eJ_iqXmPLEAApeSAgZ1msH01oK_JYb5Ndv3f6u_HAeFK4KgGI7D7-kmdFX4VtfFUtggv3p0yOpliPMAzxtq3jbUyxs79Cl3xcAEecK8bFCYaS616_CXjtDoLgDUS-BgQmCymbCrhha-F8EnTO3sJHoMWFQnYTggdg4P02RqOJfo6_EPYQ4DTgoWztAocp24oDBTpATxRbIQ5isaGgGeazIUQI45AliwqDRkMful5-lhz0kexfq0w4zkVfH8JxcNrp4uUqQKr%26csui%3D3)에서 최신으로 업데이트되었습니다. 이 표준은 ".ics" 확장자를 가진 파일의 구조와 내용을 정의하며, 구글 캘린더, 마이크로소프트 아웃룩 등 다양한 캘린더 프로그램에서 사용되어 서로 다른 캘린더 간에 일정을 공유하고 상호 운용성을 높이는 데 기여합니다.

```jsx
//iCal 형식의 공개주소
https://calendar.google.com/calendar/ical/77518f3e2c6ed03625a9af2e568a9933085c799eab415f30b8aae822f44d9e59%40group.calendar.google.com/public/basic.ics
```

사용법은 간단합니다. 현재 회의실 예약 시스템은 특정 Google 계정의 Calener API를 통해 예약되는 CREATE, UPDATE, DELETE 이벤트가 동기화되고 있습니다.

![Image 2](https://github.com/user-attachments/assets/7f43cadb-a57f-470f-aec4-dc2f00457b9c)


따라서 위에 나와있는 `iCal 형식의 공개주소`만 구독을 해주시면 본인이 사용하시는 주 캘린더(네이버 캘린더, 맥OS 캘린더, 구글 캘린더)에서도 회의실 예약 내역을 확인하실 수 있어서 서비스의 사용성이 향상되는 효과가 있습니다. (단, 보는 것만 가능하며 생성, 삭제, 수정은 여전히 회의실 예약 서비스에서만 가능합니다.)

-----

## GOOGLE 캘린더

### 구독

구글 캘린더는 워낙 범용성이 넓어서 어디든 사용이 가능합니다. 특히 window를 사용하시는 분들께서는 window 기본 캘린더에서 iCal 형식을 아직 지원하지 않고 있기 때문에 사용하시면 좋겠습니다.

![Image 1](https://github.com/user-attachments/assets/2fd18a35-c7cb-4ad6-8d34-bfea35097605)


캘린더 좌측 슬라이드바 - 다른 캘린더 오른쪽에서 + 버튼 - URL로 추가를 눌러줍니다.

![Image 3](https://github.com/user-attachments/assets/11763216-7683-4774-9bdc-42bb99da2caa)

공유된 iCal 형식의 주소를 입력하고 캘린더 추가 버튼을 눌러줍니다. 끝입니다.

![Image 4](https://github.com/user-attachments/assets/3640bf97-f87a-4576-a123-e5cd94f068c7)

### 구독 취소

추가한 캘린더에서 아래와 같이 X 버튼을 눌러줍니다.

![Image 5](https://github.com/user-attachments/assets/c6a15300-ce49-4f31-8b5a-7fe68debc8fd)

아래에서 캘린더 삭제 버튼을 눌러줍니다.

![Image 6](https://github.com/user-attachments/assets/25440c8d-b49f-4f62-b162-f9e72e7ca715)

-----

## APPLE 캘린더

### 구독

MacOS 사용자께서는 기본 캘린더에서 iCal 형식이 지원됩니다. 캘린더 앱을 열고 파일 - 새로운 캘린더 구독… 을 클릭합니다.

![Image 7](https://github.com/user-attachments/assets/a50622da-cc25-4a32-a589-d2e80d9e461c)

공개된 iCal 주소를 입력합니다.

![Image 8](https://github.com/user-attachments/assets/0ed3eb8e-195e-4115-b20f-8e76934fd20f)

아래에서 캘린더 이름과 알림 여부, 저장할 위치, 새로 고침 간격 등을 수정할 수 있습니다.

![Image 9](https://github.com/user-attachments/assets/daa124c6-d0e3-4858-8dac-5ff8295b90be)

완료되면 구독 캘린더의 내역이 보이게 됩니다.

![Image 10](https://github.com/user-attachments/assets/504bb238-0130-4ada-ac84-6f8fb2e0c4a6)

### 구독 취소

취소도 매우 간단합니다. 구독한 캘린더 우클릭 - 구독 취소를 클릭합니다.

![Image 11](https://github.com/user-attachments/assets/ca822388-4598-42d7-a7f5-9dcbda67c5f1)

구독 취소를 입력해줍니다. 끝입니다.

![Image 12](https://github.com/user-attachments/assets/3dd5650f-b426-486d-901e-a36bed75c177)

-----

## NAVER 캘린더

### 구독

NAVER를 메인으로 이용하신다면 네이버 캘린더 화면으로 이동합니다. 좌측 사이드바 아래쪽의 구독 캘린더 - 오른쪽 + 버튼 - URL로 구독하기를 클릭합니다.
![Image 14](https://github.com/user-attachments/assets/e895fe72-d566-45b5-8359-c7a7fe10f66a)


공개된 iCal 형식의 주소를 입력하고, 캘린더명과 색상을 변경할 수 있습니다. 저장을 클릭합니다.
![Image 15](https://github.com/user-attachments/assets/47bf73c2-f177-4599-8512-ec857b25d72d)


아래와 같이 구독 캘린더의 내역이 보이게 됩니다.

![Image 13](https://github.com/user-attachments/assets/136b91a7-2710-41f5-80f4-d0a7cbc421a8)


### 구독 취소

구독 취소는 같은 메뉴에서 우측 톱니바퀴 모양 - 캘린더 설정을 클릭합니다.

![Image 16](https://github.com/user-attachments/assets/9a655f86-5b5b-4939-bc72-80d975c695a3)


그러면 메인화면에 캘린더 목록이 나오는데요. 구독한 캘린더에가서 구독해지라고 적혀있는 부분을 클릭합니다.

![Image 17](https://github.com/user-attachments/assets/527ed744-e27b-44a2-b5ad-326bf0c7dc5b)

그러면 중앙 상단에 아래와 같은 팝업이 뜨고 확인을 클릭하면 끝입니다.

![Image 18](https://github.com/user-attachments/assets/1f07284f-16d1-4a66-b906-74c2c226a293)
