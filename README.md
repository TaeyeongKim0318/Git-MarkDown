
## Git 개요
#### Git 이란
소스코드를 효과적으로 관리할 수 있게 해주는 무료 소프트웨어로 **버전 관리 시스템**의 일종이다.

#### Git의 기능
- Backup  
  만약의 사태에 대비할 수 있다.
- Recovery  
  이전 상태로 돌아갈 수 있다.
- Collaboration  
  다른 사람과 협업이 가능하다.

#### Git  자료
생활 코딩의 [지옥에서 온 Git](https://www.youtube.com/watch?v=hFJZwOfme6w&list=PLuHgQVnccGMA8iwZwrGyNXCGy2LAAsTXk)을 통해 학습  
[Git for Windows](https://gitforwindows.org/)를 다운로드 후 설치

## Git 기본 
### git init  
관리할 폴더를 지정한다. 지정 시 '.git'이라는 폴더 생성되는데 삭제하면 안된다.  
```bash
git init
```

### git config
git이 commit할때 저장할 사용자의 정보를 설정한다.
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

파일을 새로 만들 경우 Untracked 상태 즉, git이 파일을 추적하지 않는 상태가 된다. git 저장소에 저장할 필요가 없는 파일들은 Untracked 상태로 두면 된다. 이후 `git add` 명령어를 이용하여 파일을 add해주면, 해당 파일은 staging area에 저장되어 Tracked 상태 즉, git이 파일을 추적하는 상태가 된다.

**Tracked 상태의 파일들은 다시 크게 Unmodified, Modified, Staged 3개의 상태로 나뉜다.** **staging area에 있는 파일들의 상태는 Staged이다.** staging area에 있는 파일들을 commit하게 되면 해당 파일들은 하나의 **커밋으로 저장된 후, 파일의 상태는 Unmodified로 내려오게 된다.** **Unmodified 상태의 파일들을 수정하게 되면 Modified 상태가 된다.** 이후 다시 `git add` 명령어를 이용하여 Staged 상태로 올려준 후 commit을 하는 과정을 반복하게 된다.  
<img src=https://git-scm.com/book/en/v2/images/lifecycle.png>

### git add
워킹 디렉토리의 파일을 스테이징 영역에 추가한다.
```bash
git add <파일명>
```

### git commit
스테이징 영역에 있는 파일을 저장한다.
```bash
git commit
```
-m 옵션을 이용하면 vim을 사용하지 않고 메세지를 저장할 수 있다.
```bash
git commit -m "<저장할 메세지>"
```

### git log
git의 로그를 출력한다. 커밋 ID를 확인할 수 있다.
```bash
git log
```
-p 옵션을 이용하면 소스코드가 어떻게 변했는지 비교하여 보여준다.
```bash
git log -p
```

### git diff
마지막 커밋과 현재 수정한 코드를 비교해준다.
```bash
git diff
```
두 커밋의 소스 상의 차이를 보여준다.
```bash
git diff <커밋ID 1>..<커밋ID 2>
```

### git reset
버전 id로 돌아간다.
```bash
git reset --hard <버전 id">
```
cf) 원격 저장소가 아닌 본인 PC 버전에 대해서만 reset을 진행해야한다.

### git revrt
버전 id의 커밋을 취소한 내용을 새로운 버전으로 만드는 명령

```bash
git revert <버전 id>
```
## Git 명령어 사용 빈도
|command|google results|%|
|:---|---:|---:|
**|commit|528,000|7.981980075|**
|push|523,000	|7.906393143|
|pull|506,000|7.649397572|
|clone|489,000|7.392402002|
|checkout|470,000|7.105171658|
**|add|446,000|6.742354382|**
|branch|439,000|6.636532676|
**|log|388,000|5.865545964|**
**|diff|369,000|5.578315621|**
|fetch|355,000|5.36667221|
|merge|354,000|5.351554823|
**|init|343,000|5.185263572|**
**|status|286,000|4.323572541|**
**|reset|267,000|4.036342197|**
|tag|246,000|3.718877081|
|rebase|203,000|3.068829461|
|rm|142,000|2.146668884|
|show|104,000|1.572208197|
|bisect|62,800|0.9493718726|
|grep|49,400|0.7467988934|
|mv|44,700|0.6757471768|
