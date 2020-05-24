---
title : "Don't Mess with the Mater 번역본"
cateories :
 - "Git공부"
---

※ 번역하면서 번역오류가 발생된 부분들이 있을 수 있습니다. 지적 해주시면 감사하겠습니다~

원문 : https://thenewstack.io/dont-mess-with-the-master-working-with-branches-in-git-and-github/

지금까지 여러분들은 git이 사용자에 의해 커밋되엇을 때 각 버전 별로 소스를 저장하는 것에 대해 알고 계실 겁니다.
기본적으로 프로젝트의 버전관리는 어떠한 버그 발생시 이전버전으로 되돌리기 위해 이루어집니다.

이러한 Git과 GitHub는 특히 한 명 이상의 작업자가 한 프로젝트에서 어떤 변경점을 발생시킬 때, 이를 "Branch"로 프로젝트 버전을 관리합니다.
한 개의 저장소(Repository)는 한 개 이상의 Branch를 가질 수 있습니다.
Main Branch는 모든 변경사항을 다시 병합하는 Branch를 뜻하며 이를 "Master" 라고 부릅니다.

Master Branch를 지나치게 사용하지 마세요. 만약 여러분들의 프로젝트 번경점을 바로 Master Branch에 적용시키면서 다른 사용자 또한 Master Branch를 가지고 업무를 진행하게 된다면,
여러분들이 사소하게 소스를 수정했음에도 모든 사용자들에게 영향이 끼치며 이는 병합 충돌을 일으키며 큰 절망감에 휩사이게 될 것입니다.

Master Branch 왜 자니차게 사용하면 안될까요? 간단합니다. Master Branch는 상용화되어 있습니다. 즉 여러분들의 코드가 세상에 출시될 준비가 마쳤다는 겁니다. 
Master Branch는 안정적인 상태여야 합니다. 그리고 오픈 소스 소프트웨어 규범에는 "테스트가 되지 않은 코드를 함부로 Master Branch에 넣지 않도록 되어 있으며 이를 지키지 않을 경우 해당 프로젝트는 무너진다"고 되어 있습니다.
이러한 이유로 Github에서는 언제나 Maseter Branch로부터 안전하게 작업해야 합니다.

====================

Mess with : 남용하다
Essential : very important - 가본적인
Disaster : 버그
On the fly : 즉석으로
Ripple out : 영향을 끼친다
Roll out : to make a new Service for the first time -> 출시하다

====================