# git-study-howto
Git how to doc

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
