# git-hub 사용 관련 이슈 정리 

1.로컬 저장소와 원격저장소 연결이 지속적으로 안됐었음 
- msg) refusing to merge unrelated histories
- 원인) 로컬저장소와 원격저장소간 차이가 많이 날 경우 발생함 

2.해결방법
- master branch에서 작업하지 말고 create new branch로 새 작업 
- 원격 저장소와 연결 : git branch --set-upstream-to=origin/master junyahn/python/1
- 강제로 원격저장소 pull 처리 : git pull --allow-unrelated-histories



-----------------------------------------------------------------------------------------------

# 신규 프로젝트 repository 등록 방법 

1. 해당 폴더 가서 [ git bash ] 

2. github 사이트에서 create repository 

3. bash 콘솔창에서  "git init "

4. git config 설정 
> git config --global user.email "superukie@naver.com" 
> git config --global user.name "superukie" 

5. remote branch 연결 
git remote add origin https://github.com/superukie/[repository주소] 

6. git add 
> 작업된 소스코드 add 
> git add * 

7. commit 
git commit "커밋메시지" 

8. git push -u origin master 
> origin master push  
