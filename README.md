#Git 자주 사용하는 명령어 정리



#코드 블록으로 인식하게 하는 백틱(`)
```python
import this
```


#진행 흐름

##1. 저장소 초기화 / 환경설정

01. 저장소에 해당하는 폴더를 만든 후, cd 명령어를 통해서 해당 위치로 이동
(예: cd /c/git/git-project)

02. 해당 위치에서 git init
2-1. ls -al을 했을 때 .git 디렉터리가 생성된 것을 볼 수 있다

3. touch README.md로 README.md 파일 생성
3-1. git status로 현재 상태를 보면 README.md가 Untracked files에 있는 것을 알 수 있다

4. git add README.md로 README.md 파일을 스테이지에 올린다
4-1. git status로 현재 상태를 보면 README.md 파일이 스테이지에 있고, 따라서 커밋할 수 있음을 확인할 수 있다

5. git commit -m "Init: README.md"와 같이 커밋한다
(형식: git commit [옵션] "커밋메시지")
5-1. 커밋메시지는 Init: README.md와 같이 형식을 갖추도록 한다
5-2. git log --decorate=full --oneline --graph로 커밋이 잘 되었는지 로그를 확인한다

6. git checkout -b readme로 readme라는 브랜치를 새로 만들고, 
(브랜치는 대개 만들고자 하는 기능의 단위로 사용한다)



8. 터미널에서 합칠 기준점이 되는 브랜치로 이동한 후에 머지해야하므로,
git checkout master #합치는 기준점이 되는 master 브랜치로 이동!

git log --oneline --graph --all

git remote add [저장소 주소]로 #저장소 추가
리모트 저장소 이름은 origin으로 하는 것이 일반적!
(예: git remote add origin https://github.com/morned270/git-project.git)

git remote -v로 리모트 저장소가 잘 지정됐는지 확인