<img width="851" alt="1" src="https://github.com/MoonKimTeam/.github/assets/87420630/4d85da1e-606d-4d85-84ef-b20e977251cb">

## 서비스
종류: 콘서트 티켓 예매

## 기술 스택
<img src="https://img.shields.io/badge/Kotlin-7F52FF.svg?&style=flat&logo=Kotlin&logoColor=white" alt="Java"><img src="https://img.shields.io/badge/Spring_Boot 3.x-6DB33F.svg?&style=flat&logo=SpringBoot&logoColor=white" alt="Spring Boot"><img src="https://img.shields.io/badge/MySQL-%2300f.svg?style=flat&logo=mysql&logoColor=white" alt="MySQL">
<img src="https://img.shields.io/badge/Redis-%23DD0031.svg?style=flat&logo=redis&logoColor=white" alt="Redis"><img src="https://img.shields.io/badge/Apache%20Kafka-000?style=flat&logo=apachekafka" alt="Apache Kafka">

## 구조
- 유저 -> 공연(티켓, 장소, 예매) -> 결제 -> 알림

### 유저
- 이름/생년월일/비밀번호/성별/전화번호/이메일/주소/상세주소/계좌번호 등...
- 로그인/ 가입/수정/탈퇴
- 이메일 아이디
- 주문 가능 상태 여부(휴면, 탈퇴 여부)

### 공연
- 티켓
	- 공연 이름/공연장/설명/콘서트 시작일시/종료일시/예매 시작일시/종료일시/예매 가능 여부/나이 제한 여부...
- 공연장
	- 좌석 수/주소/위치...

### 예매
- 공연 id/예매 수량/좌석 위치/예매 일시/결제 완료 여부/...

### 결제
- 예매 id/ 결제 금액/회원 ID/ 결제자 이름/결제 수단/카드 및 은행번호/카드 번호...

알림
- 알림 제목/내용/회원 아이디
- 알림 방식: 메일


## 기타

공연, 결제 간에 보상 트랜잭션 사용
