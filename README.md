# Codebang
## 커뮤니티 프로젝트
- spring으로 만들어 본 개발자 커뮤니티 웹사이트 프로젝트.
- 배포 : [Codebang 웹사이트](https://codebang.store)

## 설계

### 유스케이스 다이어그램

![유스케이스 다이어그램](./img/유스케이스%20다이어그램.png)

### 시스템 구성 다이어그램

![시스템 구성 다이어그램](./img/시스템%20구성%20다이어그램.png)

### ERD

![ERD](./img/ERD.png)

## 주요 기능 

### 회원 관리

- 회원 가입
- 로그인
- 회원 정보 조회
- 정보 수정(이름, 비밀번호, 이메일) 수정
- 회원 탈퇴

### 게시글 기능

- 게시글 작성
  - 제목, 내용 작성
  - 이미지 업로드
  - 로그인 한 유저만 작성 가능
- 게시글 조회
  - 전체 조회
    - 전체 글의 제목, 작성자, 작성일, 조회수 조회
  - 상세 조회
    - 해당 글의 제목, 작성자, 내용, 이미지, 작성일, 조회수, 댓글 조회
    - 로그인 사용자라면 댓글 작성 가능
  - 페이징 처리
- 게시글 수정
  - 제목, 내용, 이미지 수정 가능
  - 글의 작성자만 수정 가능
- 게시글 삭제
  - 해당 글과 글에 달린 댓글, 이미지를 모두 삭제
  - 글의 작성자만 삭제 가능
- 댓글 기능
  - 댓글은 로그인 한 유저만 작성 가능하고, 본인의 댓글을 수정 삭제 가능
  - AJAX로 비동기적인 댓글 기능 구현

## 사용된 기술
- Java 17
- SpringBoot 3.0.2
- Spring MVC
- Spring DataJPA
- Thymeleaf
- Gradle
- Amazon EC2
- MariaDB
- Nginx


