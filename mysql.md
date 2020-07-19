# MySQL 笔记

> 客户端工具 Navicat vs DataGrip vs TablePlus

## 基本命令

```sql
mysql -uroot -p123456   -- 连接数据库

update mysql.user set authentication_string=password('123456') where user='root' and Host='localhost'; -- 修改用户密码
flush privileges;  -- 刷新权限
```

```sql
show databases;  -- 查看所有的数据库

use school  -- 切换数据库

show tables;  -- 查看数据库中所有表
describe student;  -- 查看student表的设计信息

create database westos; -- 创建一个数据库

exit;  -- 退出连接

-- 单行注释 (SQL 原始注释)
/*  (sql 多行注释)
*/ 
```

DDL 定义
DML 操作
DQL 查询
DCL 操作

## 数据库操作语句

操作数据库 -> 操作数据库中的表 -> 操作数据库中表的数据

### 操作数据库

#### 创建数据库

```sql
CREATE DATABASE [IF NOT EXISTS] westos
DEFAULT CHARACTER SET utf8mb4
DEFAULT COLLATE utf8mb4_unicode_ci;
```

#### 删除数据库

```sql
DROP DATABASE [IF EXISTS] westos;
```

#### 使用数据库

```sql
USE `swstor`;
```

### 查看数据库

```SQL
SHOW DATABASE;  -- 查看所有数据库
```

## 数据库的列类型

> 数值

- tinyint     1个字节
- 

> 字符串

> 时间日期

> null



---

```sql
SET NAMES UTF8;
```