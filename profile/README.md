![Yaneogal_main](https://user-images.githubusercontent.com/105188620/181587809-cb324016-bc39-4ae0-ba8b-5f3aa99072fc.jpeg)

## 🔎 프로젝트 소개 
<p>'야, 너도 갈래?' 는 인상 깊었던 여행코스, 
일상에서 추천하고 싶었던 장소를 공유할 수 있도록 기획한 서비스 입니다.</p>
<p>야너갈을 통해 내가 관심있는 지역이나 테마를 설정하고 진짜 정보를 경험하세요.✨</p> 
<br/>

## ✏ 서비스 기획
- “야 너도 갈래?”는 경험자들의 여행 코스와 정보를 공유하는 서비스
- **타겟층**
    - 여행 계획을 세우기에 시간적 여유가 없는 사람들
    - 여행 계획을 세우기 귀찮은 사람들
    - 다른 사람들의 여행 계획을 보고 싶은 사람들
    - 여행 계획을 어떻게 세워야할지 모르는 사람
    - 내주변 맛집이나 내가 모르는 특별한 장소 찾아보기
    
         
- 나만의 핫플레이스 저장하고 공유
<br/>

## 💻 기술 스택
FrontEnd
<div align='center'>
    <img src="https://img.shields.io/badge/html-E34F26?style=for-the-badge&logo=html5&logoColor=white">
    <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white">
    <img src="https://img.shields.io/badge/sass-CC6699?style=for-the-badge&logo=sass&logoColor=white">
    <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
    <img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">
    <img src="https://img.shields.io/badge/redux-764ABC?style=for-the-badge&logo=redux&logoColor=black">
    <br/>
    <img src="https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=black">
    <img src="https://img.shields.io/badge/aws-232F3E?style=for-the-badge&logo=aws&logoColor=black">
    <img src="https://img.shields.io/badge/github-white?style=for-the-badge&logo=github&logoColor=black">
    <img src="https://img.shields.io/badge/github%20actions-0769AD?style=for-the-badge&logo=github%20actions&logoColor=white">
</div>
    <br/>    <br/>    <br/>

BackEnd
<div align='center' >
    <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white">
    <img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
    <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=black">
    <img src="https://img.shields.io/badge/gradle-02303A?style=for-the-badge&logo=gradle&logoColor=black">
    <img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=black">
    <br/>
    <img src="https://img.shields.io/badge/amazon%20aws-f7f7f7?style=for-the-badge&logo=amazon%20aws&logoColor=f89400">
    <img src="https://img.shields.io/badge/CodeDepoly-1F497D?style=for-the-badge&logo=CodeDepoly&logoColor=white">
    <img src="https://img.shields.io/badge/EC2-782A90?style=for-the-badge&logo=EC2&logoColor=white">
    <img src="https://img.shields.io/badge/S3-FC5230?style=for-the-badge&logo=S3&logoColor=white">
    <img src="https://img.shields.io/badge/lambda-EAEAEA?style=for-the-badge&logo=lambda&logoColor=black">
    <img src="https://img.shields.io/badge/Querydsl-FF9900?style=for-the-badge&logo=Querydsl&logoColor=white">
    <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
    <img src="https://img.shields.io/badge/github%20actions-0769AD?style=for-the-badge&logo=github%20actions&logoColor=white">
</div>
<br/>

## 📖 아키텍처 
![yaneogal아키텍쳐 drawio (1)](https://user-images.githubusercontent.com/105032621/183237722-3896f2c4-e0d5-4ecd-8327-c45d1cbe4463.png)
<br/>

## 📃 ERD
![야너도갈래ERD](https://user-images.githubusercontent.com/105188620/181571360-7046077c-10ef-4d94-a744-8a2cc319a293.png)
<br/>


## 🔥 트러블 슈팅
- ## FE

    <details>
    <summary>이미지 용량에 따른 랜더링 시간 지연</summary>

    <br/>

    - browser-image-compression 라이브러리로 이미지를 압축한 후 서버로 전달
    - 669KB 이미지가 154KB로 압축되어 전달됨
    <img src="https://velog.velcdn.com/images/hongsoom/post/eb1ff74f-65e1-4510-a8a3-20436b3df7eb/image.png"/>
    </details>

    <details>
    <summary>카카오맵 : 키워드로 장소 검색을 할 때마다 기본 위치의 맵이 계속해서 렌더링되는 문제</summary>

    <br/>

    - 기본 위치 맵은 게시글 작성하기 페이지에 들어갔을 때 처음 한번만 뜨도록 useEffect 빈 의존성 배열로 넣어줌
    <img src="https://velog.velcdn.com/images/hongsoom/post/b58b59f9-3881-48c0-affb-95708eef2c34/image.png"/>
    </details>

    <details>
    <summary>무한스크롤 : 이벤트가 반복 실행(여러번 요청) 되는 문제</summary>

    <br/>

    - lodash 라이브러리를 사용해 동일 이벤트가 반복적으로 시행되는 경우 이벤트의 실제 반복 주기와 상관없이 임의로 설정한 일정 시간 간격(밀리세컨드)으로 콜백 함수의 실행을 하는 throttle 기능을 사용
    - 불필요한 서버 리퀘스트를 막을 수 있고, 동시에 필요 없는 렌더링 또한 막을 수 있어 컴포넌트의 성능 개선에 도움을 줌
    <img src="https://velog.velcdn.com/images/hongsoom/post/8ae4ef94-1557-4def-8c7a-1cfcfe767dc1/image.png"/>
    </details>

    </details>


<br/>

- ## BE

    <details>
    <summary>원본 이미지를 그대로 사용하여 성능 저하</summary>

    <br/>

    <img width="452" alt="BE_트러블슈팅1" src="https://user-images.githubusercontent.com/105188620/183325600-71ddb2ca-7ee7-49bb-b16d-e6811928027c.png">
    <img width="467" alt="트러블슈팅2" src="https://user-images.githubusercontent.com/105188620/183326058-9e066047-17dd-4f44-b2d2-e2a7af87f53e.png">
    </details>

    <details>
    <summary>CI/CD 빌드와 배포 완료 후 적용되지 않는 문제</summary>

    <br/>

    <img width="444" alt="트러블슈팅3" src="https://user-images.githubusercontent.com/105188620/183325991-2df8ce72-40d0-411d-99e3-52b5d667cd43.png">
    <img width="435" alt="트러블슈팅4" src="https://user-images.githubusercontent.com/105188620/183326109-f201c32c-ee89-45ea-b14d-eea9bf307e45.png">
    <img width="402" alt="트러블슈팅5" src="https://user-images.githubusercontent.com/105188620/183326139-5f8f2009-ae0e-4659-a36d-2f95601ab5ef.png">
    </details>

    </details>


<br/>


## 🧑‍🤝‍🧑 팀원 🧑‍🤝‍🧑
|이름|포지션|깃허브|
|------|---|---|
|🔹노흥진|BE|https://github.com/goodtonoh|
|🔹김수정|FE|https://github.com/soojeongkimkr|
|이준호|BE|https://github.com/Mohorang|
|이호진|BE|https://github.com/HoJinnn|
|홍수민|FE|https://github.com/hongsoom|
|이찬율|디자이너||

## 🎥사이트 데모

<summary>데모영상</summary>
  
|회원가입|로그인|마이페이지| 
|:---:|:---:|:---:| 
|<img src="https://velog.velcdn.com/images/hongsoom/post/cbb7a088-439f-472d-b1d1-7b4f4fccff0c/image.gif" />|<img src="https://velog.velcdn.com/images/hongsoom/post/6fb8813a-a5f8-4ddc-88d5-2d40ab79898b/image.gif"/>|<img src="https://velog.velcdn.com/images/hongsoom/post/96baf7ad-1a81-41e4-ad4f-363b8bce81b4/image.gif" />|
|메인페이지|상세페이지|
|<img src="https://velog.velcdn.com/images/hongsoom/post/4cd61f5b-b3bf-4c87-8b68-88c7aac36432/image.gif" />|<img src="https://velog.velcdn.com/images/hongsoom/post/cbbefcaf-8a21-4417-b47a-d776e97c74bd/image.gif" />|
|게시글작성|게시글 수정,삭제|댓글|
|<img src="https://velog.velcdn.com/images/hongsoom/post/152c55c0-7e27-4ce1-9e75-16ddb5cc1632/image.gif" />|<img src="https://velog.velcdn.com/images/hongsoom/post/b41390f1-fb4e-4e96-968e-6151c7fd879a/image.gif" />|<img src="https://velog.velcdn.com/images/hongsoom/post/fbce1f69-1a65-4b90-b601-9721f6ed32e2/image.gif" />|
|검색|필터|좋아요,북마크,공유|
|<img src="https://velog.velcdn.com/images/hongsoom/post/23f9c1aa-d549-4f89-b2f8-64b54d533ef4/image.gif" />|<img src="https://velog.velcdn.com/images/hongsoom/post/3a73dcaa-260a-480e-b851-f5f5b4779573/image.gif" />|<img src="https://velog.velcdn.com/images/hongsoom/post/d7343e7e-837e-4490-9b46-a3a812acf8f2/image.gif" />|

<br />
