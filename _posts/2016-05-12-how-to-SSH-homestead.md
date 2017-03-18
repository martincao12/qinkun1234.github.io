---
layout: single
title: how to SSH homestead
---

## how to ssh homestead


 一般情况下我们是如此登录到虚拟机的:

	➜  Homestead git:(v3.1.0) ✗ pwd
	/Users/qk/Homestead
	➜  Homestead git:(v3.1.0) ✗ vagrant ssh
	Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-25-	generic x86_64)


但是更直观的方法是如下(任意目录):

	ssh homestead
	Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-25-generic x86_64)

下面介绍下设置操作步骤:

#### 1 在（本机）生成秘钥和公钥

	ssh-keygen -t rsa -C "vagrant"

	按照提示指定文件，我指定为~/.ssh/id_rsa_homestead

	分别生成了公钥文件id_rsa_homestead.pub
	和秘钥文件id_rsa_homestead

#### 2 （本机）指定登录到vagrant虚拟机的参数(包括私钥匙文件..)

	vi ~/.ssh/config

内容如下:

	Host homestead
  		IdentityFile ~/.ssh/id_rsa_homestead
	HostName 127.0.0.1
	User vagrant
	Port 2222		


#### 3 (vagrant虚拟机)上将公钥文件中的内容拷贝到服务器的authorized_keys文件中:

	.ssh pwd
	/home/vagrant/.ssh
	.ssh ls -l
	total 20
	-rw------- 1 vagrant vagrant  389 Dec 19 13:09 authorized_keys

参考:

[Getting Started with Laravel Homestead](https://scotch.io/tutorials/getting-started-with-laravel-homestead)

[ssh gist](https://gist.github.com/jexchan/2351996)

[digital ocean](https://www.digitalocean.com/community/tutorials/how-to-configure-custom-connection-options-for-your-ssh-client)
