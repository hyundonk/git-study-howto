# git-study-howto
Git how to doc

## branch에서 작업한 내용을 main에 반영하기
```
# 현재 branch 확인
git branch

# 먼저 branch 작업 한 내용을 해당 branch의 원격지에 반영
git commit -m "initial working version"

# local repo의 main branch로 변경
git checkout main

# 작업했던 branch와 merge
git merge branch-name

# Remote repo에 반영
git push origin main
```


## 
특정 Tag로 부터 수정한 내용을 새로운 branch에 반영하는 방법

```
# Local에 clone된 repository로 부터 'v1.1' tag를 checkout
$ git checkout v1.1

# check current branch
$ git branch
* (HEAD detached at v1.1)
  master

# check current tag
$ git describe --tags
v1.1

# 변경 후 git add, git commit으로 반영

# 'new-branch'로 push (해당 branch가 없는 경우 -u 옵션을 사용)
$ git push -u origin new-branch

```

Ref)
https://devconnected.com/how-to-push-git-branch-to-remote/
