# 🧭 HAENGYEON 행연
> **관광지를 함께 걷는 여행 동행 매칭 앱**

<p align="center">
<img width="1920" height="1080" alt="Image" src="TODO: 배너 이미지 URL" />
</p>

<!--
---
# 🧑🏼‍💻 How To Start
🔗 [www.haengyeon.site](https://www.haengyeon.site) -->

---
# ✨ Features & Demo

| **회원가입 / 로그인** | **홈** | **매칭** | **결제** | **채팅** | **코스** | **마이페이지** |
|:-------------------:|:------------:|:--------------------:|:----------------:|:----------------:|:----------------:|:----------------:|
| <img src="TODO" width="200" alt="로그인&회원가입"> | <img src="TODO" width="200" alt="홈"> | <img src="TODO" width="200" alt="매칭"> | <img src="TODO" width="200" alt="결제"> | <img src="TODO" width="200" alt="채팅"> | <img src="TODO" width="200" alt="코스"> | <img src="TODO" width="200" alt="마이페이지"> |

---
# 🖥️ System Architecture
<p align="center">
<img width="1205" height="674" alt="Image" src="TODO: 아키텍처 다이어그램 URL" />
</p>

# 🛠️ Tech Stack

<p align="center">
<strong> Frontend <br></strong>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=nextjs,tailwind,ts" />
</a>
</p>

<p align="center">
<strong> Backend <br></strong>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=nestjs" />
</a>
</p>

<p align="center">
<strong> Database <br></strong>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=postgres" />
</a>
</p>

<p align="center">
<strong> External API <br></strong>
<img src="https://img.shields.io/badge/Kakao_Login-FFCD00?style=flat-square&logo=kakao&logoColor=black" />
<img src="https://img.shields.io/badge/Kakao_Pay-FFCD00?style=flat-square&logo=kakao&logoColor=black" />
<img src="https://img.shields.io/badge/한국관광공사_TourAPI-0F9D58?style=flat-square" />
</p>

<p align="center">
<strong> Tool <br></strong>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=figma,notion" />
</a>
</p>

# 🗄️ DataBase
<img width="750" alt="DB ERD" src="TODO: ERD 이미지 URL" />

# 📤 API

<details>
<summary><b>auth</b></summary>

| Method | Path | 설명 |
|---|---|---|
| POST | `/auth/kakao` | 카카오 회원가입/로그인 |
| POST | `/auth/token/refresh` | 액세스 토큰 재발급 |
| DELETE | `/auth/logout` | 로그아웃 |
</details>

<details>
<summary><b>user</b></summary>

| Method | Path | 설명 |
|---|---|---|
| POST | `/users/me/profile` | 프로필 작성 |
| GET | `/users/me/profile` | 프로필 조회 |
| PATCH | `/users/me/profile` | 회원수정 |
| DELETE | `/users/me` | 회원탈퇴 |
| GET | `/users/me/payments` | 결제내역 |
| POST | `/users/me/reports` | 신고 |
| POST | `/user/me/block` | 차단 |
</details>

<details>
<summary><b>home</b></summary>

| Method | Path | 설명 |
|---|---|---|
| GET | `/home/matching-status` | 현재 매칭 상태 조회 |
| POST | `/home/fcm-token` | 알림 수신 토큰 등록 |
| POST | `/home/matching/{matchingId}/accept` | 양쪽 매칭 성사 처리 |
| PATCH | `/home/matching/:matchingId/conditions` | 결제취소(환불 및 조건수정) |
</details>

<details>
<summary><b>matching</b></summary>

| Method | Path | 설명 |
|---|---|---|
| POST | `/matchings` | 매칭조건설정 |
| GET | `/matchings/current` | 현재 매칭 상태 조회 |
| GET | `/matchings/{matchingId}/attempts/{attemptId}` | 매칭 상대 프로필 조회 |
| PUT | `/matchings/{matchingId}/attempts/{attemptId}/response` | 매칭 응답(수락/거절) |
</details>

<details>
<summary><b>payment</b></summary>

| Method | Path | 설명 |
|---|---|---|
| POST | `/payments` | 결제진행 (카카오페이) |
| GET | `/payments` | 결제내역 |
| POST | `/payments/{paymentId}/cancellations` | 결제취소 |
</details>

<details>
<summary><b>chat</b></summary>

| Method | Path | 설명 |
|---|---|---|
| GET | `/chat` | 채팅방 목록 조회 |
| GET | `/chat/{chatId}` | 채팅 잠금/정보 조회 |
| WS | `/chat/{chatId}` | 채팅 메시지 전송 |
| POST | `/chat/:matchingId/report` | 채팅 내 신고 |
</details>

<details>
<summary><b>course</b></summary>

| Method | Path | 설명 |
|---|---|---|
| GET | `/courses/current` | 진행중 코스 조회 |
| GET | `/courses/recommended` | 추천 코스 조회 |
| GET | `/courses/history` | 완료 코스 목록 조회 |
| GET | `/courses/{courseId}` | 특정 코스 상세 조회 |
| POST | `/courses/{courseId}/missions/{missionId}/photos` | 인증샷 촬영/업로드 |
| POST | `/courses/{courseId}/review` | 완료 코스 후기 작성 |
| POST | `/courses/{courseId}/completions` | 코스 완료 처리 |
| GET | `/courses/{courseId}/memory-video` | AI 추억영상 조회 |
</details>

<details>
<summary><b>notification / reward</b></summary>

| Method | Path | 설명 |
|---|---|---|
| POST | `/notifications` | 매칭성사알림(카카오알림) 발송 |
| GET | `/points` | 포인트 조회 |
| GET | `/points/history` | 포인트 내역 |
| GET | `/stamps` | 스탬프 목록 |
| GET | `/stamps/{stampId}` | 스탬프 상세 |
</details>

# 👨‍👩‍👧‍👦 Members

| [김가을](https://github.com/fallkim) | [곽소정](https://github.com/ssojungg) | [장정운](https://github.com/jeongwoonjjang) |
|--------------------------------------|----------------------------------------|--------------------------------------------|
| <img width="210" alt="김가을" src="TODO"/> | <img width="210" alt="곽소정" src="TODO"/> | <img width="210" alt="장정운" src="TODO"/> |
| <div align="center">`Back-end`</div> | <div align="center">`Back-end`</div> | <div align="center">`Front-end`</div> |