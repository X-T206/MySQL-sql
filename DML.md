# 一、添加数据（INSERT)
    1.给指定字段添加数据
    INSERT INTO 表名(字段名1，字段名2……) VALUES(值1,值2……);
    2.给全部字段添加数据
    INSERT INTO 表名 VALUES(值1,值2);
DataGrip中查看更新的数据可直接点击查看/select * 表名;

    3.批量添加数据
    INSERT INTO 表名（字段名1，字段名2，……），（值1，值2，……），（值1，值2，……）;
    INSERT INTO 表名 VALUES(值1，值2，……),(值1，值2，……);
!插入数据时，指定的字段顺序需与值顺序一一对应
 字符串和日期型数据应包含在引号中
 插入的数据大小，应该在字段的规定范围之内

# 二、修改数据（UPDATE）
    1.UPDATE 表名 SET 字段名1=值1,字段名2=值2,……[WHERE条件];
      UPDATE 表名 SET 字段名=值; 
      !不添加where条件默认修改整表该字段全部信息
# 三、删除数据（DELETE)
    1.DELETE FROM 表名[where条件];
    !DELETE语句的条件可以有，也可以没有。没有默认删除整张表的所有数据。
    DELETE语句不能删除某个字段的值（可以使用UPDATE)
