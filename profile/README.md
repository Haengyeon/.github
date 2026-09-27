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

| **온보딩** | **기본 정보 입력** | **취향 관심사 입력** | **수락·결제** |**매칭 조건 설정** |
|:----------------:|:----------------:|:----------------:|:----------------:|:----------------:|
| <img width="130" alt="KakaoTalk_Photo_2026-09-27-12-03-24" src="https://github.com/user-attachments/assets/b2cf6cc9-6080-4304-a09a-1cf2ef1c3172" />| <img width="130"  alt="KakaoTalk_Photo_2026-09-27-15-39-53 002" src="https://github.com/user-attachments/assets/290cbfb3-5dc9-4bfd-b1b1-bdc77716327d" /> |<img width="130" alt="KakaoTalk_Photo_2026-09-27-15-39-53 001" src="https://github.com/user-attachments/assets/01eba829-7002-458a-9db5-26762d531b54" /> |<img width="130" alt="KakaoTalk_Photo_2026-09-27-15-39-54 003" src="https://github.com/user-attachments/assets/363c9442-9538-44f8-a067-3dbf0a5d409b" /> | <img width="130" alt="KakaoTalk_Photo_2026-09-27-15-39-55 005" src="https://github.com/user-attachments/assets/efdebb00-9b2b-4100-baa2-0ae10f7f5d67" />  |

| **테마 선택** | **코스, 스탬프** | **코스(지도)** | **채팅** | **후기, AI영상** |
|:----------------:|:----------------:|:----------------:|:----------------:|:----------------:|
| <img width="130"  alt="KakaoTalk_Photo_2026-09-27-11-55-36 003" src="https://github.com/user-attachments/assets/f1e9f784-934b-4e94-a55b-c35602d9ce8c" /> | <img width="130" alt="KakaoTalk_Photo_2026-09-27-15-59-44" src="https://github.com/user-attachments/assets/e312846a-af93-4721-9cb7-e807a1865165" /> | <img width="130" alt="KakaoTalk_Photo_2026-09-27-15-54-30" src="https://github.com/user-attachments/assets/a1c64af9-3f16-4c62-9a7e-604c767d6d67" />| <img width="130"  alt="KakaoTalk_Photo_2026-09-27-11-55-37 006" src="https://github.com/user-attachments/assets/d936e8b1-485d-4c0a-acb2-24bd9ae670cf" /> |<img width="130" alt="KakaoTalk_Photo_2026-09-27-15-39-57 007" src="https://github.com/user-attachments/assets/67c0ef9c-f696-4894-9ffd-12fd20a3375a" /> |

---
# 🖥️ System Architecture
<p align="center">
<img width="1027" height="757" alt="Image" src="https://github.com/user-attachments/assets/ec4bebd0-5db2-41ce-b8a8-23b872ec0cee" />
</p>

# 🛠️ Tech Stack

<p align="center">
<strong>Frontend</strong><br><br>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=nextjs,tailwind,ts" />
</a>
</p>

<p align="center">
<strong>Backend & Database</strong><br><br>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=nestjs,prisma,postgres" />
</a>
&nbsp;
<img
  src="https://upload.wikimedia.org/wikipedia/commons/a/ab/Swagger-logo.png"
  height="48"
  alt="Swagger"
  title="Swagger"
/>
</p>

<p align="center">
<strong>Infra</strong><br><br>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=gcp,vercel,docker,firebase" />
</a>
&nbsp;
<img
  src="https://cdn.simpleicons.org/googlecloudstorage/4285F4"
  height="48"
  alt="Google Cloud Storage"
  title="Google Cloud Storage"
/>
</p>

<p align="center">
<strong>External API</strong><br><br>
<img
  src="https://upload.wikimedia.org/wikipedia/commons/e/e3/KakaoTalk_logo.svg"
  width="64"
  height="64"
  alt="Kakao Login"
  title="Kakao Login"
/>&nbsp;&nbsp;
<img
  src="https://play-lh.googleusercontent.com/hOXXHuezGl0ur3l7EWTdwEAyybjZQn6ayMokEL_XMV3UJuvLfUrefgovyrngh2UTsT4TvdniwYkqDTkVaBqywv4=w240-h480"
  width="64"
  height="64"
  alt="Kakao Pay"
  title="Kakao Pay"
/>&nbsp;&nbsp;
<img
  src="https://upload.wikimedia.org/wikipedia/commons/3/3c/Korea-Tourism-Organization-en.svg"
  height="52"
  alt="TourAPI"
  title="한국관광공사 TourAPI"
/>&nbsp;&nbsp;
<img
  src="https://upload.wikimedia.org/wikipedia/commons/6/66/OpenAI_logo_2025_%28symbol%29.svg"
  width="64"
  height="64"
  alt="OpenAI API"
  title="OpenAI API"
/>
</p>

<p align="center">
<strong>Collaboration</strong><br><br>
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=figma,notion" />
</a>
</p>

# 🗄️ DataBase
<img width="3342" height="3115" alt="Image" src="https://github.com/user-attachments/assets/2444d426-3929-42de-9227-f225a15ca750" />

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
