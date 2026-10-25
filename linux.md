# Linux

## 명령어구조

- 셋 사이는 **띄어쓰기**로 구분합니다.
  - `brewinstall --cask iterm2` : 띄어쓰기 없이 쓰면 없는 명령어라고 나옴

```
명령어 옵션 대상
ls    -l   notes
brew install --cask iterm2
```

## 경로

- `~` : 내 홈 폴더
- `.` : 지금 있는 폴더
- `..` : 한 칸 위 폴더
- `/`로 시작 : 절대 경로
- 나머지 : 상대 경로

## 명령어

- pwd (print working directory)

```
pwd
```

- ls (list)

```
ls
ls TIL # 특정 폴더의 목록
ls -l # 자세히 보기
ls -a # 숨김 파일(.으로시작하는 파일/폴더)까지
ls -la
```

- cd (change directory)
  - 파일이나 폴더는 TAP으로 자동완성 사용 권장

```
cd ..
cd SD4
cd ~ # 홈으로 이동
cd SD4/TIL # 특정폴더로 바로이동
```

- mkdir (make directory)

```
mkdir temp # temp라는 폴더 생성
mkdir -p temp/hi # 중간의 부모 폴더까지 한번에 생성
```

- touch

```
touch test.txt # test.txt 이름으로 빈파일 생성
```

- echo

```
echo '안녕하세요'
```

- `>` (새로쓰기), `>>` (덧붙이기)

```
echo 'hello' > test.txt # 새로 쓴다 (있으면 덮어쓰기)
echo 'world' >> test.txt # 끝에 덧붙이기
ls > test.txt # ls의 출력값을 text.txt에 쓰기
```

- 파일 내용 보기
  - `cat` : 전부 출력
  - `head -3` : 앞부분 출력 (옵션을 입력하는 경우 그 줄만큼)
  - `tail -2` : 뒷부분 출력
  - `less` : 새로운 레이어에 출력

- cp(copy), mv(move), rm(remove)
  - `rm -r` : 폴더 삭제 (recursive)

```
cp test.txt temp (복사)
mv test.txt temp2 (이동)
mv test.txt result.txt (이름 바꾸기, 같은폴더에서 이동)
rm result.txt (파일삭제 - 휴지통 없음 주의!!!)
rm -r temp (폴더삭제)
```

- `grep`, `|`

```
grep touch linux.md # linux.md파일에서 touch가 들어간 줄 출력
ls -l | grep linux # ls -l 출력결과 중에서 linux가 들어간 줄만 보기

```

- which
  - 이 명령어가 어디있는지 출력

```
which node (node명령어 위치)
```

- `--help` : 거의 대부분 명령어의 설명 출력