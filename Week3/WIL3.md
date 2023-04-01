# WIL3
***
## git 명령어 공부

#### commit
 : Git 저장소에 나의 디렉토리에 있는 모든 파일에 대한 스냅샷을 기록하는 것

#### branch
 : commit의 복사본 

> git branch 이름 : 브랜치 생성
> git switch 이름 : 브랜치로 이동

<img src="https://user-images.githubusercontent.com/128215774/229275622-6bd54155-d9c7-4187-a3ec-d347265e90eb.jpg" width="500" height="400"/>

>git switch main
> git merge 대상

→ main 브랜치에 병합
<br/>
>git checkout experiment
>git rebase master


<img src="https://git-scm.com/book/en/v2/images/basic-rebase-3.png" width="500">


rebase를 하든, merge를 하든 최종 결과물은 같고 커밋 히스토리만 다르다. 

다만, rebase가 더 깨끗한 히스토리(→선형)
<br/>
#### HEAD
 : HEAD는 현재 체크아웃된 커밋을 가리킴. 즉, 현재 작업중인 커밋
 
 ***

 ## 과제를 한 과정..
- git clone을 통해 내 노트북에다가 webstudy-homework-yeonee911 파일 생성
- git init 작성 :  이후 branch를 생성하려 했으나 오류 : 구글링 결과, 하위 폴더에 .git파일 존재 시 발생하는 오류로 추정. 그래서 .git 파일 삭제함
- git branch yeonee911을 통해 branch를 생성하려 했으나 오류 : 구글링 결과, 한번도 commit하지 않은 파일이라서 발생한 오류 추정
- git add webstudy-homework-yeonee911
- git commit -m "메모" : 커밋 메모 없이 'git commit'만 작성 시 먼가 이상한 창이 뜸.. 메모를 꼭 작성해야겠다는 것을 깨달음. 
- 가까스로 git branch yeonee911 생성
- git switch yeonee911 : master에서 yeonee911로 변경 성공
- yeonee911 폴더 생성 후 그 안에 리드미 파일 생성
- github desktop을 통해 제출하려 했으나 제출 실패
- push 하는 법을 모르겠음..!!
- 결국.. 아린이에게 도움 
- 첨부터 다시 시작...
- 이번에는 vsc에서 명령어 대신 github에서 new branch를 통해 yeonee911 브랜치 생성
- 깃헙 데스크탑에서 add에서 clone repository를 선택한 게 문제였던 거 같음..?