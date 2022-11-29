---
layout: post
title: About git
subtitle: git literally from hell
comments: true
tags: [git]
---

# git

"The information manager from hell"

2005년 리눅스 개발자인 리누스 토발즈가 git을 내놓으며 한 말이다.

말 그대로 "지옥"에서 온 git이다.

git을 모르던 내가 중고딩 때 열심히 만들어 놓은 피피티가 날라가거나 수정할 때마다 파일명 뒤에 수정, 최종, 진짜 최종을 지저분하게 적어가며 고쳤던 기억이 난다. 리누스 토발즈가 말한 지옥이란 이런 어려움일 것이다.

---

**git**은 버전 관리 시스템의 일종으로 우리가 작업한 변경 사항을 저장하고 필요에 따라 특정 시점으로 돌아가고, 협업도 가능하게 해준다.

## 파일 상태
<img src="../assets/img/lifecycle.png"/>

### - unstaged (untracked)
git이 버전관리를 하지 않은 상태
### - staged (tracked)
git이 변경 사항을 추적하고 있는 상태, 즉 버전관리 중인 상태

    git add <원하는 파일>
add로 unstaged(untracked)를 staged(tracked) 상태로 바꾼다.

### - commit
변경 사항을 저장, commit 하나 당 체크포인트라고 생각하면 된다.

    git commit -m <커밋 메시지>

### - modified
commit한 파일이 변경된 상태

### - ignored
git이 무시하는 파일, 즉 버전 관리 하지 않는 파일. 주로 정적 파일이나 빌드된 파일 등이 이에 해당한다.