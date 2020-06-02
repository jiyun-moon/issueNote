## vscode 자동 저장으로 lint 오류 뜰 때
settings.json 파일에서
`"editor.formatOnSave": false,`

부분을 true > false 로수정 하니 자동 저장은 꺼짐.
이 설정을 왜 기본으로 잡아줬는지는 모르겠다..


**2020.06.02 추가
Prettier eslint 와 Eslint 익스텐션 설치 후 해결.
https://marketplace.visualstudio.com/items?itemName=rvest.vs-code-prettier-eslint
