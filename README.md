# git-hub 사용 관련 이슈 정리 

1. 로컬 저장소와 원격저장소 연결이 지속적으로 안됐었음 

msg : refusing to merge unrelated histories
원인 : 로컬저장소와 원격저장소간 차이가 많이 날 경우 발생함 

해결방법 : 

1. master branch에서 작업하지 말고 create new branch로 새 작업 
2. 원격 저장소와 연결 : git branch --set-upstream-to=origin/master junyahn/python/1
3. 강제로 원격저장소 pull 처리 : git pull --allow-unrelated-histories



