public:: true
经过一番折腾，距离我的基于 Logseq 的网页发布前所未有的近，在此总结一下遇到的问题：

- 已解决的：
- - action 中 deploy 时问题：本质上是 deploy 问题，secret.ACCESS_TOKEN 实际上就是一个可替换的字符，权限是 secret ，自动替换为自己生成的 personal access token
-
- 未解决的：
- - 主页似乎没有正常显示
-