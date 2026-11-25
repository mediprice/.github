<h1 align="center">
  <img src="https://raw.githubusercontent.com/mediprice/.github/main/profile/logo.png" alt="MediPrice" width="160"><br />
  MediPrice
</h1>

<h4 align="center">
병원마다 다른 비급여 진료비를 한곳에서 비교합니다
</h4>

<p align="center">
  <a href="#소개">소개</a> •
  <a href="#주요-기능">주요 기능</a> •
  <a href="#프로젝트-구조">프로젝트 구조</a> •
  <a href="#기술-스택">기술 스택</a> •
  <a href="#참고-자료">참고 자료</a>
</p>

<div align="center">

| <img src="https://github.com/khm1102.png" width="100px;"/><br /><sub><b>김현민</b></sub><br />[khm1102](https://github.com/khm1102) | <img src="https://github.com/myje0804-create.png" width="100px;"/><br /><sub><b>myje0804</b></sub><br />[myje0804-create](https://github.com/myje0804-create) | <img src="https://github.com/Rael0515.png" width="100px;"/><br /><sub><b>Rael0515</b></sub><br />[Rael0515](https://github.com/Rael0515) | <img src="https://github.com/Dibo-world.png" width="100px;"/><br /><sub><b>Dibo</b></sub><br />[Dibo-world](https://github.com/Dibo-world) | <img src="https://github.com/2da2.png" width="100px;"/><br /><sub><b>hee</b></sub><br />[2da2](https://github.com/2da2) |
| :---: | :---: | :---: | :---: | :---: |
| Frontend, AI, DevOps | Backend | Data Batch | OCR, Voice AI | Design |

</div>

## 소개

도수치료, MRI, 초음파 같은 비급여 진료는 병원이 가격을 정하기 때문에 같은 항목도 병원마다 차이가 큽니다. MediPrice는 건강보험심사평가원(HIRA)이 공개하는 가격 자료를 모아, 내 주변 병원의 가격을 미리 확인할 수 있게 합니다.

가격과 병원 수는 모두 HIRA 공공데이터에서 나옵니다. AI는 항목을 찾는 데만 쓰고 숫자를 만들지 않습니다.

## 주요-기능

- **가격 비교**: 비급여 항목을 검색해 병원별 공개 가격을 비교합니다.
- **지도 탐색**: 지도에서 주변 병원과 가격을 함께 봅니다.
- **상황으로 찾기**: "어깨가 아픈데 얼마나 나올까"처럼 상황을 말하면 관련 비급여 항목을 찾아 줍니다. 진단이나 치료 권유는 하지 않습니다.
- **영수증 인식**: 진료비 영수증에서 비급여 항목을 읽어 냅니다.

## 프로젝트-구조

| 영역 | 하는 일 | 저장소 |
| --- | --- | --- |
| Web | 서비스 화면, 백엔드 중계(BFF) | [mediprice-front](https://github.com/mediprice/mediprice-front) |
| Backend | API, 로그인, 리뷰, 즐겨찾기 | 비공개 |
| Data | HIRA 공공데이터를 매주 DB에 동기화 | [mediprice-batch](https://github.com/mediprice/mediprice-batch) |
| AI | 상황으로 항목 찾기, 음성 질문, 대화 요약 | 비공개 |
| OCR | 진료비 영수증에서 비급여 정보 추출 | 비공개 |

## 기술-스택

### Frontend

[![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://simpleicons.org/?q=nextdotjs)
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://simpleicons.org/?q=react)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://simpleicons.org/?q=typescript)
[![TanStack Query](https://img.shields.io/badge/TanStack%20Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white)](https://simpleicons.org/?q=reactquery)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://simpleicons.org/?q=tailwindcss)

### Backend & Data

[![Java](https://img.shields.io/badge/Java%2021-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://simpleicons.org/?q=openjdk)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)](https://simpleicons.org/?q=springboot)
[![Spring Batch](https://img.shields.io/badge/Spring%20Batch-6DB33F?style=for-the-badge&logo=spring&logoColor=white)](https://simpleicons.org/?q=spring)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://simpleicons.org/?q=postgresql)

### AI

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://simpleicons.org/?q=python)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://simpleicons.org/?q=fastapi)
[![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://simpleicons.org/?q=googlegemini)

### Infra & DevOps

[![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white)](https://simpleicons.org/?q=proxmox)
[![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://simpleicons.org/?q=ubuntu)
[![Cloudflare Tunnel](https://img.shields.io/badge/Cloudflare%20Tunnel-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)](https://simpleicons.org/?q=cloudflare)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://simpleicons.org/?q=vercel)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://simpleicons.org/?q=docker)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)](https://simpleicons.org/?q=githubactions)

### 외부 연동

[![Naver Maps](https://img.shields.io/badge/Naver%20Maps-03C75A?style=for-the-badge&logo=naver&logoColor=white)](https://www.ncloud.com/product/applicationService/maps)

## 참고-자료

- [건강보험심사평가원 비급여 진료비 정보](https://www.hira.or.kr/npay/index.do)
- [공공데이터포털](https://www.data.go.kr/)
