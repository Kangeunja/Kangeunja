## 👋 안녕하세요:)
디테일과 디자인 감각으로 사용자 경험까지 놓치지 않는
1년차 프론트엔드 개발자 강은자입니다.

# 🏝️ Jeju Travel Portal (제주 관광 포털)
> **제주도의 관광지, 축제, 역사 정보를 한눈에 확인하는 관광 포털 서비스**
> 
> **개발 기간**: 2025.08 ~ 2025.10 (개인 프로젝트)  
> **배포 주소**: [https://jeju-portfolio.netlify.app/](https://jeju-portfolio.netlify.app/)  
> **깃허브 주소**: [https://github.com/Kangeunja/Jeju-front](https://github.com/Kangeunja/Jeju-front)  
> **Figma 주소**: [프로젝트 디자인 기획안 바로가기](https://www.figma.com/design/vEg5woMNDF9BaRgZhbe5pW/%EC%A0%9C%EC%A3%BC%EA%B4%80%EA%B4%91?node-id=371-76&p=f&t=btnuuGPOzxy6IONI-0](https://www.figma.com/design/vEg5woMNDF9BaRgZhbe5pW/%EC%A0%9C%EC%A3%BC%EA%B4%80%EA%B4%91?node-id=371-76))
---

## 📺 Project Preview
<img width="245" height="180" alt="iMac-mock-up-diferents-views copy1 1" src="https://github.com/user-attachments/assets/c55b5b51-0648-4731-9b6d-23e098e74960" />

---


## 🛠 Tech Stack
- **Frontend**: React, TypeScript, Axios
- **Library**: Swiper (UI Animation), MSW (Mocking)
- **Design & Dev Ops**: Figma, GitHub, Netlify, Render

---

## 📌 Key Features (담당 기능)
- **UI/UX**: React 기반의 재사용 가능한 컴포넌트 설계 및 구현
- **Animation**: Swiper 라이브러리를 활용한 역동적인 배너 및 리스트 UI 구현
- **Data Fetching**: MSW를 활용하여 실제 서버 없이도 원활한 API 호출 환경 구축
- **Filtering**: 월별 필터 기능을 통해 선택한 조건에 맞는 데이터를 실시간으로 갱신하는 구조 설계

---

## 🔍 Trouble Shooting & Experience
### 1️⃣ 배포 환경에서의 MSW 동작 이슈 해결
- **문제**: 로컬 환경에서는 정상 작동하던 Mock 데이터가 Netlify 배포 후 작동하지 않는 문제 발생.
- **원인**: MSW는 브라우저 서비스 워커를 이용하는 도구로, 배포 환경의 API 설정과 차이가 있음을 확인.
- **해결**: 개발 환경(`development`)에서만 MSW가 실행되도록 분기 처리를 적용하고, 배포 환경에서는 실제 API 환경을 고려한 데이터 흐름을 설계하며 **Mock 데이터 활용 방식과 환경별 환경 변수 관리**의 중요성을 학습했습니다.

### 2️⃣ 이미지 렌더링 경로 최적화
- **문제**: 프로젝트 빌드 및 배포 후 일부 이미지가 엑스박스로 표시되는 현상 발생.
- **원인**: 상대 경로 설정 방식이 빌드된 정적 파일 구조와 맞지 않아 발생한 문제임을 파악.
- **해결**: 정적 리소스(Public Assets) 관리 방식을 점검하고 경로 설정 방식을 수정하여 해결했습니다. 이를 통해 **프레임워크별 정적 리소스 처리 프로세스**를 깊이 있게 이해하게 되었습니다.

---

## 📂 Repository Structure
- 기여도: 100% (기획, 디자인, 프론트엔드 전체 담당)

---

## 📚 ReadPick (도서 감상평 및 리뷰 서비스)
> **도서 검색부터 감상평 기록, 리뷰 공유까지 지원하는 도서 커뮤니티 웹서비스**
> 
> **개발 기간**: 2025.03 ~ 2025.07 (2인 프로젝트 / 프론트엔드 전담)  
> **배포 주소**: [https://readpick-front-portfolio.netlify.app/](https://readpick-front-portfolio.netlify.app/)  
> **깃허브 주소**: [https://github.com/Kangeunja/ReadPick-front-portfolio](https://github.com/Kangeunja/ReadPick-front-portfolio)  
> **Figma 주소**: [프로젝트 디자인 기획안 바로가기](https://www.figma.com/design/JfVW6xaVVXDp9eboQJNYiS/ReadPick-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8?node-id=1097-310)

---

### 📺 Project Preview
<img width="245" height="180" alt="iMac-mock-up-diferents-views copy 2" src="https://github.com/user-attachments/assets/40105578-58c8-44df-9e4e-85204ad159b8" />

---

### 🛠 Tech Stack
- **Frontend**: React, TypeScript, Axios
- **Backend/DB**: MySQL (Render 배포)
- **Dev Ops**: GitHub, Netlify (Frontend 배포)
- **Design**: Figma

---

### 📌 Key Features (담당 기능)
- **Auth**: 로그인 상태에 따른 조건부 렌더링 및 사용자 흐름 분기 처리
- **Book Search**: 외부 API 연동을 통한 실시간 도서 검색 기능 구현
- **Review CRUD**: 사용자 리뷰 작성, 수정, 삭제 및 즉각적인 UI 피드백 반영
- **Architecture**: Axios 인스턴스 분리를 통한 공통 설정 및 응답 처리 구조화
- **State Management**: `useState`와 `useSearchParams`를 활용한 URL 상태 동기화 및 탐색 흐름 유지

---

### 🔍 Trouble Shooting & Experience
#### 1️⃣ 토큰 기반 인증 및 세션 유지 구조 설계
- **문제**: 단순 로그인 처리 시 브라우저 종료나 새로고침 후 로그인이 유지되지 않는 문제 발생.
- **해결**: Access Token과 Refresh Token 구조를 도입하여 보안성을 높이고 세션을 안정적으로 유지하는 방식을 적용했습니다. 이를 통해 **토큰 기반 인증 프로세스**를 깊이 있게 이해하게 되었습니다.

#### 2️⃣ 교차 도메인(CORS) 환경에서의 세션 관리
- **문제**: 배포 후 프론트(Netlify)와 백엔드(Render)의 도메인이 달라 사용자 정보를 인식하지 못하는 세션 불안정 현상 경험.
- **해결**: Axios 환경 변수 설정 및 Cookie 속성(SameSite, Secure 등)을 세밀하게 조정하여 해결했습니다. **서로 다른 도메인 환경에서 발생하는 제약 사항**과 해결 방법을 실전에서 경험했습니다.

#### 3️⃣ 환경별 API 주소 관리 자동화
- **문제**: 로컬 테스트와 배포 시마다 API 주소를 수동으로 수정해야 하는 번거로움과 실수 유발.
- **해결**: `.env` 파일을 활용한 환경별 설정 분리를 구축했습니다. 이를 통해 수동 작업 없이 **개발과 배포 사이의 배포 리드 타임을 단축**하고 환경 관리의 중요성을 깨달았습니다.

---

### 📂 Role & Contribution
- **기여도: 프론트엔드 파트 100% 담당**
- UI 컴포넌트 설계부터 API 연동, 배포 환경 구축까지 전 과정 주도
