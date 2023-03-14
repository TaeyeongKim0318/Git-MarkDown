
## Git 이란
소스코드를 효과적으로 관리할 수 있게 해주는 무료 소프트웨어로 **버전 관리 시스템**의 일종이다.

## Git의 기능
1. Backup  
만약의 사태에 대비할 수 있다.
2. Recovery  
이전 상태로 돌아갈 수 있다.
3. Collaboration  
다른 사람과 협업이 가능하다.

## Git 실습 자료
생활 코딩의 [지옥에서 온 Git](https://www.youtube.com/watch?v=hFJZwOfme6w&list=PLuHgQVnccGMA8iwZwrGyNXCGy2LAAsTXk)을 통해 
[Git for Windows](https://gitforwindows.org/)를 다운로드 후 설치

## Git 명령어 정리
### git init  
관리할 폴더를 지정한다. 지정 시 '.git'이라는 폴더 생성되는데 삭제하면 안된다.  
```bash
git init
```

### git config
버전을 관리하고 있는 유저명과 이메일을 설정한다.
```bash
git config --global user.name <유저명>
```
```bash
git config --global user.email <이메일>
```

### git status  
폴더 내 파일들의 상태를 알려준다.
```bash
git status
```
**워킹 디렉토리의 파일은 먼저 크게 Untracked, Tracked의 두 가지 상태로 나뉜다..**(워킹 디렉토리는 작업중인 로컬 컴퓨터의 공간이다.) 파일에 수정이 일어나면 git이 파일의 변경을 감지하여 사용자에게 알려주는 것과 같이 **파일을 추적하는 상태를 Tracked 상태라고 한다.** 반대로, 파일을 저장소에 저장할 필요가 없어 **git이 신경쓰지 않아도 되는 상태를 Untracked 상태라고 한다.**

파일을 새로 만들 경우 Untracked 상태 즉, git이 파일을 추적하지 않는 상태가 된다. git 저장소에 저장할 필요가 없는 파일들은 Untracked 상태로 두면 된다. 이후 git add 명령어를 이용하여 파일을 `add`해주면, 해당 파일은 staging area에 저장되어 Tracked 상태 즉, git이 파일을 추적하는 상태가 된다.

**Tracked 상태의 파일들은 다시 크게 Unmodified, Modified, Staged 3개의 상태로 나뉜다.** **staging area에 있는 파일들의 상태는 Staged이다.** staging area에 있는 파일들을 `commit`하게 되면 해당 파일들은 하나의 **`commit`으로 저장된 후, 파일의 상태는 Unmodified로 내려오게 된다.** **Unmodified 상태의 파일들을 수정하게 되면 Modified 상태가 된다.** 이후 다시 `git add` 명령어를 이용하여 Staged 상태로 올려준 후 `commit`을 하는 과정을 반복하게 된다.  
<img src=https://git-scm.com/book/en/v2/images/lifecycle.png>
  
  
- 테스트 
```bash
git add <파일 명>
```

