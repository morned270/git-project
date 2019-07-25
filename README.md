#Git 자주 사용하는 명령어 정리



#코드 블록으로 인식하게 하는 백틱(`)
```python
import this
```


#진행 흐름

1. cd 명령어를 통해서 init할 저장소 위치로 이동
(예: cd /c/git/git-project)

2. git init
2-1. ls -al을 했을 때 .git 디렉터리가 생성된 것을 볼 수 있다

3. touch README.md로 README.md 파일 생성
3-1. git status를 했을 때 README.md가 Untracked files에 있는 것을 볼 수 있다

4. git add README.md로 README.md 파일을 스테이지에 올린다
4-1. git status를 했을 때 README.md 파일이 스테이지에 있고, 따라서 커밋할 수 있음을 확인할 수 있다

5. git commit -m "Init: README.md"와 같이 커밋한다
(형식: git commit [옵션] "커밋메시지")


