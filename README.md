:hamburger: CLI를 사용한 깃헙 푸시
=================================

### 1. .git 파일 생성

```
git init              # .git 파일 생성
git status            # 현재 git 상태 확인 
```

### 2. 파일 수정

> ### log - history 확인
> ```
> git log                   # git history를 CLI로 확인
>                           # commit 옆 내용 = 커밋ID
> git log --oneline         # hash를 짧게 표현, 한 줄로 log 확인
> ```

> ### reset - 해당 커밋ID 상태로 이동
>```
> git reset --soft 커밋ID   # Working directory & staging 초기화
> git reset --hard 커밋ID   # Working directory & staging 유지
>```

> ### checkout - branch 이동
>```
> git checkout cheez        # cheez branch가 있는 경우
> git checkout -b cheez     # cheez branch를 새로 만들고 이동하는 경우
>```

### 3. add & commit


### 4. 깃헙 푸시시

