---
layout:     post
title:      Postgresql 설치
date:       2016-12-06 00:36:00
summary:    EC2 Container 에 PostgreSql 설치 및 계정 생성
categories: mtrlmd
---


* sudo yum install postgresql
* postgresql 을 yum으로 설치하면 자동으로 postgre 계정 생성됨
* postgre 계정 패스워드 부여 및 로그인
* -bash-4.2$ initdb
* -bash-4.2$ pg_ctl start
* postgres=# Create database playdb;
* postgres=# select * from pg_database;

{{ site.url }}/images/postgre_database_creation.PNG



* postgres=# create user playuser password 'playuser' login;

{{ site.url }}/images/postgre_user_creation.PNG
