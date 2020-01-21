# warning: LF will be replaced by CRLF 해결하기

git init 을 한 후 README.md 를 만들고 commit 을 하는데 난생 처음보는 메시지가 떴다.

```
warning: LF will be replaced by CRLF in README.md.
The file will have its original line endings in your working directory
```

이 에러는 유닉스 계열에서는 한 줄 끝이 LF(Line Feed)로 이루어지는데 윈도우에서는 한 줄이 CR(Carriage Return)과 LF(Line Feed)로 이루어지기 때문에 Git이 갸우뚱하고 있는 상황이다. 하지만 git 은 이를 해결할 계획이 있었다. `core.autocrlf` 기능을 통해 상황에 맞게 변환을 해줄 수 있다. 이 기능을 켜기만 하면 된다.

```
git config --global core.autocrlf true
```

