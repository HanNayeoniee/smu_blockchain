# 블록체인 기반 이력관리 시스템

### 2019 이브와 ict 멘토링(2019.04~2019.11)

----------

__주제__: 블록체인 기반 이력관리 시스템

__기획 배경__ : 위조, 도용, 개인정보 유출의 위험이 있는 **기존 이력서 시스템의 문제점을 보완**하기 위해 블록체인을 도입함.

__팀원__: [김나혜(nahye03)](https://github.com/nahye03), [김소현(sohyeon98720)](https://github.com/sohyeon98720),[이지민(Jimin980921)](https://github.com/Jimin980921), [한나연(HanNayeoniee)](https://github.com/HanNayeoniee)

----------
           
__프로젝트 내용__ :                   

__1. 사용자 구분__:                    
  <img src="https://user-images.githubusercontent.com/47767202/79406667-a79a7a00-7fd2-11ea-9dcf-1f51ffca4310.JPG">             
  - __지원자__: 기업에 지원. 지원하기 위한 이력서의 세부 항목을 각 관련기관에게 인증받아야함.
  - __회사__: 지원자로부터 이력서를 받음. 혹은 경력인증 요청 시 경력 인증.
  - __학교__: 지원자로부터 학력인증 요청 시 학력 인증.
  
-------

__2. 기능__:                        
  - __입력기능__ : 이력서 정보 입력(인적사항, 경력, 학력)
  - __전송기능__ : 지원자와 학교, 지원자와 기업 사이에 학력, 경력 전송
  - __인증기능__ : 학교/기업이 지원자가 작성한 학력/경력 위조 여부 인증
  - __관리기능__ : 권한이 있는 사람만 이력서 작성(지원자), 열람(인증하기위함 or 이력서열람) 가능
  
  -> 이력/경력 인증을 요청하고 기다리는 동안 새로운 이력/경력을 작성할 수 없음(웹 기능)                      
  -> 인증을 받은 최소 하나 이상의 학력/경력이 존재해야 지원하고자하는 기업에 이력서를 제출할 수 있음(웹 기능)                                       
   <img src="https://user-images.githubusercontent.com/47767202/77847863-22098280-71fb-11ea-96ec-5609d349ff04.png" width="50%">    

  _=> 기존 이력서 시스템의 문제점 개선_

----------

__3. 사용프로그램__: 
  - __remix__: 블록체인 코드 구현
  - __webstorm__: 블록체인과 웹 연동 및 웹 ui, 데이터베이스 연결, 깃 연동 등 전체적인 부분 담당
  - __Robomongo__: 데이터베이스
  
---------

__4. 결과__:
  - __메인화면__: 로그인시 사용자에 따라 권한이 다르게 주어져 허락받은 페이지(지원자, 기업, 학교 중 하나)만 접속가능    
  <img src="https://user-images.githubusercontent.com/47767202/79295452-a9e9cf00-7f13-11ea-92ba-781dd9feea24.PNG" width="50%">
  <br>
  
  - __지원자로 로그인했을 때__: 학력 및 경력 작성 후 내 원서함(세번째 사진)페이지에서 전송할 수 있음 + 학력과 경력 모두 승인받은 이력서만 기업에 전송할 수 있음
   <img src="https://user-images.githubusercontent.com/47767202/79295603-06e58500-7f14-11ea-853f-2825c6cc627c.PNG" width="50%">      
   
   <img src="https://user-images.githubusercontent.com/47767202/79295730-6774c200-7f14-11ea-939a-ba83de2b7cf0.PNG" width="50%">    
   
   <img src="https://user-images.githubusercontent.com/47767202/77847898-62690080-71fb-11ea-802a-b56ab4934d07.png" width="50%">   
   <br>
   
  -  __인증)학교/기업으로 로그인했을 때__: 학력/경력 인증하기 페이지에서 지원자의 학력/경력 사실여부 검토 후 인증여부 반환               
   <img src="https://user-images.githubusercontent.com/47767202/80339015-bae1fb00-8898-11ea-83ca-dea72d075b05.png" width="50%">
   <br>
  
  - __지원자보기)기업으로 로그인했을 때__: 지원자의 이력을 각 해당기관이 모두 인증하였기때문에 위조의 우려없이 이력서 검토가능             
    <img src="https://user-images.githubusercontent.com/47767202/80339482-b23df480-8899-11ea-8a0a-091fd9a9292c.png" width="50%">
