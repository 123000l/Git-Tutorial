* remote repository 는 깃, local repository는 컴퓨터.
* contribution은 오픈 소스 활동. 이력이 된다.
* config 환경설정.


## 깃

+ 장점 : 병렬적 개발이 가능하다. 개발 속도를 높일 수 있다. ( 요즘에는 포트폴리오로 사용한다.)
+ 특징 
   * 분산적 : 합치기(merge)가 가능하여 전체 개발 내용을 각 개발자 로컬 컴퓨터로 보내 다수 개발자가 함께 작업이 가능하다.
   * 효율적 : 변경 이력이 많아도 변경된 내용만 처리하므로 메모리적 효율성이 높다.
   * 비선형 : 브랜치(branch)로 충돌 발생 시 관리가 용이하다.
   * 변경 이력이 보장된다.           



 ## 동작 원리

순간을 중요시하여 수정내역을 저장한다.
* Working Directory : 작업할 파일이 존재하는 공간.
* Staging Area : 커밋(commit)을 수행할 파일이 올라가는 영역.
* Git Directory : Git 프로젝트의 메타 데이터와 데이터 정보가 저장되는 디렉토리.


## 소스 코드 수정

소스 코드를 수정할 때는 두 가지의 상황으로 나눌 수 있다.
1) 해당 프로젝트에 소속되어 있지 않을 때 (접근 권한이 없을 때)
-> fork로 복제.
2) 소속되어 있을 때
-> 그냥 커밋하고 푸시하면 됨.    


## 커밋 내역 수정하기
- 언제 수정되었는지 알 수 있고, 심지어 이전으로 되돌릴 수 있다.
  - 옵션
     + --hard : 특정 지점 이휴 증발시키겠다.
     + -f : 강제 push ( 사용법: git push -f)
     + --amend : 커밋 메시지 변경.   


## branch
+ 동시에 여러 명이 작업할 수 있게 해줌.
#### 마스터 브랜치 (master branch)
* 언제나 작동해야함.
* 언제나 배포 가능해야함.
* 안정적으로 작업할 수 있게 해줌.

* checkout 으로 branch 관리
   * -d 는 브랜치 삭제.   

## 원격 저장소 관리
* 원격 저장소는 네트워크 안에 존재하는 또 다른 컴퓨터를 말한다.
* 받아올 때 pull, 들어올 때 push.
* remote 옵션
  - -v : 전체 목록 확인.
  - rm : 삭제    

## log
- 다양한 커밋 내용을 시간 순서에 따라 볼 수 있다. 즉, 처리 내역(history)를 볼 수 있음.
- 옵션
    + --stat :  모든 파일 통계 보여줌.
    + pretty : 지정 형식으로 출력해줌. (%an : author, %ar : 날짜)       
