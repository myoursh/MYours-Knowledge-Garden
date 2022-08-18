- 教程详见 https://imap.vercel.app/#/page/logseq%E9%83%A8%E7%BD%B2%E7%BD%91%E9%A1%B5
- 以下为个人记录
	- 配置文件
	  collapsed:: true
		- config.edn
	- 主题修改
	  collapsed:: true
		- custom.css
	- git
	  collapsed:: true
		- hookes
			- post-commit
	- 主库动作 action
	  collapsed:: true
		- 每次 commit 时都会自动运行该脚本
		- CI 就是该脚本名（存疑，还没很懂）
	- 评论区配置
		-
	- 发布时 cdn 加速
	  collapsed:: true
		- 文件网址位置：htps:/cdn.jsdelivr..net/gh/你的用户名/你的仓库名@发布的版本号/文件路径
		- 详见 config.edn ，搜索 css
	- 自动发布流程：
	  collapsed:: true
		- 源代码库→发布库→ Vercel 拉取发布库的 main 分支并部署
-
-