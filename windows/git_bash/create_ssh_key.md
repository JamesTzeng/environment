### 生成 SSH 公開金鑰

[参考文档](https://git-scm.com/book/zh-tw/v1/%E4%BC%BA%E6%9C%8D%E5%99%A8%E4%B8%8A%E7%9A%84-Git-%E7%94%9F%E6%88%90-SSH-%E5%85%AC%E9%96%8B%E9%87%91%E9%91%B0)

```
$ cd ~/.ssh
$ ls
$ ssh-keygen
$ cat ~/.ssh/id_rsa.pub
```

push repository 到 github 时，默认使用 ~/.ssh/id_rsa key，如果要指定不同的 key，要建立 ~/.ssh/[config](config) 文档
```
Host github.com
  IdentityFile ~/.ssh/github_rsa
```

[指定 rsa key](http://stackoverflow.com/questions/4565700/specify-private-ssh-key-to-use-when-executing-shell-command-with-or-without-ruby)
