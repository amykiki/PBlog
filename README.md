# PBlog (测试端口地址:http://115.29.112.160:8011/)
Version: 0.1.0-SNAPSHOT | 更新: 05/03 2016

[![Build Status](https://travis-ci.org/penglongli/PBlog.svg?branch=master)](https://travis-ci.org/penglongli/PBlog) [![Coverage Status](https://coveralls.io/repos/github/penglongli/PBlog/badge.svg?branch=master)](https://coveralls.io/github/penglongli/PBlog?branch=master)

[**简介**](#简介) | 
[**安装使用**](#安装使用) | 
[**项目构建**](#项目构建) |  [**版权**](#版权)
 
---

## 简介
PBlog是一款使用Java开发的单页应用blog，目的是为了作为学习交流使用。当然，你也可以将其作为个人博客网站使用，在使用的过程中如果遇到什么问题，
有好的想法或者建议，可以一起互相交流。

### 使用到的开源项目:
- [Spring Framework](http://spring.io/) famework
- [MyBatis](http://www.mybatis.org/mybatis-3/) persistence framework
- [jQuery](http://jquery.com) 
- [Less](http://lesscss.org/)
- [Font Awesome](http://www.bootcss.com/p/font-awesome/)
- [AngularJS](https://angularjs.org/)
- [angular-loading-bar.js](https://github.com/chieffancypants/angular-loading-bar)
- [marked.js](https://github.com/chjj/marked)
- [highlight.js](https://highlightjs.org/)
- [gulp](http://gulpjs.com/)

### 项目目录结构
```
├── dbmigrate/  数据库修改记录
└── src/
    └── main/ 
      └── java/com/pblog 源代码
        └── core
          ├── orm/ MyBatis分页对象
          ├── utis/ 
        └── dao/
        └── domain/
        └── service/
        └── web/ 
          └── controller/
          └── interceptor/
            ├── GlobalInterceptor.java  Spring拦截器:获得用户IP等信息
            ├── PaginationInterceptor.java MyBatis拦截器: 重构sql语句, 实现分页
      └── resources 源配置 
      └── webapp/ 
        └── WEB-INF/ 
          ├── jsp/  视图
        └── resources/
          ├── assets/  gulp自动化构建后生成的资源文件
          ├── js/  
          ├── less/
    ├── test/ 单元测试
├── travis.yml travis-ci配置
├── deploy.sh 部署脚本(个人部署需重写)
├── gulpfile.js gulp自动化构建脚本
├── pblog.sql PBlog初始化sql
├── pom.xml 项目依赖

```
## 安装使用

## 项目构建

## 版权
This project is open-sourced under [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)


