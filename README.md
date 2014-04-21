# 基于Rails的管理系统模板

----

## 一. 介绍

>    Rails可以通过几个命令帮助我们快速搭建一个框架. 但是里面缺少样式, 用户登录,权限认证等框架, 每次一个一个去添加gem,进行配置,多少也会消耗一些时间. admin-templates是这样一个管理系统框架, 它里面已经包含了用户登录,管理, 权限认证等功能, 并且通过bootstrap框架进行样式管理. 我们只需要几个命令就可以搭建一个管理系统的雏形, 剩下的可以通过rails自带的scaffold创建带有bootstrap风格的resources, 可以减少70%的编码工作量.


## 二. 运行环境
1. ruby 1.9.3 or later
2. rails 3.2.15 or later


## 三. 使用步骤
1. git clone https://github.com/siye1982/admin-templates.git
2. bundle install
3. 默认数据库是sqlite3, 可以根据需要变更数据库
4. rails g scaffold Item title:string description:text --skip-stylesheets  用脚手架添加资源,Item是你的自定义资源
5. rails g bootstrap:themed items -f  给item资源加样式
