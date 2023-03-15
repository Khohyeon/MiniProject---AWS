<!-- # Springboot-MyBatis-Recruitment-Project -->
<h1> 👩‍👩‍👦‍👦HIGHRE란?👩‍👩‍👦‍👦 <br></h1>

![image](https://user-images.githubusercontent.com/122351733/223630188-a70350c4-3496-4705-bfe3-c031f68d27f3.png)


>'고용하다'라는 의미의 Hire와 '더 높은'이라는 의미의 Higher를
><br>합쳐 고객들에게 더 좋은 일자리를 제공한다는 의미를 담았습니다

<br> 

# 기술스택💡
- JDK 11
- Springboot 2.7.8
- Bootstrap
- MyBatis
- 테스트 H2 DB
- 프로덕션 MySQL DB
- JSP
- redis

<br>

# 아키텍쳐(MVC) 💫

![image](https://user-images.githubusercontent.com/122351733/223648466-ee6ce325-64b3-4f82-888b-5d627e5e55fe.png)

## 패키지 구조
> Controller👩‍💻 Model📚 Service✨ View🎨

- Client의 책임 : View로 부터 응답을 받음 , Model을 거쳐 데이터를 받아 View로 부터 응답

- Service의 책임 : Controller의 책임을 Transaction 을 사용하여 분리 하는 역할 

- Model의 책임 :  DataBase나 File이나 다른 서버로 부터의 통신

- View의 책임 : Client에 그림을 그려줌


<br>

# 기능정리📝
<br>

## <strong>Frontend💕
- Header, Footer 레이아웃
- 메인, 로그인, 회원가입 페이지
- 이력서 메인, 등록, 목록 보기, 상세 보기 페이지
- 채용공고 리스트, 등록, 상세보기 페이지
- 개인-기업) 정보 수정
- 개인) 마이페이지 - 지원 현황, 매칭 서비스, 북마크 스크랩
- 기업) 마이페이지 - 지원자 현황, 매칭 서비스, 북마크 스크랩

## <strong>Backend💕
<br>

### 1단계💛

- DB 설계
- 로그인 기능 구현
- 회원가입 기능 구현
- 이력서 등록 기능 구현
- 이력서 수정 기능 구현
- 이력서 삭제 기능 구현
- 채용공고 등록 기능 구현
- 채용공고 수정 기능 구현
- 채용공고 삭제 기능 구현

<br>

### 2단계💚 
<br>

🙋‍♂️ 개인  
- 비밀번호 HASH,salt 암호화 
- 아이디 중복 체크 및 Password 중복 검사
- 회원가입 시 기술스택 선택 기능
- 로그인 시 아이디 기억 (Cookie)
- 로그인 시 최초 접속 페이지 유지 하기
- 회원정보 수정
- 이력서 지원 하기, 취소하기
- 북마크 기능 구현

🏢기업
- 비밀번호 HASH,salt 암호화 
- 아이디 중복 체크 및 Password 중복 검사
- 회원가입 시 기술스택 선택 기능
- 로그인 시 아이디 기억 (Cookie)
- 로그인 시 최초 접속 페이지 유지 하기
- 회원정보 수정

📜공고
- 공고 제목, 내용으로 검색 하기
- 카테고리 별 검색 하기
- 마감일자 기능
-공고 등록시 기술스택 선택 기능

<br>

### 3단계💙

<br>

🙋‍♂️ 개인 
- 마이페이지-지원 현황 보기(합격/불합격/대기중 버튼)
- 마이페이지-지원 취소(마감일자 전에만 가능)
- 공고 상세보기 페이지에서 이력서 선택하여 제출 기능
- 기술스택이 동일한 기업과의 매칭 서비스
- 합격/불합격 처리 시 마이페이지 동기화 기능
- 합격/불합격 처리 시 SSE 알림 기능
- 회사 별점 달기
- 회원가입 시 이메일 인증 받기
- 회원가입 시 전화번호 인증 받기

🏢기업
- 지원자 개인정보와 이력서 열람 기능
- 이력서 열람 및 합격/불합격 처리
- 합격/불합격 처리 시 마이페이지 동기화 기능
- 기술스택이 동일한 개인회원과의 매칭 서비스

🎻기타 기능
- Redis 세션

<br>

### 4단계💜

<br>

- 지도 API
- 주소 입력 API
- OAUTH 로그인
- 공고 목록 캘린더에 담기

<br>

### 5단계💔

-