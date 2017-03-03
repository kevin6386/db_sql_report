# db_sql_report
数据库通用SQL汇报程序
1、创建库

create database system;


2、创建表

CREATE TABLE `db_list_sql` (
  `id` int(10) unsigned NOT NULL AUTO_INCREMENT,
  `type` varchar(255) DEFAULT NULL,
  `sql` text,
  `ip` varchar(255) DEFAULT NULL,
  `result` varchar(255) DEFAULT NULL,
  `num` int(11) NOT NULL DEFAULT '1',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1161970 DEFAULT CHARSET=utf8;

3、程序自行修改用户及密码

4、为了保证SQL的真实性，会开启general_log，或一定时间的sql进行汇报到表中，当作样例存储。
