# MediPrice

**병원마다 다른 비급여 진료비를 한곳에서 비교합니다.**

도수치료, MRI, 초음파 같은 비급여 진료는 병원이 가격을 정하기 때문에 같은 항목도 병원마다 차이가 큽니다. MediPrice는 건강보험심사평가원(HIRA)이 공개하는 가격 자료를 모아, 내 주변 병원의 가격을 미리 확인할 수 있게 합니다.

## 할 수 있는 일

- **가격 비교**: 비급여 항목을 검색해 병원별 공개 가격을 비교합니다.
- **지도 탐색**: 지도에서 주변 병원과 가격을 함께 봅니다.
- **상황으로 찾기**: "어깨가 아픈데 얼마나 나올까"처럼 상황을 말하면 관련 비급여 항목을 찾아 줍니다. 진단이나 치료 권유는 하지 않습니다.
- **영수증 인식**: 진료비 영수증에서 비급여 항목을 읽어 냅니다.

가격과 병원 수는 모두 HIRA 공공데이터에서 나옵니다. AI는 항목을 찾는 데만 쓰고 숫자를 만들지 않습니다.

## 구성

| 영역 | 하는 일 | 기술 | 저장소 |
| --- | --- | --- | --- |
| 웹 | 서비스 화면, 백엔드 중계(BFF) | Next.js, React, TypeScript | [mediprice-front](https://github.com/mediprice/mediprice-front) |
| 백엔드 | API, 로그인, 리뷰, 즐겨찾기 | Java, Spring Boot | 비공개 |
| 데이터 | HIRA 공공데이터를 매주 DB에 동기화 | Java, Spring Batch, PostgreSQL | [mediprice-batch](https://github.com/mediprice/mediprice-batch) |
| AI | 상황으로 항목 찾기, 음성 질문, 대화 요약 | Python | 비공개 |
| OCR | 진료비 영수증에서 비급여 정보 추출 | Python | 비공개 |

## 팀

| 멤버 | 담당 |
| --- | --- |
| [@khm1102](https://github.com/khm1102) | 프론트엔드, AI 서버, DevOps |
| [@myje0804-create](https://github.com/myje0804-create) | 백엔드 |
| [@Rael0515](https://github.com/Rael0515) | 데이터 배치 |
| [@Dibo-world](https://github.com/Dibo-world) | 영수증 OCR, 음성 질문 |
| [@2da2](https://github.com/2da2) | 디자인 |
