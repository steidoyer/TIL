# linux

## 명령어 구조

- 셋 사이는 `띄어쓰기`로 구분합니다.
  - brewinstall --cask iterm2 # 띄어쓰기 없이 쓰면 없는 명령어라고 나옴

```
명령어 옵션 대상
ls -l notes

프로그램 이름 / 동작 / 기능 / 설치할 거
brew install --cask iterm2
```

## 경로

- `~`: 내 홈 폴더
- `.`: 지금 있는 폴더
- `..`: 한 칸 위 폴더
- `/`로 시작: 절대 경로
- 나머지: 상대 경로

## 명령어

- pwd (print working directory)
  **지금 위치 항상 알고있기**

```
pwd
```

- ls (list)

```
ls # 현재 위치의 내용 보여줌
ls TIL # 특정 폴더 안의 목록
ls -l # 자세히 보기
ls -a # 숨김 파일(.으로 시작하는 파일/폴더)까지 보여줌
ls -a =>  ./ 현재 위치 폴더 ../ 상위 폴더 TIL/
ls -la # 옵션 붙여서 적용도 됨. 옵션 붙여쓰기는 모든 명령어가 다 되는 건 아님.
```

- cd (change directory)
  - 파일이나 폴더는 tao키로 자동완성 사용 권장

```
cd ..
cd SD4
cd ~ # 홈으로 이동
cd SD4/TIL # 특정 폴더로 바로 이동
cd s (tab 1번 내지 2번 누르기) # s 시작하는 파일이나 폴더 보여줌
```

- mkdir (make directory)

```
mkdir temp # temp라는 폴더 생성
mkdir -p temp/hi #중간의 부모 폴더까지 한번에 생성
```

- touch (파일 생성)

```
touch test.txt # text.txt 이름으로 빈 파일 생성
```

- echo

```
echo '안녕하세요'
```

- `>` (새로쓰기), `>>` (덧붙이기) : 출력(결과, 리턴?)을 파일에 입력

```
echo 'hello' > test.txt # test.txt 파일에 'hello' 문자열이 들어감. 명령어를 실행할 때마다 새로 쓰고 있으면 덮어쓴다.
echo 'world' >> text.txt # 끝에 덧붙이기
ls > test.txt # ls의 출력값을 test.txt에 입력
```

확장자라는 건 이 파일을 '무슨 프로그램'으로 실행시킬지에 대한 표시같은거.
확장자가 이상해도 파일은 만들어짐.

- 파일 내용 보기
  - `cat`: 파일 내용 출력
  - `head`: 앞부분 출력
  - `tail` 뒷부분 출력
  - `less`: 새로운 레이어에 출력

- cp(copy) mv(move), rm(remove)
  리눅스는 기본적으로 폴더는 삭제하지 않음
  - `rm -r`: 폴더 삭제(recursive)

```

```

- `grep`, `|`
  - 잡다
  - 나중에 서버 로그 보거나 이럴때 많이 씀
  - 파일 결과 많은거에서 추려서 보게

```
grep touch linux.md # linux.md 파일에서 touch가 들어간 줄 출력
ls -l | grep linux #
```

- which
  - 이 명령어가 어디있는지 출력
  - 프로그래밍 언어가 어떤 경로로 잡혀있는지 볼때 사용

```
which node
```

- `--help`: 거의 대부분 명령어의 설명 출력

```

```
