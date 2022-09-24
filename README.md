# resume

[![Anurag's github stats](https://github-readme-stats.vercel.app/api?username=kimth007kim)](https://github.com/anuraghazra/github-readme-stats)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=kimth007kim&layout=compact&hide=css,html,pug,Assembly,Scilab)](https://github.com/anuraghazra/github-readme-stats)

## 소개

<img width="217" alt="증명사진" src="https://user-images.githubusercontent.com/48907339/101289048-48c59180-383d-11eb-8dbb-4e93dd4e09f8.png">

- 김경동
- E-mail : kimth007kim
- GitHub : https://github.com/kimth007kim

- 안양대학교 정보통신공학과 졸업
- 미국 유학경험(2010~2012)

항상 더 나은 개발자가 되기위해 1일 1커밋운동을 하고있고, 새로운 기술들을 스폰지 같이 흡수하는 개발자가 되고싶습니다.


## 사용언어 및 기술들

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![Spring Security](https://img.shields.io/badge/spring--security-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-green?style=for-the-badge&logo=)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white)

## 프로젝트

### Team-Project

### `CrewCrew (취미 및 스터디 매칭) ` 202201~202207

![sacsca](https://user-images.githubusercontent.com/48907339/190577512-9d7a278e-62e2-41fa-8950-08726d41b9bc.jpg)

백엔드 개발자 3명 , 프론트 엔드 개발자 1명, 웹퍼블리셔 1명, 웹 디자이너 1명으로 구성된 프로젝트로,
제가 사이드 프로젝트를 하고싶을때 각각 다른역할의 팀원을 구하기 힘들어서 팀원을 찾기 쉬운 서비스를 만들면 어떨까 해서 개발해보게 되었습니다.

[프로젝트 깃허브](https://github.com/kimth007kim/crewcrew)

#### 개발

- 이메일 회원 가입
    - 이메일 인증 코드 발송
    - 이메일 인증 코드 유효성 검사
    - 닉네임 중복 여부 확인
    - 회원 가입 시 default 이미지 선택
    - 회원 가입 시 유저가 선택한 이미지 선택 후 S3 저장소에 저장 후 DB에 저장
- 이메일 로그인
    - 이메일 로그인
    - 로그인 시 토큰 유지 시간 설정 기능( 3시간, or 3일)
    - access,refresh 토큰 재발급
- 마이 페이지
    1. 비밀 번호 변경
        - 이메일  인증 코드 발송 기능(비밀번호 변경 시)
        - 이메일 인증 코드 유효성 검사(비밀번호 변경 시)
    2. 프로필 이미지 변경
        - default 이미지 선택
        - 유저가 선택한 이미지 선택 후 S3 저장소에 저장 후 DB에 저장
        - 유저가 선택한 이미지 선택 후 S3 저장소에 저장 후 DB에 저장
    3. 닉네임 변경

- 소셜 통합 회원 가입 ,로그인
    - Kakao,Naver 에서 유저가 입력한 email ,password 로  해당 유저 refreshToken, AccessToken 정보 redirect
    1. 해당 유저가 DB에 존재 하지 않은 경우(회원 가입)
        - Kakao,Naver 에서 redirect한 token에서 프로필 이미지 URL을 추출한 후 S3에 업로드 후 DB에 저장
        - Kakao,Naver 에서 redirect한 token에서 닉네임을 추출한 후 중복을 피하기 위해 랜덤한 숫자를 #뒤에 붙여서 새로운 닉네임 생성
        - 소셜 회원 가입시 DB에 랜덤한 환영 메세지 생성 후 DB에 저장
    2. 해당 유저가 DB에 존재할 경우(로그인)
        - 비밀 번호 없이 Kakao, Naver 에서 발급한 accessToken 을 통해서 로그인

- 채팅 기능
    - Stomp+ SockJS로 채팅 프론트와 통신
    - DB에 보낸 메세지들 저장
    - user의 id 값으로 참여중인 채팅방 조회
    - room id 값으로 채팅을 페이지네이션 후 조회



### Mini-Project

### `에브리타임 클론코딩`

![에타메인](https://user-images.githubusercontent.com/48907339/101289117-d43f2280-383d-11eb-8857-89062e08ce32.PNG)

Node.js 프로그래밍 3판 -윤인성 저자님의 책을 학습하고 에브리타임 홈페이지를 1인 미니프로젝트를 진행하기로 했습니다.

[프로젝트 깃허브](https://github.com/kimth007kim/everyTime_clone_nodejs)

#### 개발

- express template engine인 pug를 이용해서 프론트엔드 작업

- node.js와 express를 이용해서 백엔드 작업

- DB는 Mysql을 사용
