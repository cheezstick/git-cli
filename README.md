:hamburger: CLI를 사용한 깃헙 푸시
=================================

### 1. .git 파일 생성

> ### 기본
> ```
> git init              # .git 파일 생성
> git status            # 현재 git 상태 확인 
>                       # GUI 소스 제어에서도 확인 가능
> ```

#### .gitignore
DS_Store/thumb.db와 같은 무시하는 것들 넣기


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

> ### merge - branch 병합
>```
> git checkout main         # 병합할 branch로 이동
> git merge cheez           # cheez branch 병합
> git branch -d cheez       # cheez branch 삭제
>```


### 3. add & commit

> ### add - untracked/modified :arrow_right: tracked
>```
> git add 파일이름           # 해당 파일만 tracked 상태로
> git add .                 # 모든 파일을 tracked 상태로
>```

> ### commit 
>```
> git commit                # 메시지 입력 창이 뜸뜸
> git commit -m '1st'       # 1st라는 메시지로 커밋
> git commit -?? '1st'      # add + commit
> git commit --amend -m '~' # 기존 커밋 메시지 수정
>```


### 4. 깃헙 푸시

>```
> git remote add origin 저장소링크     # 현재 프로젝트를 원격 저장소와 연결
> git remote -v                       # 연결된 저장소 정보 확인
> git push origin main                # 깃헙 푸시
> git push -u origin +main            # README 파일 존재 시 덮어쓰기
>```
