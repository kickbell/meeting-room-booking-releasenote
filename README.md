# 릴리즈 노트

### 버전관리

| NO | Version | Change Note | Release Date | Author |
| --- | --- | --- | --- | --- |
| 4 | 1.1.2 | 기능 수정<br>디자인 수정 | 2025.07.17 | 김종찬  |
| 3 | 1.1.1 | 버그 수정<br>디자인 수정 | 2025.07.16 | 김종찬  |
| 2 | 1.1.0 | 유효성 검증 로직 추가<br>도메인, 이메일 연결<br>디자인 수정  | 2025.07.15 | 김종찬 |
| 1 | 1.0.0 | 세미나 발표 | 2025.07.02 | 김종찬  |

### 1.1.2v 릴리즈 노트

- 메일 참석자에 예약자도 포함되도록 수정 
- 메일 발신자 '케이스마텍'으로 수정  
- 릴리즈 노트가 변경될 때마다 Github Action을 활용한 자동 업데이트 추가
- 룸 상세, 예약하기 화면 borderRadius 값 수정 

![](https://uygiaejuijgwotpuiltj.supabase.co/storage/v1/object/public/contents//release_note_112_1.png)
![](https://uygiaejuijgwotpuiltj.supabase.co/storage/v1/object/public/contents//release_note_112_2.png)


### 1.1.1v 릴리즈 노트

- 오늘 이전의 날짜로는 예약이 불가하도록 변경 
- 릴리즈 노트 화면 왼쪽 x버튼 제거 
- 회의실 상세화면, 예약하기 화면 디자인 수정 
- 내 예약목록 화면 디자인 수정 

### 1.1.0v 릴리즈 노트

- 새 예약 생성시 유효성 검증
- 회의실, 회의제목 값 필수
- KST 기준 현재 날짜, 시간 이후에만 예약이 가능하도록 수정
- 시작 예약일자와 종료 예약일자가 일치하도록 수정
- 같은 시간, 같은 장소의 회의가 중복되지 않도록 수정

![스크린샷 2025-07-15 14.10.45.png](https://uygiaejuijgwotpuiltj.supabase.co/storage/v1/object/public/contents//release_note_110_1.png)

- 반복 예약시 중간에 겹치는 예약이 있을 때 대응 추가
- 주간회의 같은 매주 반복예약 생성 시 중간에 다른 예약이 겹치게 되면 경고창 알림
- 중복되는 해당 예약을 제외하고 나머지 예약을 생성하도록 구현
- 반복예약의 우선순위가 높다면, 중복 예약자를 통해 회의시간/장소를 변경하거나 중복 일자에만 새로운 회의 예약을 잡을 것을 권고

![스크린샷 2025-07-15 14.12.14.png](https://uygiaejuijgwotpuiltj.supabase.co/storage/v1/object/public/contents//release_note_110_2.png)

- 고객센터 화면 추가

![스크린샷 2025-07-15 14.10.45.png](https://uygiaejuijgwotpuiltj.supabase.co/storage/v1/object/public/contents//release_note_110_3.png)

- 최초 로그인시 비밀번호 재설정 권고
- 최초 비밀번호를 통한 로그인시 비밀번호 재설정 화면으로 즉시 이동
- 최초 비밀번호를 변경하지 않고 사용할 수도 있으나, 최초 비밀번호를 변경하지 않으면 로그인 할 때마다 비밀번호 재설정 화면으로 이동시켜서 재설정 유도
- 최초 비밀번호가 변경된다면, admin 화면에서 ‘비밀번호 변경됨’으로 표시되도록 대응

![image.png](https://uygiaejuijgwotpuiltj.supabase.co/storage/v1/object/public/contents//release_note_110_4.png)

## 1.0.0v 릴리즈 노트

### 세미나 발표

- 주요 기능 설명
- 개발 방법 소개
- 배포, 유지보수, 관리 방법 소개
- 비용, 피드백 수정
