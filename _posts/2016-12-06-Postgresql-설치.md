* sudo yum install postgresql
* postgresql 을 yum으로 설치하면 자동으로 postgre 계정 생성됨
* postgre 계정 패스워드 부여 및 로그인
* -bash-4.2$ initdb
* -bash-4.2$ pg_ctl start
* postgres=# Create database playdb;
* postgres=# select * from pg_database;


datname  | datdba | encoding | datcollate  |  datctype   | datistemplate | datallowconn | datconnlimit | datlastsysoid | datfrozenxid | dattablespace |               datacl
-----------+--------+----------+-------------+-------------+---------------+--------------+--------------+---------------+--------------+---------------+-------------------------------------
template1 |     10 |        6 | en_US.UTF-8 | en_US.UTF-8 | t             | t            |           -1 |         12918 |         1877 |          1663 | {=c/postgres,postgres=CTc/postgres}
template0 |     10 |        6 | en_US.UTF-8 | en_US.UTF-8 | t             | f            |           -1 |         12918 |         1877 |          1663 | {=c/postgres,postgres=CTc/postgres}
postgres  |     10 |        6 | en_US.UTF-8 | en_US.UTF-8 | f             | t            |           -1 |         12918 |         1877 |          1663 |
playdb    |     10 |        6 | en_US.UTF-8 | en_US.UTF-8 | f             | t            |           -1 |         12918 |         1877 |          1663 |
(4 rows)


* postgres=# create user playuser password 'playuser' login;

{{ site.url }}/images/postgre_user_creation.PNG
