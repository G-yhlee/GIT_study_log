# 스태쉬에 대한 이해
- c0-c1-[c2:main]-[~c3:iss53] 커밋 하지 않음
- c0-c1-[c2:main]-[c3:iss53:~] git stash :: 임시저장
- c0-c1-[c2:main]-[~c3:iss53] git stash apply :: 임시저장 적용 
- c0-c1-[c2:main]-[c3:iss53:~] git reset --hard HEAD 
- c0-c1-[c2:main]-[c3:iss53:~] git stash list :: 임시저장 목록 보기 
    - git stash 명령 => working directory 저장
    - ~ :: wip :: working in process
    - git stash apply; git stash drop; == git stash pop


