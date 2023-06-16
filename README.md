# PORTFOLIO
# :clipboard: 목차

- :books: <a href="#outline">개요</a>
- :wrench: <a href="#tech">기술스택</a>
- :family: <a href="#team">팀원소개</a>
- :bookmark_tabs: <a href="#function">기능구현</a>
  - 이메일 인증
  - 사업자등록번호 확인
  - 주문목록확인
  - 결제
  - 배송추적
- :bulb: <a href="#result">결론</a>
- :mag_right: <a href="#">보완할점</a>

# :books: <a name="outline">개요</a>
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/Mainpage.png">

>**프로젝트**: 항만물류사이트 제작
>
>**기획 및 제작** : Team Orca
>
>**분류**: 개인포트폴리오
>
>**제작 기간**: 2023.05.15 ~ 2023.06.09
>
>**담당 기능**: 이메일인증, 사업자등록번호 확인, 선박 시뮬레이션, 배송추적, 결제, 목록확인

# :wrench: <a name="tech">기술스택</a>
<h4>데이터베이스</h4>
<div align="left">
 	<img src="https://img.shields.io/badge/ORACLE-F80000?style=flat&logo=oracle&logoColor=white" />
  <img src="https://img.shields.io/badge/H2-232F3E?style=flat&logo=h2&logoColor=white" />
</div> 
<h4>백엔드</h4>
<div align="left">
 	<img src="https://img.shields.io/badge/JAVA-007396?style=flat&logo=Java&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=flat&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring Security-6DB33F?style=flat&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/JPA-59666C?style=flat&logo=hibernate&logoColor=white" />
  <img src="https://img.shields.io/badge/MyBatis-232F3E?style=flat&logo=mybatis&logoColor=white" />
</div> 
<h4>프론트엔드</h4>
<div align="left">
	<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />
	<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />
  <img src="https://img.shields.io/badge/JAVASCRIPT-F7DF1E?style=flat&logo=javascript&logoColor=white" />
</div>
<h4>UI프로토타입</h4>
<div align="left">
	<img src="https://img.shields.io/badge/FIGMA-F24E1E?style=flat&logo=figma&logoColor=white" />
</div>
<h4>배포</h4>
<div align="left">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=white" />
	<img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white" />
</div>
<h4>협업도구</h4>
<div align="left">
	<img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=Notion&logoColor=white" />
	<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white" />
</div>

# :family: <a name="team">팀원소개</a>
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/팀원소개.png"> <br/><br/>
# :bookmark_tabs: <a name="function">기능구현</a>
**1. 이메일 인증**
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/이메일인증.gif"> <br/><br/>
- SimpleMailMessage 클래스를 이용하여 메일 내용 설정
- JavaMailSender를 이용하여 Gmail로 고객에게 인증번호 전송
- 전송된 인증번호를 입력하여 인증확인
<br/>

**2. 사업자등록번호 확인**
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/사업자등록번호.gif"> <br/><br/>
- 공공데이터포럼에서 사업자등록번호 API를 통해 데이터를 받는다.
- 받은 값(b_stt_cd)을 이용하여 유효성 검사 실시(01:유효한 사업자등록번호)
<br/>

**3. 주문목록확인**
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/주문상세목록.png"> <br/><br/>
- RESTful 웹 서비스를 구축하여 RestController로 주문상세목록 객체를 JSON으로 데이터 전송
- 버튼 클릭시 Modal에서 주문 상세 목록 출력
<br/>

**4. 결제**
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/결제.gif"> <br/><br/>
- 아임 포트(Iamport)를 이용한 무료로 서비스되는 결제 연동API 사용
- 각 종 PG를 이용하여 결제 후 완료시 상품 State 결제완료로 변경 후 
<br/>

**5. 배송추적**
<img src="https://raw.githubusercontent.com/ldj8196/Portfolio/main/src/main/resources/static/DJ/portfolioimage/배송조회.gif"> <br/><br/>
- Scheduler의 크론식을 이용하여 배의 위치를 5초마다 확인
- Server-Sent-Events이용 선박의 위도와 경도를 Server로 부터 수신받아서 지도에 표시
- 처음 요청은 버튼을 눌러서 Push 방식, JS setTimeOut으로 3초마다 Pull방식으로 위치 요청
<br/>

# :bulb: <a name="result">결론</a>

# :mag_right: <a name="fullfill"></a>
