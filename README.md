# GIT- 기본명령어:CLI(Command Line Interface)

> Git 을 배워봅시다!!

---

## Git Bash 실행 후 사용자 설정

- 깃 헙 사용자 모두 설정 필요

```
git config --global user.email "가입된 이메일"

- git config --global user.email hyukjin4976@naver.com

git config --global user.name "깃헙이름"

- git config --global user.name JungHyukJin


* email 과 name 작성시 ""는 제외한다.

```

---

## Project Manager

```
1. Github 사이트 로그인 >> 우측상단 "+" 클릭 >> New Repository 생성 >> Repository Name & Description(해당 Repository 간단한 소개) 작성.

2. 생성 후 Repository창에서 URL을 복사.

3. 연동할 프로젝트 파일 오픈 후 git bash 실행.

4. git bash창에 아래 코드 차례대로 작성.
   git init   (이 파일을 깃으로 관리하겠다.)
   git remote add origin {project repository url} >> 복사한 URL을 {}를 포함한 위치에 붙여넣기.
   
5. 생성한 Repository창에서 우측에 Settings 클릭 >> 좌측에 Collaborators 클릭 후 초대.

```

---

## Collaborators (Contributors)

```
1. 초대받은 사람은 이메일 확인 후 수락.

2. Github 사이트 로그인 >> 해당 Repository 우측에 clone or download 클릭 >> URL 복사.

3. 본인 컴퓨터에서 연동할 프로젝트 파일 오픈, 우클릭 후 git bash 실행.

4. git clone {project repository url} >> {}를 포함한 위치에 URL 붙여넣기.

```

---

## Branch 설정

![branch](README.assets/branch.png)


    1. 브랜치 생성 : git branch {브랜치 이름}
    2. 브랜치 확인 : git branch
    3. 브랜치 이동 : git checkout {브랜치 이름}
    4. 브랜치 삭제 : git branch -d {브랜치 이름}
    5. 브랜치 생성 + 이동 : git checkout -b {브랜치 이름}

---

## git bash를 사용하여 깃허브에 업로드하기

```
1. git add . ( .은 모든 파일을 뜻함 / git add시, lf가 crlf로 바뀐다는 경고가 뜸 >> 무시해도 됨)

2. git commit -m "메세지 내용"

3. git push origin master

```

---

## 기타 명령어

```
1. pwd(Present Working Directory): 현재위치

2. cd(Change Directory): 폴더변경
                         / 는 현재 사용하는 컴퓨터의 경로 최상단을 의미 (root 폴더)
                         ~ 는 홈 폴더를 의미

3. ls: 현재 폴더 내부의 폴더, 파일들을 출력
   ls -a: 숨긴 폴더도 전부 표시
   (./ 앞에 .은 현재폴더,  ../은 상위폴더,  .git/ 의 .은 숨긴폴더를 의미)

4. touch.gitignore : 이그노어 폴더를 만들겠다. (가장 기본적인 설정)

5. git log: 이때까지 commit한 기록은 보겠다.

6. git log --oneline: 이때까지 commit한 기록을 한 줄로 보겠다.

7. git status: 상태확인 >> 항상 모든 명령어 뒤에 상태를 확인하자.

```

---



