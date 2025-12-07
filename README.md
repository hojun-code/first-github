|code|work space|stage|head|
|:---:|:---:|:---:|:---:|
|git diff|O|O|X|
|git diff --staged|X|O|O|
|git diff HEAD|O|X|O|

|code|previous|after|
|:---:|:---:|:---:|
|git add {file}|work space|stage|
|git commit|stage|head|

|code|explain|
|:---:|:---:|
|cat {file}|{file} 내용 보기|
|echo {content} >> {file}|{content}를 {file}에 추가|
|echo {content} > {file}|{content}를 가진 {file}을 생성|
|git status|work space, stage, head 간의 차이를 확인|
|git status -s|git status의 간소화 버전|
|git log --oneline|한 줄로 변경 사항 확인|
|git commit -am {message}|변경 사항이 있는 모든 파일을 add하고 commit|
|git revert HEAD|이전 버전으로 되돌림|
|git reset --hard HEAD~|이전 버전을 복사해서 적용. 로그도 삭제되며, 이후의 버전을 삭제.<br>모든 저장소를 동일하게 맞춘다. (soft는 head만 변경, mixed는 head, stage 변경)|
|git config --global alias.{name} {command}|{name}을 호출하면 {command}를 실행시킴. git {name}으로 가능.|
|git revert HEAD --no-edit|이전으로 되돌리는데, 메시지를 오토로 넣음.|
|git stash|임시 저장소에 현재 작업 공간을 저장|
|git stash apply|임시 저장소의 것을 불러옴|
