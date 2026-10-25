# Git

## init

- `.git` 폴더 생성 (사진첩생성)

```
git init
```

## status

- 현재 폴더의 git 작업상태

```
git status
```

## add

- staging area에 올리기 (무대에 올리기)

```
git add <filename>
git add . # 모든 파일/폴더 올리기
```

## commit

- `.git` repository에 저장 (사진 찍기)

```
git commit -m "message"
git commit --amend -m "fix message" # 마지막 커밋 메세지 수정
```

## log

- git 히스토리 출력

```
git log
git log --oneline # 핵심만 출력
```

## remote add

- 원격저장소 주소를 별명(origin)으로 추가

```
git remote add origin https://github.com/SESAC-SD4/TIL.git

```

## push

- 원격 저장소에 업로드

```
git push origin main
git push origin master
```

## restore

- 수정을 취소하기

```
git restore <filename>
git restore .
git restore --staged <filename> # 무대위에서 내린다
```