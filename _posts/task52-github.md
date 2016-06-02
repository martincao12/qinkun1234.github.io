

问题的提出:在完成了[带用户功能的任务管理系统](http://laravelacademy.org/post/3297.html#comments)之后追加[github登录功能](http://laravelacademy.org/post/1305.html)。


### 1、用户表追加了两个字段

[2016_06_01_070231_add_github_id_avatar_to_users](https://github.com/jnuc093/study_quickstart-intermediate/blob/master/database/migrations/2016_06_01_070231_add_github_id_avatar_to_users.php)
	
	php artisan migrate	

### 2、路由定义

	
	php artisan make:controller SocialAuthController

在routes.php中添加:

	Route::get('auth/github', 'SocialAuthController@redirectToProvider');
	Route::get('auth/github/callback', 'SocialAuthController@handleProviderCallback');
	
### 3、在resources/views/auth/login.blade.php登录按钮下添加:

	<a class="btn btn-link" href="auth/github">GitHub Login</a> 
	
### 4、按照[github登录功能](http://laravelacademy.org/post/1305.html)设置自己的相应配置	




