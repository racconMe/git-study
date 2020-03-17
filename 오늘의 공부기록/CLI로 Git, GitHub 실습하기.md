## 오늘의 할일

[x] GitHub 가입하기 
[x] Git 설치하고 로컬저장소에 커밋 관리하기 
[x] GitHub 원격저장소에 커밋 올리기

## 용어정리

- git : 소스코드 버전 관리 시스템
- gitHub : git으로 관리하는 프로젝트를 올려둘 수 있는 Git 호스팅 사이트.
- 왜 git을 사용할까?
    다른 개발자와 소스코드 협업을 위해서 git을 사용한다. GitHub에 프로젝트 소스 코드를 올려두면, 시간과 장소에 구애받지 않고 협업할 수 있다는 장점이 있다.
- git 호스팅 사이트 : GitHub, GitLab, BitButcket 등
-로컬저장소 : git을 통해 버전관리가 될 내 컴퓨터의 폴더. 즉, `git init` 명령어를 통해 생성되는 `[.git]` 폴더.
- 커밋 : 버전 관리를 통해 생성된 파일.
- git log : 지금까지 만든 커밋 히스토리 확인하기.
- git checkout : 원하는 커밋으로 되돌리기.
- 원격저장소 : GitHub에서 협업하기 위해 만든 저장소(공용 폴더).

## CLI로 Git, GitHub 실습하기

   1. 로컬 저장소 만들기

      ```js
      $ git init
      ```

2. 커밋 만들기

   2 - 1 )

   ```js
   $ git add 커밋에 추가할 파일
   
   예 ) $ git add README.txt
   ```

   2 - 2 )

   ```js
   $ git commit -m "커밋에 대한 상세 설명 작성"
   
   예 ) $ git commit -m "사이트 설명 추가"
   ```

   * [ -m  ] : 'message'의 약자

3. 원격저장소에 커밋 올리기

   3 - 1 ) 내 컴퓨터의 로컬저장소와 GitHub의 원격저장소 연결하기

   

   * 로컬저장소에서 원격저장소 주소를 아래의 명령어로 입력하기(한 번만 설정해주면 된다)

   ```js
   $ git remote -add origin "GitHub에 있는 원격저장소 주소"
   ```

   3 - 2 ) 로컬저장소에 있는 커밋들을 원격저장소에 올리기

   ```js
   $ git push origin master
   ```

   