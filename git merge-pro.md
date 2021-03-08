https://git-scm.com/book/ko/v2/Git-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EB%B8%8C%EB%9E%9C%EC%B9%98%EC%99%80-Merge-%EC%9D%98-%EA%B8%B0%EC%B4%88

# 패스트 포워드에 대한 이해
- c0-c1-[c2:main] :: 이슈발생 
- c0-c1-[c2:main]-[c3:iss53] :: 이슈53 대응
- c0-c1-[c2:main]-[-c3:iss53,-c4:hotfix]  :: 핫픽스대응
- c0-c1-c2-[-c3:iss53,-c4:hotfix,main] :: 통합 :: fast-forward :: merge :: 자리 이동만 일어남
- c0-c1-c2-[-c3:iss53,-c4:main] :: 핫픽스 삭제
- c0-c1-c2-[-c3-c5:iss53,-c4:main] :: 이슈53 해결
- c0-c1-c2-[-c3-c5:iss53,-c4]-[c6:main] :: 통합 :: recursive 전략 , three-way merge, merge commit 이라고 부름
    - 충돌: 같은 부분 merge시 발생
    - 충돌 해결 : git status 로 충돌 부분 탐색
- c0-c1-c2-[-c3-c5,-c4]-[c6:main] :: 이슈53 삭제

