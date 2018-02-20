![图片](http://image.sdingo.cn/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20180220205649.png)
### laravel web简单入门开发案例

--------
这是一个laravel 5.5 简单案例 是基于 laravel china 社区的 [laravel 教程 - Web 开发实战入门](https://laravel-china.org/courses/laravel-essential-training-5.5)
所制作完成的

### 基本功能

--------
* 登录注册
* 邮件激活用户、邮件重置密码
* 个人中心
* 用户列表
* 粉丝功能
* 文章发布

### 安装

--------
1.克隆代码
```git
   git clone https://github.com/shixiaoding/laravel-weibo.git
```

2.设置配置
```shell
    cp .env.example .env 
```

3.安装扩展包
安装`laravel`扩展
```shell
    composer install
```
安装前端扩展
```shell
    yarn install
```

4.生成key
```shell
    php artisan key:generate
```

5.创建表并填充数据
在`.env`配置文件中，有关database相关配置修改为系统设置
```shell
    php artisan migrate --seed
```

6.配置邮件相关配置
在`.env`配置文件中
```php
MAIL_DRIVER=smtp
MAIL_HOST=smtp.163.com
MAIL_PORT=465
MAIL_USERNAME=你的邮箱地址
MAIL_PASSWORD=邮箱授权码
MAIL_ENCRYPTION=ssl
MAIL_FROM_ADDRESS=你的邮箱地址
MAIL_FROM_NAME=你的邮箱用户名
```

### 谢谢

--------
* [Summer](https://laravel-china.org/users/1)
* [Laravel - 中国](https://laravel-china.org/)




