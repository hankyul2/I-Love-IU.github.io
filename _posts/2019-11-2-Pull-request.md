---
title: "Pull Request"
date: 2019-11-03 20:23:11 -0400
categories: Git
---
# PULL REQUEST

##목차
1. BACKGROUND-KNOWLEDGE: TOPIC-BRANCH and INTERGRATION-MANAGER WORKFLOW
2. GITHUB WORKFLOW: CONTRIBUTION
3. PULL REQUEST 사용하기 WITH ISSUES AND COMMITS
4. PULL REQUEST REVIEW
5. PULL REQUEST CLOSE

## 1. BACKGROUND-KNOWLEDGE: TOPIC-BRANCH and INTERGRATION-MANAGER WORKFLOW
GITHUB에서 contribution하는 방법: 내 REPO인 경우에는 그냥 푸쉬 하면 된다. 하지만 그렇지 않을 경우 FORK & PULL REQUEST라는 것을 해야한다. 이것을 이해하기 위해서는 TOPIC BRANCH & INTERGRATION MANAGER 라는것을 이해해야한다.

TOPIC BRANCH라는 것은 해결하고자 하는 이슈나 기능을 만들기 위해서 만든 브런치를 가르킨다. 깃허브에서는 이런 토픽 브런치를(이슈 브런치) 중심으로 작업을 진행한다. 즉, 프로젝트에 필요한 것들을 이슈화 해서 제시하면 여러 사람들이 그 이슈를 해결하기 위한 브런치를 생성하고 그 브런치에서 작업을 하는 것이다. 기존의 VCS에서는 브런칭을 하는것이 High-Cost이기 때문에 하기 쉽지 않았지만 깃은 그렇지 않기에 적극적으로 사용해도 프로젝트에 부담이 되지 않는다. 토픽 브런치에 대한 자세한 정보를 얻고 싶다면 다음 사이트를 추천한다. [git-book-topic_branch][2]
> A topic branch is a short-lived branch that you create and use for a single particular feature or related work.  

토픽 브런치외에도 깃허브의 work-flow를 이해하기 위해서는 깃의 work-flow 중 하나인 인터그레이션 매니저라는 것을 이해해야 한다. 깃은 리모트 저장소를 여러개로 등록할 수 있다. 따라서 각 개발자는 자신의 리모트 저장소에는 쓰기 권한을 가지고 나머지는 읽기 권한만 가지는 상황이 있을 수 있다. 이제 하나의 프로젝트가 있고 그 프로젝트에 기여 하고자 하는 개발자가 여러명 있다고 가정하자. 각 개발자는 대상 프로젝트를 카피해서 자신의 프로젝트로 만든다. 이 프로젝트는 원래 프로젝트와 완전히 내용이 같으나 개발자 자신의 프로젝트이므로 본인이 수정한 코드를 커밋해서 푸쉬 할 수 있다. 이렇게 커밋을 자신의 프로젝트에 푸쉬한 뒤 개발자는 원본 프로젝트의 관리자에게 연락을 한다. 자신의 변경된 커밋을 PULL해서 원본 프로젝트에 반영 시켜 달라고. 연락을 받은 관리자는 개발자가 보낸 변경 사항과 설명을 듣고 자신이 로컬에서 직접 테스트 해본다. 만약 괜찮다면 Merge & Push 할 것이고, 아니라면 개발자에게 추가로 수정할 부분에 대해서 comment를 남기거나 reject를 할 것이다. 이러한 work-flow를 Intergration-Manager라고 하고 GITHUB에서는 개발자가 관리자(Maintainer)에게 연락을 할 때 사용하는 방법이 PULL REQUEST인 것이다. 이 방법에(Intergration-Manager) 대해 더 알고 싶다면 다음 글을 읽는 것을 추천한다. [git-book-intergration_manager][3]

위에서 길게 길게 설명한 글을 다 읽었다면 이제 실제로 PULL REQUEST를 사용하는 예제를 살펴보자.

## 2. GITHUB WORKFLOW: CONTRIBUTION
만약 내가 기여하고 싶은 프로젝트가 있다, 그리고 PUSH할 권한이 있다면 그냥 푸쉬하면 된다. 하지만 아쉽게도 그 프로젝트의 MAINTAINER가 내 친구가 아닌이상 대부분 프로젝트 레포지토리에서는 나에게 CLONE이상의 권한을 주지 않는다. 그렇다면 그냥 기여하는 것을 포기해야 하는가? 그렇지 않다! FORK & PULL REQUEST 라는 방법을 사용하면 나에게도 멋진 프로젝트에 멋지게 기여할 방법이 있다. 우선 기여할 프로젝트를 고르는것 부터 시작한다. # N

## 3. PULL REQUEST 사용하기 WITH ISSUES AND COMMITS
## 4. PULL REQUEST REVIEW
## 5. PULL REQUEST CLOSE

ROW 글




[1]: https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project
[2]: https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows#_topic_branch
[3]: https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows#_integration_manager
