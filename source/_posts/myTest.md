---
title: myTest
date: 2018-12-26 09:38:39
tags:
---
###搭建个人博客-hexo+github详细完整步骤
### 
1.安装git与配置
    http://git-scm.com/
  (1) 安装过程：
    Adjusting your PATH environment(选择项中)
    Use Git from the Command Prompt,其他一路next
  (2) config：用git config配置 Git，要做的第一件事就是设置名字和邮箱地址：：
```base
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

2.安装NodeJs
  (1) https://nodejs.org/en/
  (2) 安装步骤：一路默认就行（安装路径根据自己需要更改）
3.安装Hexo 
  (1) 利用 npm 命令即可安装。在任意位置点击鼠标右键，选择Git Bash
```
$ npm install -g hexo
```
 (2)在_config.yml,进行基础配置
 title:可修改为自己的标题
 https://hexo.io/themes/ 可以在这里浏览更多主题，然后在Hexo文件夹下 Git Bash

4. 初始化hexo
```
$ hexo init      
```
 (1) 写文章:在D:\Hexo\source\_posts文件下，新建.md文件就可以写文章
```
$ npm install    #install before start blogging
$ hexo generate       #自动根据当前目录下文件,生成静态网页
$ hexo server         #运行本地服务
在浏览器输入：localhost：4000 ，就可以进行访问
```
5.部署到Github上
1、申请Github账号，（注意别忘了进行账号邮箱验证）
2.new repository
 #first:
 Owner:hanmiaomiao123 /Repository name:hanmiaomiao123.github.io
 #second:
 create repository
3. #在_config.yml进行配置
  deploy:
    type: git     #space before the adrress
    repo: https://github.com/hanmiaomiao123/hanmiaomiao123.gitHub.io   #space before the adrress
4. 安装hexo-deployer-git自动部署发布工具
```
 $ npm install hexo-deployer-git  --save
```
5. 发布到Github
```
hexo clean && hexo g && hexo d
```
第一次发布需要验证github账号(username,password)   
直到出现Info Deploy done:git  # 表示发布完成
6. 测试访问
浏览器输入https://hanmiaomiao123/hanmiaomiao123.github.io/

