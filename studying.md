### **5장 - 서버(server)**

01. 깃허브 서버 준비
02. 깃허브 연동 및 원격 등록
03. 서버 전송
04. 자동으로 내려받기
05. 수동으로 내려받기
06. 순서

본 프로젝트는 프로젝트 진행 시 원활하게 코드를 관리하기 위해
서버를 이용하는 방법을 소개하고 있습니다.

요약
로컬저장소와 서버(원격 저장소)를 연동하고,
작성한 파일을 서버에 올리거나, 서버에 저장된 코드를 내려받을 수 있습니다.

### ** 6장 - 브랜치(branch)**

01. 브랜치 생성 및 확인
02. 브랜치 이동 및 공간
03. HEAD 포인터 & 브랜치 생성과 이동
04. 원격 브랜치
05. 브랜치 전송
06. 브랜치 삭제

본 프로젝트는 프로젝트 진행 시에 구현하게 될 각 기능, 버그 들을
branch 라는 작업의 흐름으로 나누어 작업하는 방법을 소개하고 있습니다.

요약
하나의 기능 작성 또는 디버깅 시 새로운 브랜치를 만들게 됩니다.
새 브랜치를 만들 때 원하는 커밋을 HEAD로 지정할 수 있으며, 해당 브랜치에서 원격 저장소에 push 하거나, main 브랜치에 병합할 수 있습니다.
생성한 브랜치의 사용을 다 했을 때, 해당 브랜치를 삭제할 수 있습니다.

### ** 8장 - 병합(merge)**

01. Fast-Forward
02. 3way
03. 브랜치삭제
04. 충돌
05. 병합확인
06. rebase

Chapter 6에서 설명한 브랜치를 합치는 명령
즉, 각각의 작업의 흐름을 하나로 합칠 수 있는 방법을 소개하고 있습니다.

요약
merge 명령을 통해 병합하고자 하는 브랜치 끼리의 상태를 비교하여,

1. 병합을 받는 브랜치(A)가 병합 해오려는 브랜치(B)의 조상 커밋이라면,
fast-forward 방식을 사용하여 브랜치(A)의 커밋이 병합을 해오려는 브랜치(B)와 같은 커밋을 HEAD로 가지게 됩니다.
2. A 브랜치가 B 브랜치의 조상 커밋이 아니라면
3way 방식을 사용하여 두 브랜치를 합친 새로운 커밋을 생성하고 A의 HEAD는 생성된 커밋을 가르키게 됩니다.

### ** 9장 - 복귀(reset, revert)**

01. 리셋(reset)
02. 리버트(revert)

본 프로젝트는 여태 진행한 커밋들 중 일부 커밋을 취소하려고 할 때 사용할 Git 명령어를 소개하고 있습니다.

요약
Git 사용 시 진행했던 커밋을 이전으로 돌려야 하는 상황이 올 수 있습니다.
이때, reset & revert 명령어로 돌아갈 수 있습니다.
