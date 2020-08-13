## 로컬에서 gitignore 시키는 방법

`git update-index --assume-unchanged 삭제하려는 파일명`

unchanged 로 지정된 파일을 보려면?

`git ls-files -v | grep ^h` 실행


** 추가
`fatal: Unable to mark file`
fatal 에러가 나는 경우,

1. `git reset HEAD` 를 해주면 M 뒤에 리스트가 막 있다. 스테이지에 올라가지 않은 변경 사항을 리셋해주는 명령어 같다.
그중에 원하는 파일명을 복사해서
2. `git update-index --assume-unchanged index.php`
다시ignore 명령을 넣어주면 끝.

<예시>

`Unstaged changes after reset:`

`M   index.php`

`git update-index --assume-unchanged index.php`


/* 변경이 잦을 떄 */
.gitconfig
[alias]
    hide = update-index --assume-unchanged
    unhide = update-index --no-assume-unchanged
