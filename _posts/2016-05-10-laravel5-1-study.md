---
layout: single
title: Laravel5.1 study
---

## a 文档资料

[官方文档](https://laravel.com/docs/5.1)

[laravel学院 发行版本说明 差异对比](http://laravelacademy.org/post/9.html)

新建指定版本项目:

	composer create-project laravel/laravel blog "5.1.*"

[laravel.com 5.1](https://laravel.com/docs/5.1/seeding)

[laravelbook Migrations](http://laravelbook.com/laravel-migrations-managing-databases/)

### 环境设置

	subl 	~/.homestead-56/Homestead.yaml

## 常用操作

	php artisan migrate
	php artisan db:seed
	composer install
	composer update

	php artisan vendor:publish			生成配置文件

####  [sitepoint migrations](http://www.sitepoint.com/laravel-migrations/)

## laravel5.1



#### ryanchenkie

ONE [Token-Based Authentication for AngularJS and Laravel Apps ](https://scotch.io/tutorials/token-based-authentication-for-angularjs-and-laravel-apps) 5.1

TWO Authenticated User Route [Token-Based Authentication for AngularJS and Laravel Apps](http://ryanchenkie.com/token-based-authentication-for-angularjs-and-laravel-apps/)

#### huanghua581

[dingo-api-demo](https://github.com/huanghua581/dingo-api-demo)

jwt-auth 、短信

github中搜 dingo

### Laravel-5-Bootstrap-3-Starter-Site
[Laravel-5-Bootstrap-3-Starter-Site](https://github.com/mrakodol/Laravel-5-Bootstrap-3-Starter-Site/issues/205)

项目启动的步骤:

	$ composer dump-autoload
	$ composer install --no-scripts
	$ npm install --save-dev
	$ gulp
	$ php artisan migrate
	$ php artisan db:seed
	$ php artisan key:generate			//重要
	👍 3  
	

## laravel学院

### 基础教程

[使用Laravel内置组件快速实现注册登录](http://laravelacademy.org/post/1258.html)

[auth/register](http://task51.dev/auth/register)

[add-new-column-migrate-to-database](http://stackoverflow.com/questions/16791613/add-new-column-migrate-to-database)


已实现

[SMTP驱动实现邮件发送（含附件和图片）](http://laravelacademy.org/post/1986.html)

[github登录  auth/github](http://laravelacademy.org/post/1305.html)

[微信开放平台网页登录 未有视频]()

[手机短信]()


### 扩展包
	
[JWT实现基于API的用户认证](http://laravelacademy.org/post/3640.html) 

	middle jwt.auth
	
### email

	composer require "guzzlehttp/guzzle=~5.0"	
		
## jeerf
[auth](https://laracasts.com/series/laravel-5-fundamentals/episodes/15)

[auth 5.1.4](https://laraveltips.wordpress.com/2015/06/15/how-to-make-user-login-and-registration-laravel-5-1/)

重要  traits [laraveltips 注册与登录](https://laraveltips.wordpress.com/2015/06/15/how-to-make-user-login-and-registration-laravel-5-1/?blogsub=confirming#subscribe-blog)

## laravel视频

[基础教程](https://laravist.com/series/laravel-5-basic)

[稍微深入](https://laravist.com/series/dive-a-little-deep-into-laravel-5)

## laravel学院