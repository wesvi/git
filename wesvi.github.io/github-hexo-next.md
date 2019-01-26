---
title: GitHub Hexo Next搭建博客
date: 2019-01-26 20:12:41
tags: [ github, hexo, next]
---
## GitHub账号注册
GitHub上新建一个仓库，命名为user.github.io
## Git安装使用
``` bash
git --version
```
### 配置个人信息
``` bash
git config --global user.name "yourname"
git config --global user.email "youremail@example.com"
```
### 生成SSH公钥
``` bash
ssh-keygen -t rsa -C "youremail@example.com"
```
测试
``` bash
ssh -T git@github.com
```
## Node.js安装配置
使用管理员权限打开命令行工具并且cd到node安装包的项目文件夹，执行下面代码：
``` bash
msiexec  /i node-v11.8.0-x86.msi
```
``` bash
node -v
npm -v
```
## Hexo安装使用
### 下载安装
``` bash
npm install hexo-cli -g
npm install hexo --save
```
``` bash
hexo -v
```
### 初始化
项目目录
``` bash
hexo init
```
安装依赖
``` bash
npm install
```
### 常用命令
``` bash
hexo clean
hexo g
hexo s
hexo d
```
### 推送配置
``` bash
deploy:
  type: git
  repo: git@github.com:yourname/yourname.github.io.git
  branch: master
```
## Next主题设置

*** 参考: *** [Hexo+Pages静态博客-Next主题篇](https://blog.csdn.net/mango_haoming/article/details/78207534/)
