##### 1.查询所有数据库：show DATABASES;
##### 2.查询当前所有数据库：SELECT DATABASES();
##### 3.数据库创建
      CREATE DATABASES 数据库名;
    3.1删除数据库：DROP DATABASE[IF EXISTS] 数据库名;
    3.2查询当前所在数据库所有表：SHOW TABLES;
        查看表结构： DESC 表名;
        查建表语句： SHOW CREATE TABLE 表名;
    3.3 使用：
            USE 数据库名                                

    3.4建表：
            CREATE TABLE 表名(                           
            字段1  字段1类型 [注释];
            字段2  字段2类型 [注释];
            ……
            )[COMMENT 表注释];                              例：CREATE TABLE tb_user(
                                                              id tinyint unsigned comment '编号';
                                                              name varchar(50) comment '姓名';
                                                              age int comment '年龄';
                                                              gender varchar(1) comment '性别'
                                                              )comment '用户表';
##### 4.表修改：
          添加字段：    alter table 表名 add 字段名 类型（长度）
          修改数据类型： alter table 表名 modify 字段名  新数据类型（长度）
          修改字段名和字段类型： alter table 表名 change 旧字段名 新字段名 类型（长度） [comment];

          4.2删除
          删字段：ALTER TABLE 表名 DROP 字段名;
          删表:DROP TABLE [IF EXISTS]表名;
          删指定表并创新:TRUNCATE TABLE 表名

          4.3修改表名
          ALTER TABLE 表名 RENAME TO 新表名;
