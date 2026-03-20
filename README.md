# 안녕하세요, 백엔드 개발자를 준비 중인 정성준입니다. 👋

Java와 Spring 기반으로  
사용자 흐름을 고려한 웹 서비스를 만드는 것을 좋아합니다.

- JWT / OAuth2 기반 인증 구조 학습 및 구현
- 예약 / 결제 / 게시판 / 파일 업로드 등 실서비스 기능 구현 경험
- MyBatis, Oracle SQL, REST API 중심 백엔드 개발
- 팀 프로젝트를 통해 협업, 역할 분담, 발표 경험 축적

---

## 🙋 About Me

- 풀스택 개발자로 취업 준비 중이며, 백엔드 개발 역량을 중심으로 성장하고 있습니다.
- 단순 구현보다 **왜 이렇게 설계하는지**를 이해하는 방식으로 공부합니다.
- 프로젝트를 진행하며 인증, 예약 충돌 검증, 결제 처리, 파일 처리, 게시판 기능 등을 직접 구현했습니다.
- 협업 과정에서 문서화, 발표 준비, 기능 설명까지 함께 경험했습니다.

---

## 🛠 Tech Stack

### Backend
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-000000?style=for-the-badge&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

### Frontend
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white)

### Database
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### Tools
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white)

---

## 📌 Projects

### 1. 맛조아 - 맛집 리뷰 플랫폼
- **기간**: 10일
- **인원**: 3인 팀 프로젝트
- **기술 스택**: JSP / Servlet / MySQL / Tomcat
- **담당 역할**
  - 로그인 / 회원가입 기능 구현
  - ERD 설계 및 DB 구조 정리
  - 사용자 / 가게 / 게시글 관계 설계
  - 일부 게시판/리뷰 기능 수정 및 연동 보완

**프로젝트 설명**  
사용자가 음식 카테고리를 기준으로 맛집을 탐색하고 리뷰를 남길 수 있는 플랫폼입니다.

**배운 점**
- 테이블 관계 설계와 정규화의 중요성
- DAO / Service 분리 구조의 필요성
- 실제 기능 구현에서 SQL과 백엔드 로직이 어떻게 연결되는지 경험

---

### 2. 튜터링고 - 튜터/튜티 매칭 플랫폼
- **기간**: 3주
- **인원**: 4인 팀 프로젝트
- **기술 스택**: Spring Boot / MyBatis / Spring Security / JWT / OAuth2 / Toss Payments / OpenAI API
- **담당 역할**
  - JWT 인증 필터 및 인증 흐름 구현
  - 튜터 마이페이지 기능 구현
  - 예약 시간 검증 로직 구현
  - 결제 완료 후 예약 상태 변경 트랜잭션 처리

**프로젝트 설명**  
튜터와 튜티를 연결하고, 수업 예약 및 결제까지 관리할 수 있는 서비스입니다.

**핵심 구현**
- `JwtAuthenticationFilter`를 통한 토큰 검증 및 `SecurityContext` 인증 정보 저장
- 예약 이동/변경 시 서버에서 시간 충돌과 과거 시간 여부 재검증
- Toss 결제 완료 후 예약 상태 반영
- OAuth2 소셜 로그인과 JWT 인증 구조 적용

**배운 점**
- 인증은 단순 로그인 기능이 아니라 요청 흐름 전체와 연결된다는 점
- 클라이언트 검증만으로는 부족하고 서버 검증이 필수라는 점
- 협업 시 기능 구현만큼 문서화와 의사소통도 중요하다는 점

---

## 🧩 Troubleshooting

### JWT 인증 흐름 이해
처음에는 토큰 검증 이후 인증 정보가 어디에 저장되고 어떻게 사용되는지 헷갈렸지만,  
필터 → SecurityContext → Controller 흐름을 정리하면서 요청 단위 인증 구조를 이해하게 되었습니다.

### 예약 충돌 검증
예약 기능은 화면에서만 막으면 충분하다고 생각했지만,  
실제로는 서버에서 한 번 더 검증해야 데이터 무결성을 보장할 수 있다는 점을 배웠습니다.

### Git 협업 경험
브랜치 병합 과정에서 코드 충돌과 손상 문제를 겪으며,  
기능 단위 커밋과 역할 분리, 머지 전 확인 과정의 중요성을 체감했습니다.

---

## 📊 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=여기에본인아이디&show_icons=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=여기에본인아이디&layout=compact)

---

## 📫 Contact

- Email: your-email@example.com
- GitHub: https://github.com/여기에본인아이디

---

## ✨ Pinned Repository 추천
- 팀 프로젝트 백엔드 저장소
- 리액트 리팩토링 저장소
- 미니 프로젝트 저장소
- SQL / 알고리즘 / 학습 정리 저장소
