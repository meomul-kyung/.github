<div align="center">
  <h1>머물;경(慶) - 경북 인구감소지역 체류형 여행 추천 서비스</h1>
  <p>🏞️ "어디 가서 무엇을 볼 것인가"가 아니라, "왜 이 지역에 머물러야 하는가" 🏞️</p>
</div>

<br/>

<!-- [사진 ①] 메인 이미지 — 서비스 대표 화면 또는 로고
<div align="center">
  <img src="./assets/Main.png" alt="Main" style="border-radius: 10px;"/>
</div>
-->

<br/>

<!-- [링크] 배포 후 주석 해제
<div align="center">
  <a href="">서비스 바로가기</a>
  &nbsp; | &nbsp;
  <a href="">Swagger</a>
  &nbsp; | &nbsp;
  <a href="">Notion</a>
</div>
-->

---

## ✍️ 프로젝트 개요

- **프로젝트명:** 머물;경(慶)
- **프로젝트 형태:** 2026 관광데이터 활용 공모전 (웹·앱 개발 부문) 출품작
- **목표:** 스쳐 가는 관광이 아닌 체류형 여행을 설계하고, 그 여행이 지역에 남긴 기여를 공공 기준으로 환산해 제공하는 서비스 개발
- **대상 지역:** 행정안전부 지정 경상북도 인구감소지역 15개 시·군
- **주요 타겟 사용자:** 지역 여행을 계획하는 20~40대 개인 여행자

---

## ✍️ 프로젝트 소개

### 프로젝트 배경

인구감소지역의 관광은 다음과 같은 문제를 안고 있습니다:

1. **방문은 있으나 체류가 없음:**
   - 대부분의 여행이 당일치기로 한두 곳만 둘러보고 끝남.
   - 방문객 수는 집계되지만, 지역에 실질적으로 남는 것은 적음.

2. **기존 여행 서비스의 한계:**
   - 인기·검색량 순으로 유명 관광지를 나열하는 구조.
   - "얼마나 머물지"는 사용자가 알아서 정해야 하며, 체류를 전제로 설계된 일정이 없음.

3. **여행 정보의 신뢰성 문제:**
   - 운영시간·휴무일 정보의 출처와 최신성이 불분명.
   - 조회에 실패해도 오래된 값이 그대로 노출되어 현장에서 헛걸음이 발생.

**머물;경**은 위 문제를 해결하기 위해 「인구감소지역 지원 특별법」의 **생활인구** 개념을 서비스 한가운데에 놓았습니다.
해당 법에서 체류인구는 *"주민등록지가 아닌 지역을 월 1회 이상 방문해 하루 3시간 이상 머무는 사람"* 으로 정의됩니다.
즉 지역에 필요한 것은 더 많은 방문객이 아니라 **더 오래 머무는 방문객**입니다.

---

### 문제점 해결

- **체류를 전제로 한 일정 설계:** 1박 단위로 관광지·체험 3곳과 음식점 2곳을 배치하고, 여행 기간 중 열리는 지역 축제를 자동 편입하여 "머무는 이유"가 있는 일정을 생성.
- **추천 대상의 한정:** 유명 관광지가 아닌 행정안전부 지정 인구감소지역 15곳만을 대상으로 추천하여, 분산이 필요한 지역으로 여행 수요를 유도.
- **정확성의 구조화:** 모든 외부 조회 결과에 출처와 조회 시각을 함께 제공하고, 실패 시 임의로 채우지 않고 빈칸임을 명시하며, 휴무일은 단정하지 않고 가능성으로 안내.
- **기여의 가시화:** 여행 완료 시 생활인구 산입일수와 예상 소비액을 공개된 공공 기준으로 산출하여, 여행의 끝이 후기가 아닌 지역 기여 기록이 되도록 설계.

---

## 🚀 프로젝트 목표

1. **체류형 여행으로의 전환:**
   - 당일치기 중심의 지역 관광을 1박 이상의 체류형 일정으로 유도.
   - 이동·식사·휴식이 포함된 현실적인 하루 구성 제공.

2. **여행 정보의 신뢰 확보:**
   - 출처·조회 시각 표기와 빈칸 명시로 잘못된 정보로 인한 현장 손해 방지.
   - 휴무 가능성 사전 경고로 헛걸음 감소.

3. **지역 기여의 정량화:**
   - 개인의 여행이 만든 생활인구 산입일수와 소비액을 공공 기준으로 환산.
   - 서비스 전체 누적 기여 현황을 공개하여 지방소멸 대응 효과를 가시화.

---

## 📌 주요 기능

### **0. 소셜 로그인 | 온보딩**

- 카카오 | 구글 | 네이버 소셜 로그인
- 최초 로그인 시 닉네임 설정 후 서비스 진입

<!--
<div align="center">
<img src="./assets/로그인.gif" alt="로그인" style="border-radius: 10px; width: 700px;"/>
</div>
-->

---

### **1. 조건 기반 지역 추천**

- **기능 설명:** 사용자가 선택한 취향·동행 유형·희망 숙박일수를 가중 합산하여, 경북 15개 인구감소지역 중 적합한 3곳을 추천합니다.

- **선택 조건:**
  - 취향 9종: 한옥·유교 / 자연 / 바다 / 걷기 / 힐링 / 음식 / 자전거 / 역사 / 밤하늘
  - 동행 유형 4종: 혼자 / 커플 / 친구 / 가족
  - 희망 숙박일수

- **제공 정보:** 매칭된 취향 태그, 추천 이유, 지역 대표 장소

<!--
<div align="center">
<img src="./assets/지역추천.gif" alt="지역추천" style="border-radius: 10px; width: 700px;"/>
</div>
-->

---

### **2. 체류형 여행 일정 자동 생성**

- **기능 설명:** 선택한 지역과 기간에 맞춰 1박 단위의 여행 일정을 자동으로 생성합니다.

- **주요 과정:**
  1. TourAPI에서 해당 지역의 관광지·체험·음식점 목록을 실시간 조회.
  2. 1박당 관광지·체험 3곳 + 음식점 2곳을 순서대로 배치하고 도착·출발 일정을 포함.
  3. 여행 기간 중 열리는 지역 축제·행사를 자동으로 일정에 편입.

- **추가 기능:** 마음에 들지 않는 항목의 개별 교체, 일정 전체 재생성

<!--
<div align="center">
<img src="./assets/일정생성.gif" alt="일정생성" style="border-radius: 10px; width: 700px;"/>
</div>
-->

---

### **3. 현장 정보 제공**

- **기능 설명:** 일정에 포함된 장소와 이동 구간에 대해, 실제 방문에 필요한 정보를 실시간으로 제공합니다.

| 정보 | 내용 |
|---|---|
| **운영시간·휴무일** | 방문 요일과 대조해 휴무 가능성을 경고. 단정하지 않고 원문과 함께 안내 |
| **날씨** | 여행일까지 3일 이내는 단기예보, 4~10일은 중기예보로 자동 전환 |
| **이동 경로** | 자차는 소요시간·거리·예상 택시요금, 대중교통은 소요시간·요금·환승·경로선을 구간별로 제공 |
| **지역 버스** | 15개 시·군의 공식 버스 시간표 링크와 관내 무료버스 안내 제공 |

<!--
<div align="center">
<img src="./assets/휴무경고.png" alt="휴무경고" style="border-radius: 10px; width: 700px;"/>
</div>

<div align="center">
<img src="./assets/이동경로.png" alt="이동경로" style="border-radius: 10px; width: 700px;"/>
</div>
-->

---

### **4. 지역 스토리 및 관광 정보 제공**

- **기능 설명:** 각 지역의 정체성을 담은 소개와 함께, 한국관광공사 데이터 기반 지역 대표 사진을 제공합니다.
- 단순한 관광지 나열이 아니라 "이 지역이 어떤 곳인가"를 먼저 설명하여, 머물러야 할 이유를 전달합니다.

<!--
<div align="center">
<img src="./assets/지역상세.png" alt="지역상세" style="border-radius: 10px; width: 700px;"/>
</div>
-->

---

### **5. 여행 결과 기반 지역 기여도 산출**

- **기능 설명:** 여행을 완료하면 체류시간과 인원을 바탕으로 지역 기여도를 산출합니다.

- **산출 항목:**
  - 생활인구 산입일수 — 「인구감소지역 지원 특별법」 체류인구 기준(하루 3시간 이상) 적용
  - 예상 소비액 — 2025 국민여행조사 기준 1인 1일 단가 적용
  - 방문 지역 스탬프 수집

- **서비스 전체 누적 기여 현황:** 총 여행 수·여행자 수·누적 체류일수·예상 소비액·지역별 랭킹을 로그인 없이 공개

<!--
<div align="center">
<img src="./assets/기여도.png" alt="기여도" style="border-radius: 10px; width: 700px;"/>
</div>

<div align="center">
<img src="./assets/누적현황.png" alt="누적현황" style="border-radius: 10px; width: 700px;"/>
</div>
-->

---

## 📊 활용 데이터

### 한국관광공사 OpenAPI

| API | 활용 |
|---|---|
| **국문 관광정보 서비스 (TourAPI)** | 지역별 장소 목록, 지역 축제·행사, 콘텐츠 타입, 이용시간·휴무일 조회 — 지역 추천·일정 생성·휴무 경고·대표 사진의 핵심 데이터 |

> TourAPI 응답은 로컬 DB에 저장하지 않고 **요청 시점에 실시간 호출**합니다.
> 출처: ⓒ한국관광공사

### 그 외 데이터

| 데이터 | 활용 |
|---|---|
| 기상청 단기예보 조회서비스 | 여행일 3일 이내 시간별 날씨 |
| 기상청 중기예보 조회서비스 | 여행일 4~10일 하늘상태·최저/최고기온 |
| 카카오모빌리티 길찾기 | 자차 이동 구간별 경로·소요시간·택시요금 |
| 카카오맵 대중교통 경로 | 대중교통 구간별 소요시간·요금·환승·경로선 |
| 행정안전부 인구감소지역 지정 데이터 | 추천 대상을 경북 15개 인구감소지역으로 한정하는 기준 |
| 지자체 공식 버스 시간표 (15개 시·군) | 대중교통 이용 시 공식 시간표 링크 제공 |

---

## 📐 기여도 산출 기준

서비스가 임의로 만든 점수가 아니라, 공개된 공공 기준을 그대로 적용합니다.

| 항목 | 기준 |
|---|---|
| **생활인구 산입일수** | 「인구감소지역 지원 특별법」의 체류인구 기준 — 하루 3시간 이상 체류한 날만 1일로 산입 |
| **1인 1일 소비 단가** | 2025 국민여행조사 국내여행 1인 1회 평균 132,000원 ÷ 숙박여행 평균 1박 2일 = **66,000원** |
| **정책 버전** | 산출 결과에는 항상 적용된 정책 버전을 함께 기록 |

---

## 🧑‍💻 팀원 소개

| **이름** | **역할** | **GitHub** |
|:--------:|:--------:|:----------:|
| 안재일 | Backend | |
| 박혜일 | Backend | |
| 김재웅 | Frontend | |
| 김온유 | Frontend | |

---

## ⚙️ 기술 스택

<table>
  <thead>
    <tr>
      <th>분류</th>
      <th>기술 스택</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>프론트엔드</td>
      <td>
        <img src="https://img.shields.io/badge/React_19-61DAFB?style=flat&logo=react&logoColor=black"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white"/>
        <img src="https://img.shields.io/badge/React_Router-CA4245?style=flat&logo=reactrouter&logoColor=white"/>
        <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white"/>
        <img src="https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>백엔드</td>
      <td>
        <img src="https://img.shields.io/badge/Java_21-007396?style=flat&logo=openjdk&logoColor=white"/>
        <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white"/>
        <img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white"/>
        <img src="https://img.shields.io/badge/Lombok-BC4521?style=flat&logo=lombok&logoColor=white"/>
        <img src="https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>데이터베이스</td>
      <td>
        <img src="https://img.shields.io/badge/MySQL_8.0-4479A1?style=flat&logo=mysql&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>인프라</td>
      <td>
        <img src="https://img.shields.io/badge/AWS_EC2-FF9900?style=flat&logo=amazon-ec2&logoColor=white"/>
        <img src="https://img.shields.io/badge/Ubuntu_24.04-E95420?style=flat&logo=ubuntu&logoColor=white"/>
        <img src="https://img.shields.io/badge/Nginx_1.24-009639?style=flat&logo=nginx&logoColor=white"/>
        <img src="https://img.shields.io/badge/Let's_Encrypt-003A70?style=flat&logo=letsencrypt&logoColor=white"/>
        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white"/>
        <img src="https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>협업 도구</td>
      <td>
        <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>
        <img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=notion&logoColor=white"/>
      </td>
    </tr>
  </tbody>
</table>

---

## 📂 저장소

| 저장소 | 내용 |
|---|---|
| **meomul-kyung** | 백엔드 — 지역 추천, 일정 생성, 외부 API 연동, 기여도 산출 |
| **meomulgyeong-frontend** | 프론트엔드 — 모바일 웹 화면 |

---

<div align="center">
<sub>
2026 관광데이터 활용 공모전(웹·앱 개발 부문) 출품작<br/>
관광 정보 출처: ⓒ한국관광공사 · 날씨 정보 출처: 기상청
</sub>
</div>
