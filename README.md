# oneinstack-nginx-drupal8-vhost-config
English tutorial:

This is the [oneinstack](https://oneinstack.com/) nginx vhost config for drupal8

<b>The config is very easy, Just modify the only file of the vhost/*.conf</b>

When Use oninstack(nginx+php) for drupal8, We will come a lot of errors
Such as 

	

1.  update.php error
	

2.  An AJAX HTTP error occurred.  
           HTTP Result Code: 403  
           Debugging information follows.  
           Path: /core/authorize.php/core/authorize.php?batch=1&id=2&op=do_nojs&op=do


3.  and so on...

*Special remind:*
The error of ftp permission when install module is not the problem of nginx ,It cause that the user and group of nginx/php/mysql is not the same.

Because the oneinstack is not just for drupal8,So the author of oneinstack won't write the special config for it,So we should modify it forourselves.

----------
**中文教程：**

这是对[oneinstack](https://oneinstack.com/)（nginx+php）的vhost配置文件的修改，从而完美运行drupal8

<b>修改配置非常简单，你仅仅需要修改一个东西：域名对应的vhost配置文件 /vhost/*.config</b>



深入了解：

用了这个配置文件，你讲解决以下问题

1.  update.php 错误
	

2.  An AJAX HTTP error occurred.  
           HTTP Result Code: 403  ****
           Debugging information follows.  
           Path: /core/authorize.php/core/authorize.php?batch=1&id=2&op=do_nojs&op=do


3.  and so on...

*特别提醒*：安装模块时出现的ftp permission错误与nginx的配置无关，是由于你的nginx/php/mysql的用户和用户组不一致导致的，百度搜索方案将其改为一致即可解决

因为Oneinstack不是专门为drupal而写的，所以不可能将drupal的所有配置都考虑到，故我们要自己手动去修改
本项目将持续更新，为drupal开发者免去配置的烦恼
