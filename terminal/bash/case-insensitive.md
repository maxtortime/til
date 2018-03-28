가끔 SSH로 터미널에 접속하면 디렉토리를 자동완성해서 찾아가려고 할 때 쉘에서 대소문자를 엄격하게 구분해서 불편할 때가 있다.

이럴 때는,
1. `/etc/inputrc` 를 텍스트 에디터로 연다.
2. 적당한 곳에 `set completion-ignore-case on` 를 넣어준다.
3. `exit`를 하든 터미널을 다시 켜든 해서 재접속한다.
4. 성공!

우분투에서는 잘 됐는데 맥이나 다른 배포판에서도 되는 지는 해보지 않았음.

https://superuser.com/questions/90196/case-insensitive-tab-completion-in-bash
