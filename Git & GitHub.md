# Git & GitHub

### 리눅스 명령어

- 현재 경로 표시

  `$ pwd`

- 현재 디렉터리의 내용 표시

  `$ ls`

- 디렉터리 이동하기

  `$ cd`

- 텍스트 문서 내용 확인하기

  `$ cat`



### 구조

**작업 트리(로컬)** -(add)-> **스테이지** -(commit)-> **저장소** -(push)-> **원격 저장소**



### repository 생성 후 처음 push 할 때

```bash
# README파일 생성
echo "# repository이름" >> README.md
# 깃 초기화
git init
# add
git add README.md
# commit
git commit -m "first commit"
# 저장소 연결
git remote add origin https://github.com/계정이름/repository이름.git
# push
git push -u origin master
```



### repository에서 pull 받기

```bash
git pull
```



### Git 명령어

- 깃 상태 확인

  `$ git status`

- 커밋한 기록 확인

  `$ git log`



- 방금 커밋한 커밋메시지 수정하기

  `$ git commit --amend`

- 로컬에서 수정한 파일 되돌리기

  `$ git checkout -- [파일명]`

- 스테이지에 올린 파일 되돌리기

  `$ git reset HEAD [파일명]`

- 마지막 커밋 되돌리기

  `$ git reset HEAD^`

- 특정 커밋으로 되돌리기

  `$ git reset --hard [되돌릴 커밋 해시]`



- 브랜치 목록 확인하기

  `$ git branch`

- 새 브랜치 만들기

  `$ git branch [브랜치이름]`

- 브랜치 이동하기

  `$ git checkout [브랜치이름]`

- 브랜치 삭제하기
  - master 브랜치에 병합이 끝난 브랜치

    `$ git branch -d [브랜치이름]`

  - master 브랜치에 병합하지 않은 브랜치

    `$ git branch -D [브랜치이름]`

