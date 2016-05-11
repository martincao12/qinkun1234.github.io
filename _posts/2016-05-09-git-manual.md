---
layout: single
title: Git manual
---

### [Multiple SSH Keys settings for different github account](https://gist.github.com/jexchan/2351996)

	git clone git@qinkun1234.github.com:qinkun1234/qinkun1234.github.io.git

#### git pms 项目常用命令

	git update-index --assume-unchanged src/g4server.properties //忽略某一文件更新
	git update-index --assume-unchanged src/jdbc.properties     //忽略数据库配置文件变化
	git update-index --no-assume-unchanged src/g4server.properties
	git status
	git pull
	git add .
	git commit -m "ce shi"
	git push

	git stash     //暂存
	git stash list

	10-忽略跟踪 .idea目录
	在.gitignore中加入: .idea/

	11-删除已经存在git跟踪的 .idea目录
	git rm -r --cached .idea
