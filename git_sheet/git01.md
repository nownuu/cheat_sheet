## Git Sheet 01
------

### ■ 초기 설정
```bash
# 편집기 vscode로 설정
$ git config --global core.editor 'code --wait'
# 직접 변경
$ code ~/.gitconfig
```

```bash
# 사용자 설정
$ git config --global user.name "User name"
$ git config --global user.email "User email"

# CR(Carriage-Return)과 LF(Line Feed) 문자
$ git config --global core.autocrlf true  #window
$ git config --global core.autocrlf input #mac
$ git config --global core.safecrlf false
```

```bash
# 설정 취소
$ git config --global --unset <이름>

# 설정 보기
$ git config --global -list
```
<br>

----
### ■ 저장소 연동 기초

```bash
# 새로운 로컬 저장소 생성
$ git init [directory Name]

# 원격 저장소 내려받기
$ git clone [Repository URL]

# 원격 저장소 별칭 확인
$ git remote 
$ git remote -v # +주소

# 현재 위치의 파일 추가
$ git add [directory]
$ git add . # 현재 위치의 모든 파일 추가

# 커밋
$ git commit –m 'messege'

# 현재 위치의 파일 추가 및 커밋
$ git commit -am 'messege'

# 깃 현재 상태확인
$ git status
$ git log
$ git log --oneline # 요약 확인

```
<br>

-----
### ■ 깃 브랜치 생성
```bash
# 브랜치 생성
$ git branch [branch name]
$ git checkout -b [branch name]
$ git switch -c [branch]

# 브랜치 변경
$ git checkout [branch]

# 브랜치 삭제
$ git branch -d [branch]
```