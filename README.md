# Git (분산형 버전 관리 시스템)

## GIT vs Gihub

* GIT
  * 소프트웨어 개발 및 소스코드 관리에 사용
  * 로컬에서 버전관리를 하지만 다른 사람과 실시간으로 코드를 공유할 수 없다
 
* Github
  * git repository를 위한 웹기반 호스팅 서비스
  * 클라우드 서버를 사용하여 로컬에서 관리한 코드를 업로드하여 공유할 수 있다

### GIT의 작업 영역

* working directory
* staging area(index영역)
* repository

git init -- 현재 위치를 git저장소로 지정한다는 말, 해당 위치에 .git이라는 폴더가 생성된다<br>
git status -- 변경된 파일이 있는지 감지한다<br>
git add . -- 변경된 파일을 staging area에 add한다 파일이 트리구조로 인덱스 영역에 들어간다<br>
git commit -m "" -- commit 된 파일들이 버전별로 관리된다
git branch --현재 브랜치 보기(뒤에 단어를 쓰면 새로운 브랜치를 생성한다)<br>
git checkout A --'A'라는 브랜치를 사용하겠다고 명시적으로 지정<br>
> 체크아웃에 -b 옵션을 넣으면 브랜치 작성과 체크아웃을 동시에 실행 할 수 있다<br>

git push -- (업로드+merge)를 뜻한다

### Branch의 기본 개념
형상이란... 브랜치의 히스토리를 말한다
 * 3way-merge(형상이 다를 때)
 * fast-forward merge(형상이 같을 때)
   * 두개의 브랜치가 있는 상태에서 더 앞쪽에 있는 브랜치로 HEAD를 옮기고'git merge (head브랜치보다 더 뒤에있는 브랜치)'를 적어주면 merge가 된다
