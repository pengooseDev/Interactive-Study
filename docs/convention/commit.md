# Commit Convention

[커밋 컨벤션](https://aroundlena.tistory.com/55)

### 커밋 컨벤션

> git commit -m "feat: Scroll Handler 추가"

커밋 메시지는 크게 세 부분으로 분류 됩니다.

- type: Subject
- body
- footer

##### 1. Type 기술

- feat: 새로운 기능 추가
- fix: 버그 수정
- docs: 문서 수정
- style: 포맷팅, 세미콜론 빠졌을때, 코드 변경이 없는 수정
- refactor: 리팩토링
- test: 테스트 코드 추가, 테스트코드 리팩토링
- chore: 빌드관련 수정, 패키지 매니저 수정change

##### 2. Subject 기술

- Type을 기술한 뒤에, 해당 커밋에서 어떤 작업을 했는지 직관적으로 알아볼 수 있는 Subject를 작성합니다. 콜론 뒤에 띄어쓰기를 한 번 한 뒤에 작성하도록 합니다.
- 마침표를 작성하지 않습니다.

##### 3. body(optional)

위의 Type: Subject에서 모든 내용을 담아내지 못하고 부연 설명이 필요한 경우 작성하도록 합니다.

##### 4. The Footer(optional)

- footer 또한 필수가 아닙니다. issue tracker ID의 reference를 남길 때 사용합니다.

##### Example Commit Message

```
feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```
