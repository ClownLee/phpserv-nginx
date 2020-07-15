# PHP Dockerfile
Dockerfile for php & nginx. php 容器 和 nginx 容器，php-fpm 处理PHP代码，nginx 处理纯前端和静态资源，实现前后端分离。 php 容器中 安装有（bcmath, Core, ctype, curl, date, dom, fileinfo, filter, ftp, gd, hash, iconv, json, libxml, mbstring, mcrypt, mongodb, mysqlnd, openssl, pcre, PDO, pdo_mysql, pdo_sqlite, Phar, posix, readline, redis, Reflection, session, SimpleXML, soap, sockets, sodium, SPL, sqlite3, standard, swoole, tokenizer, xml, xmlreader, xmlwriter, xsl, zip, zlib）等常用扩展。
## 目录结构
![avatar](http://chuantu.xyz/t6/739/1594804713x992249049.png)
### Project 2:
- [hub.docker.com](https://hub.docker.com/r/clownlee/phpserv-nginx) 上的镜像 `docker pull clownlee/phpserv-nginx`
- change-nginx 容器的 web 项目目录 `/www/pro/public`（web 项目目录 可在 `/phpserv-nginx/init/pro.conf` 配置文件中修改） 用于部署静态资源纯前端代码等
- change-php 容器的 web 项目目录 `/www/pro/public`（web 项目目录 可在 `/phpserv-nginx/init/pro.conf` 配置文件中修改） 基于 laravel 和 thinkphp 框架入口目录设计
