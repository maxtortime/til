sierra 업데이트 후 터미널에서 자꾸 `xcrun: error: invalid active developer path ~~` 이런 에러가 뜰 경우 당황하지 말고,

```sh
$ sudo chown -R $(whoami) /usr/local
$ xcode-select --install
```

로 차분하게 설치해주자..
나중에 homebrew에서 소유권을 다시 root한테 넘겨주라면 그렇게 하면 된다..
