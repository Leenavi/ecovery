# 🌍 ECOVERY – AI 사물인식 기반 대형폐기물 분리배출 & 재활용 플랫폼
---

(25.07.07 ~ 25.08.08 - 약 5주)  
1주차 : 사전 조사, 프로젝트 기획 및 요구사항 정의, 화면 설계, DB 설계
2주차 : 데이터 수집 및 전처리, 로그인 및 등록, 조회 기능 구현
3주차 : YOLOv8 모델 학습 및 스프링 연동, 페이징 기능 구현, 팀 중간 점검
4주차 : 관리자 페이지 및 세부 기능 구현
5주차 : 프론트엔드 연동, 통합 테스트 및 최종 발표   

---
# 📚 목차 📚
1. [🌱 프로젝트 소개](#1-프로젝트-소개)
2. [👥 참여자](#2-참여자)
3. [💻 개발환경](#3-개발환경)
4. [📋 요구사항 정의](#4-요구사항-정의)
5. [⚙️ 기술소개](#5-기술소개)
6. [🗂️ 클래스 구조](#6-클래스-구조)
7. [🖼️ 화면 예시](#7-화면-예시)
8. [🐞 Troubleshooting](#8-troubleshooting)
9. [✨ 개선사항 및 프로젝트 소감](#9-개선사항-및-프로젝트-소감)

---
# 1. 프로젝트 소개
### 🌳 ECOVERY란 ? <br>
&nbsp;&nbsp;&nbsp;&nbsp;Ecovery는 **Eco**(환경)와 **Recovery**(회복)의 합성어로,  
AI 기반 대형폐기물 분류를 비롯해 분리배출 신고, 무료나눔, 재활용 상품 판매, 환경 뉴스 제공까지 한 번에 제공하는 통합 친환경 플랫폼입니다.  
&nbsp;&nbsp;&nbsp;&nbsp;대형폐물 인식 AI와 무료나눔 서비스를 통해 자원 재활용을 촉진하고, 헷갈리는 품목도 간편하게 신고하며, 필요한 물건을 나누고 합리적인 가격으로 재활용 제품을 구매할 수 있습니다. 
또한 신뢰할 수 있는 환경 정보를 한 곳에서 확인하며 환경 보호를 실천할 수 있습니다.

---

### 💡 ECOVERY 개발 의도 <br>
&nbsp;&nbsp;&nbsp;&nbsp;현대 사회에서 생활폐기물은 지속적으로 증가하고 있으며, 특히 대형폐기물은 배출 과정이 복잡하고 불편해 시민들이 혼란을 겪는 경우가 많습니다. 
최근 1인 가구 비율이 전체 가구의 약 35%를 넘어서면서 폐기물 관리 부담은 더욱 커지고 있습니다. 
정책은 꾸준히 개선되고 있지만, 대형폐기물은 지역마다 배출 규정이 달라 시민들의 혼란이 계속 되고 있습니다.   

&nbsp;&nbsp;&nbsp;&nbsp;또한, 여전히 멀쩡한 물건들이 재활용이나 나눔 없이 그대로 폐기되고 있어 매년 약 3조 원의 재활용 가능 자원이 그냥 버려지고 있으며, 이는 자원 낭비와 환경보호에 대한 관심 부족을 심화시키고 있습니다. 
더불어 환경 관련 정보는 파편적으로 흩어져 있어, 시민들이 필요한 정보를 쉽고 빠르게 얻기 어렵습니다. 이로 인해 환경과의 연결은 점점 멀어지고, 실질적인 행동으로 이어지기 어려운 상황입니다.   

#### ECOVERY는 이러한 문제를 해결하기 위해 다음과 같은 목표로 개발되었습니다.   
1. **AI 기반 대형폐기물 인식**을 통해 간편하고 정확한 배출 절차 안내  
2. **무료나눔 플랫폼** 제공으로 사용 가능한 물품의 재사용 촉진    
3. **에코마켓**을 통한 친환경·재활용 상품 판매 및 환경 뉴스 제공  
4. 사용자 친화적인 UI/UX로 누구나 쉽게 환경 보호 활동에 참여 가능하게 설계  

#### 기대효과 
1. AI 이미지 인식을 통해 누구나 쉽게 폐기물 품목을 식별할 수 있습니다.
2. 사용자 데이터를 기반으로 정책 및 시스템 개선이 가능해집니다.
3. 재활용을 장려하여 환경을 생각하는 소비 문화를 조성합니다.
4. 환경 소식을 통해 지속적인 관심과 참여를 확대하고 건강한 환경 문화를 만들어갑니다. 

이를 통해, ECOVERY는 환경 보호를 어렵고 멀게 느끼는 사람들에게 **쉽고 친근한 참여 방법**을 제공하고,    
대형폐기물 배출과 자원 재활용을 보다 효율적이고 편리하게 만들어 지속 가능한 생활 문화를 확산시키는 것을 목표로 합니다.   

---
# 2. 참여자 

<h3>✨ 이지혜 (본인)</h3>
<strong>본 프로젝트에서 저는 분리배출 게시판 및 관리자페이지의 기획·개발을 담당했습니다.</strong><br>
역할: 팀장 / 프로젝트 전반 관리 / 백엔드 개발     
담당 기능: AI 데이터 라벨링, AI 모델링, FastAPI - Spring 연동, 분리배출 게시판, 관리자 페이지 기능 구현 
<br>
<br>
🛠️ 이연수
역할: 팀원 / 백엔드 개발 <br>        
담당 기능: AI 데이터 라벨링, 무료나눔, 문서 관리

<br>  
<br>

🗂️ 방희경      
역할: 팀원 / 백엔드 개발      
담당 기능: 회원 관리 기능, 에코마켓  

🔐 노유경  
역할: 팀원 / 백엔드 개발    
담당 기능: 소셜 로그인, 환경톡톡, 공지사항 게시판, Git 버전 관리  

🎨 최은지  
역할: 팀원 / 프론트엔드 개발  
담당 기능: 프론트 구조 설계 및 구현   

---
# 3. 개발환경

### Backend
- Spring Boot 3.4.7  
- Java 17  
- MySQL 8.0  
- MyBatis  
- Gradle  
- IntelliJ IDEA  
- Tomcat 9  
- File Save: Local

### AI Server
- FastAPI (Python)
- YOLOv8

### Frontend
- HTML, CSS, JavaScript, Thymeleaf  
- VS Code
---
# 4. 요구사항 정의 

<img width="1400" height="500" alt="{91485312-7DB7-4E4C-9A1A-BE761E7736A9}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7B423950BF-E6D3-4B52-AFA7-81B11A490E38%7D.png?raw=true" />

* 이 문서는 분리배출 게시판, 관리자페이지에 대한 **요구사항 정의서**로, 시스템이 제공해야 하는 주요 기능과 조건을 정리한 표입니다.
* 이미지 등록, AI 예측 결과와 지역 정보 기반 결과 도출, 효율적 관리 서비스 등 핵심 기능들을 요구 ID, 기능 ID, 설명 형태로 명확히 정의하여 개발 범위와 목표를 한눈에 확인할 수 있습니다.
* 프로젝트 구현 시 반드시 충족해야 할 사용자 요구와 기능 요구를 구체적으로 문서화한 것입니다.

---

# 5. 기술소개 

### 🌱 Spring Boot  
- 백엔드 전반을 구성하는 핵심 프레임워크로, MVC 기반 서비스 구현  
- MyBatis와 연동하여 게시글, 이미지, 댓글 등 CRUD 로직 처리
- FastAPI 기반 AI 서버와 연동해 이미지 인식 기능 제공 
- **분리배출 게시판, 관리자페이지의 등록·조회 API와 이미지 업로드 API를 구현하는 기반이 됨**

### 🔐 Spring Security  
- 회원 / 관리자 역할에 따른 접근 권한 제어  
- 인증·인가 로직을 커스터마이징하여 Role 기반 보안 구성  
- **분리배출 게시판은 누구나 이용 가능하지만 관리자 페이지는 관리자로 로그인한 사용자만 이용할 수 있으며, 관리자페이지를 통해 회원 권한 수정 가능 권한 설정**

### 🧩 MyBatis  
- SQL 매퍼(XML) 기반의 데이터 접근 계층 구현  
- 동적 SQL을 활용해 검색, 페이징, 조건 분기 로직 처리  
- **분리배출 페이지의 결과, 관리자페이지의 조회, 검색, 필터링, 수정 로직 구현에 사용**

### 🖼 Thymeleaf & JavaScript  
- 게시판, 상세 페이지 등 주요 뷰를 Thymeleaf로 구성하고 동적 UI를 JavaScript로 구현  
- Fetch API 기반 비동기 처리로 사용자 2차 분류 선택장, 이미지 업로드, 상태 변경 등 실시간 반영  
- **분리배출 게시판 및 관리자페이지 CRUD 기능을 비동기 방식으로 처리**

### 🤖 FastAPI & YOLOv8  
- Python 기반 FastAPI 서버를 통해 Spring과 연동
- YOLOv8 모델로 객체 탐지 및 클래스 예측 결과 반환  
- **AI 예측 결과와 지역 정보에 따라 사용자 맞춤 카테고라이징 지원**

### ⚙ 환경 구성 
- **Gradle**을 통한 빌드 및 의존성 관리
- **Tomcat 9**를 사용해 로컬 및 서버 환경에서 애플리케이션 실행
- 이미지 및 첨부파일은 **Local Storage**방식으로 저장 후 경로 DB 연동
- **MYSQL 8.0** 데이터베이스를 기반으로 모든 게시판 및 사용자 데이터 관리 

<img width="1893" height="1027" alt="image" src="https://github.com/user-attachments/assets/f2609713-accd-40bc-9adc-eae44d6a824e" />

---
# 6. 클래스 구조 

<img width="1917" height="797" alt="image" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/MemberVO.png?raw=true" />

* 이 다이어그램은 **분리배출 게시판 및 관리자페이지의 클래스 다이어그램**으로, 도메인 객체(VO/DTO), 서비스, 컨트롤러, 매퍼 간의 관계를 나타냅니다.
* 사용자, 이미지, 안내 정보, 배출 내역과 관련된 클래스들이 상호 연계되어 CRUD 기능과 비즈니스 로직을 수행하는 구조를 시각화했습니다.
* 전체 시스템의 계층 구조와 객체 간 의존 관계를 한눈에 보여줍니다.

<img width="500" height="500" alt="{9F28DA0A-40B0-4F99-AFA2-BD9EA08C7A90}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%EA%B7%B8%EB%A6%BC1.png?raw=true" /> <span></span>
<img width="500" height="500" alt="{9F28DA0A-40B0-4F99-AFA2-BD9EA08C7A90}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%EA%B7%B8%EB%A6%BC2.png?raw=true" />

* 이 **유스케이스 다이어그램**은 분리배출 게시판 및 관리자페이지에서 일반 사용자, 관리자별 권한을 나타냅니다.
* 누구나 분리배출 서비스 이용이 가능하고, 관리자는 관리자페이지 진입, 내역 확인, 회원 권한 수정 기능까지 수행할 수 있습니다.
* 사용자 유형에 따라 접근 가능한 기능 범위를 한눈에 확인할 수 있습니다.



---

# 7. 화면 예시 
<details>
<summary><h3>분리배출 및 관리자페이지 화면구성 보기</h3></summary>

--- 
<h3><분리배출 메인페이지></h3>
<img width="1000" height="893" alt="{6C3E4669-FB6F-40FB-9B22-4054EBD33E91}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%EA%B7%B8%EB%A6%BC3.png?raw=true" />

🔎 분리배출 게시판의 메인 화면입니다.
* 누구나 대형폐기물 이미지와 폐기할 지역에 대한 정보를 입력할 수 있습니다.

---
<h3><분리배출 AI 예측 결과 및 사용자 2차 선택창></h3>
<img width="500" height="500" alt="{B0B46550-D64E-49E3-873F-63E061705051}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%EA%B7%B8%EB%A6%BC4.png?raw=true" />

🔎 AI 예측 결과에 따른 2차 분류 선택창입니다.
* **검색 기준(제목/내용/지역/전체)** 을 선택해 원하는 방식으로 조회할 수 있습니다.
* 사용자가 입력한 지역 정보와 AI 예측에 맞춰 카테고라이징된 옵션을 보여줍니다.

---
<h3><최종 선택 기반 결과 안내 페이지></h3>
<img width="500" height="500" alt="{38E29525-8320-4E08-8267-2CEBD64FB62E}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%EA%B7%B8%EB%A6%BC5.png?raw=true" /> <span></span>
<img width="500" height="300" alt="{38E29525-8320-4E08-8267-2CEBD64FB62E}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%EA%B7%B8%EB%A6%BC6.png?raw=true" />

🔎 이미지 분석 결과 및 폐기 수수료 안내페이지입니다.
* 최종 선택된 분류 품목에 따라 예상 폐기 수수료를 확인할 수 있습니다.
* 결과 확인 후 에코버리 사이트의 무료 나눔 게시판에 글을 등록하거나 폐기물 배출을 신고할 수 있는 서비스를 제공합니다.
* AI의 예측이 잘못됐을 경우 사물 인식 오류 신고 버튼을 통해 관리자에게 AI 예측의 오류를 알릴 수 있습니다.

---
<h3><관리자페이지 메인 대시보드></h3>
<img width="1000" height="893" alt="{19213E0E-960C-4AA5-858D-1A16B7DAFC31}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7B04A79198-5318-4455-BFDB-14B58EE8B411%7D.png?raw=true" />
  
🔎 관리자페이지의 메인화면입니다.
* 관리자로 로그인시 진입할 수 있는 페이지입니다.
* 관리자는 한눈에 회원, 분리배출 사용량 등을 확인할 수 있습니다.
* 각 카드별 바로가기 버튼을 통해 각 기능별 관리 페이지로 이동할 수 있습니다.

---
<h3><관리자페이지 내 분리배출 내역 페이지></h3>
<img width="600" height="400" alt="{54998963-EE68-4A66-B7EE-77B730FBCC76}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7B3D0DC0AD-297E-4DD8-8357-37A327E496A0%7D.png?raw=true" /> <span></span>
<img width="400" height="500" alt="{54998963-EE68-4A66-B7EE-77B730FBCC76}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7BB2A8710C-0519-4914-B403-F4022FBEF735%7D.png?raw=true" />

🔎 분리배출 및 오류 내역 페이지입니다. 
* 관리자는 총 건수, 평균 ai 정확도 등을 한 눈에 확인할 수 있습니다.
* 검색 및 필터링을 통해 필요한 데이터만 확인할 수 있습니다.
* 각 내역별 상세보기 버튼을 누르면 해당 내역의 상세 정보를 확인할 수 있습니다.

--- 
<h3><관리자페이지 내 회원관리 페이지></h3>

<img width="1154" height="843" alt="{5A4EA635-4D2A-4E20-BA19-8A8DD82C4CEA}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7B1F93C17D-9449-4CBA-906B-78F06100F169%7D.png?raw=true" />

🔎 회원관리 페이지입니다.
* 관리자는 총 회원 수, 회원별 로그인 방식 등을 확인할 수 있습니다.
* 검색 및 필터링을 통해 필요한 데이터만 확인할 수 있습니다.
* 각 회원별 상세보기 버튼을 통해 회원별 권한 수정이 가능합니다.

---
<h3><관리자페이지 내 회원 권한 수정 페이지></h3>
<img width="700" height="600" alt="{A04AE862-8E9A-42EF-8E37-82D4DFF0C8B8}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7BB47E9945-68AF-4948-BFC4-031E5A8B8671%7D.png?raw=true" /> <span></span>
<img width="400" height="400" alt="{A04AE862-8E9A-42EF-8E37-82D4DFF0C8B8}" src="https://github.com/leeJiHye95/ecovery/blob/main/src/main/resources/static/gitImages/%7B1C32A187-31E2-4036-A544-43C632B9E42E%7D.png?raw=true" />

🔎 회원 권한 수정 페이지입니다.
* 관리자는 각 회원별 상세보기 버튼을 통해 회원별 권한 수정이 가능합니다.
* 권한 변경시 기존 권한, 새 권한 정보를 모달창으로 보여주어 한 번 더 확인할 수 있도록 합니다.

</details>

---

# 8. Trouble Shooting – 관리자페이지 데이터 페이징 및 필터링 처리 오류

📌 문제 상황
복합 조건(기간+지역+품목) 조회 시 출력·페이징 동작 불안정, 필터 갱신 시 목록이 아예 출력되지 않는 문제가 발생했습니다.

💥 원인 분석
- 서버의 페이징처리(LIMIT / OFFSET)와 클라이언트의 파라미터 조합이 분리되어 상태 불일치가 있었습니다.
- backtick과 따옴표의 혼용으로 page=${page}가 값이 아닌 문자열 그대로 전달이 되었습니다.

🔍 해결 방법
1. MyBatis에서 동적 SQL을 써서, **검색조건 + 페이징 처리(total count, row list)**를 한 번에 처리
2. 모든 검색/필터 상태를 URL 쿼리스트링으로 통일
3. 버튼, 페이지 링크, Ajax 요청 전부 이 표준화된 함수로 query string을 만들어 사용

✅ 결과
- 관리자 페이지에서 검색 + 필터 + 페이징이 일관되게 동작.
- 조건을 여러 개 걸어도 정확히 결과가 나오고, 페이지 넘겨도 조건 유지됨.
- 재입력 최소화 및 동일 문제 재발 방지  

이러한 로직 개선을 통해 사용자 경험을 크게 개선했고, 개발 단계에서도 데이터 처리 흐름을 명확히 구분할 수 있었습니다.
앞으로도 비슷한 문제를 예방하기 위해, 데이터 초기화 시점과 상태 관리 로직을 더 체계적으로 설계하는 습관을 들이게 되었습니다.

---

# 9. 개선사항 및 프로젝트 소감 

이번 프로젝트에서는 AI 라벨링과 모델링, 분리배출 게시판, 관리자 페이지까지 전 과정을 직접 개발했습니다.
분리배출 게시판에서는 사용자가 이미지를 업로드하면, AI 모델이 예측을 하고 사용자가 최종 품목을 선택해 DB에 저장할 수 있는 구조를 구현했습니다. 또한 오인식 신고 기능을 통해 사용자가 잘못 분류된 경우 이를 신고하면, 관리자 페이지에서 확인할 수 있도록 설계했습니다.

관리자 페이지에서는 검색·필터·페이징 기능과 함께 AI 예측 신뢰도, 신고 내역을 확인할 수 있는 기능을 구현했습니다. 이 과정에서 단순한 기능 구현을 넘어, 데이터 흐름과 기능 간 의존성, 운영 환경에서 발생할 문제까지 고려하는 경험을 쌓을 수 있었습니다.

향후에는 보다 나은 서비스 운영을 위해, 사용자의 신고 데이터를 활용한 AI 자동 학습, 배출 신고 자동화, 통계 그래프 시각화 기능 등을 구현해보고 싶습니다.
