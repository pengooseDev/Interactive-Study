# Git 관리

---

### [레퍼런스](https://github.com/woowacourse/woowacourse-docs/tree/main/precourse)


---

### 1. 프로젝트를 자신의 계정으로 fork하기

> 저장소에 쓰기 권한이 없기 때문에 구현한 코드를 추가할 수 없습니다.
> fork는 저장소를 자신의 계정으로 복사하는 기능입니다.  
> 앞으로 모든 미션은 같은 방식으로 자신의 계정 아래에 있는 저장소를 활용해 진행해주세요.

- 이미지와 같이 저장소 우측 상단의 fork 버튼을 클릭해 fork합니다.

- fork를 완료한 후의 저장소 상태는 아래와 같습니다.

---

### 2. fork한 저장소를 자신의 컴퓨터로 clone하기

> fork한 저장소는 github.com에 존재하기 때문에 소스 코드를 추가하고, 수정하는 작업을 할 수 없습니다.
>
> clone 명령은 github.com에 존재하는 이 저장소를 자신의 노트북 또는 PC로 복사하는 과정입니다.

- 터미널에서 다음 명령을 입력합니다.

```
git clone https://github.com/{본인_아이디}/{저장소이름}
ex) git clone https://github.com/myID/Interactive-Study
```

```
// clone한 폴더로 이동하는 방법
cd {저장소 아이디}
ex) cd Interactive-Study
```

- clone을 완료한 후의 저장소 상태는 아래와 같습니다.

---

### 3. 기능 구현을 위한 브랜치 생성

> git은 서로 다른 작업을 하기 위한 별도의 공간을 만들기 위해 브랜치를 생성할 수 있습니다.

- 터미널에서 다음 명령을 입력해 브랜치를 생성합니다.

```
git checkout -b {본인 아이디}
ex) git checkout -b myID
```

- 브랜치를 생성한 후의 상태는 다음과 같다.

---

### 4. 통합 개발 환경(IDE)으로 가져오기

> 코드 작성을 위해 clone한 저장소를 자신이 사용하고 있는 통합 개발 환경(IDE)으로 가져옵니다.

> 자신이 사용하는 도구를 사용해서 진행해주세요. 이 문서에서는 Visual Studio Code를 기준으로 설명합니다.

- Visual Studio Code를 시작
- Open Project

- 앞에서 clone한 폴더를 선택합니다.

---

### 5. 기능 구현

> 요구사항을 파악해 새로운 기능을 구현하거나 코드를 수정합니다.

---

### 6. 기능 구현 후 add, commit

> 기능 구현을 완료한 후 로컬 저장소에 변경된 부분을 반영하기 위해 add, commit 명령을 사용합니다.

```
git status // 변경된 파일 확인
git add -A(또는 .) // 변경된 전체 파일을 한번에 반영
git commit -m "메시지" // 작업한 내용을 메시지에 기록
```

- 커밋 메시지를 작성하는 과정에서, commit convention을 준수합니다.

---

### 7. 본인 원격 저장소에 올리기

> 로컬에서 commit 명령을 실행하면 로컬 저장소에만 반영되고, 원격 github.com의 저장소에는 반영되지 않습니다.  
> github.com의 저장소에도 동일하게 반영하기 위해 push 명령어를 사용합니다.

```
git push origin 브랜치이름
ex) git push origin myID
```

---

### 8. github 서비스에서 Pull Request를 보낸다.

> Pull Request는 github에서 제공하는 기능으로 코드리뷰 요청을 보낼 때 사용합니다.
>
> Pull Request는 original 저장소의 main 브랜치와 앞 단계에서 생성한 브랜치 이름(앞 단계의 예에서는 myID)을 기준으로 합니다.

```
ex) 미션을 진행한 myID/Interactive-Study myID 브랜치 => pengooseDev/Interactive-Study main
브랜치로 Pull Request를 보낸다.
```

- 브라우저에서 github 저장소에 접근
- 브랜치를 작업 브랜치로 변경(앞 단계의 예에서는 javajigi)
- 브랜치 오른쪽에 있는 **"New pull request"** 버튼 클릭

- 현재 미션에서 작업한 내용을 입력하고 **"Create pull request"** 버튼을 클릭해 Pull Request를 보내주세요.

---
