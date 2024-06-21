#### Week 11

1. PL/SQL 程序的哪部分用于处理异常？
    - a) 声明部分
    - b) 可执行部分
    - c) 异常处理部分
    - d) 事务处理部分

2. 如何在PL/SQL中声明变量`v_sal`，使其类型与表`emp`中的列`sal`相同？
    - a) v_sal emp.sal%TYPE;
    - b) v_sal%ROWTYPE;
    - c) v_sal%TYPE emp.sal;
    - d) v_sal ROWTYPE(emp.sal);

3. 在PL/SQL中，`SELECT INTO`语句的作用是什么？
    - a) 检索多行数据
    - b) 检索单行数据并赋值给变量
    - c) 更新表中的数据
    - d) 删除表中的数据

4. 以下哪个异常在`SELECT INTO`语句没有返回任何行时触发？
    - a) TOO_MANY_ROWS
    - b) ZERO_DIVIDE
    - c) NO_DATA_FOUND
    - d) VALUE_ERROR

5. 以下哪个内置函数用于返回最近一次捕获的异常的错误信息？
    - a) DBMS_OUTPUT.PUT_LINE
    - b) SQLCODE
    - c) SQLERRM
    - d) DBMS_UTILITY

#### Week 12

6. 在PL/SQL中，如何声明一个记录类型变量，该变量的结构与表`employees`的行结构相同？
    - a) v_emp employees%TYPE;
    - b) v_emp employees%ROWTYPE;
    - c) v_emp%ROWTYPE employees;
    - d) v_emp ROWTYPE(employees);

7. 哪个PL/SQL包用于在代码中执行DDL语句？
    - a) DBMS_OUTPUT
    - b) DBMS_JOB
    - c) DBMS_DDL
    - d) DBMS_LOB

8. 使用显式游标时，哪个步骤是必需的？
    - a) 打开游标
    - b) 提交游标
    - c) 回滚游标
    - d) 清除游标

9. 在PL/SQL中，如何捕获所有未被具体捕获的其他异常？
    - a) EXCEPTION WHEN OTHERS THEN
    - b) RAISE OTHERS
    - c) HANDLE EXCEPTION
    - d) EXCEPTION WHEN UNDEFINED THEN

10. 在PL/SQL中，如何创建一个触发器在插入行之前执行？
    - a) CREATE TRIGGER trigger_name AFTER INSERT ON table_name
    - b) CREATE TRIGGER trigger_name BEFORE INSERT ON table_name
    - c) CREATE TRIGGER trigger_name AFTER UPDATE ON table_name
    - d) CREATE TRIGGER trigger_name INSTEAD OF INSERT ON table_name

#### Week 13

11. 哪个包用于在PL/SQL代码中创建定时任务？
    - a) DBMS_OUTPUT
    - b) DBMS_JOB
    - c) DBMS_SCHEDULER
    - d) DBMS_LOCK

12. Oracle数据库中的控制文件保存什么信息？
    - a) 用户信息
    - b) 数据文件和日志文件的位置
    - c) 表结构
    - d) 索引信息

13. 表空间的主要用途是什么？
    - a) 存储用户信息
    - b) 存储数据库对象
    - c) 管理事务日志
    - d) 存储临时文件

14. 如何在PL/SQL中使用DBMS_DDL包执行DDL语句？
    - a) DBMS_DDL.EXECUTE_DDL('CREATE TABLE employees (emp_id NUMBER, emp_name VARCHAR2(50))');
    - b) DBMS_DDL.RUN_DDL('CREATE TABLE employees (emp_id NUMBER, emp_name VARCHAR2(50))');
    - c) DBMS_DDL.START_DDL('CREATE TABLE employees (emp_id NUMBER, emp_name VARCHAR2(50))');
    - d) DBMS_DDL.BEGIN_DDL('CREATE TABLE employees (emp_id NUMBER, emp_name VARCHAR2(50))');

15. 哪个命令用于将数据文件添加到表空间？
    - a) ALTER TABLESPACE ADD DATAFILE
    - b) CREATE TABLESPACE ADD DATAFILE
    - c) INSERT INTO TABLESPACE ADD DATAFILE
    - d) UPDATE TABLESPACE ADD DATAFILE

#### Week 14

16. ROWID的作用是什么？
    - a) 唯一标识数据库中的一行
    - b) 标识表的列
    - c) 标识表空间
    - d) 标识数据库

17. PCTFREE参数在创建表时的作用是什么？
    - a) 指定每个数据块中为将来更新保留的空闲空间百分比
    - b) 指定每个数据块中初始使用的空间百分比
    - c) 指定分配给段的最小范围数
    - d) 指定分配给段的最大范围数

18. 在Oracle数据库中，如何禁用某个表上的所有触发器？
    - a) ALTER TABLE table_name DISABLE ALL TRIGGERS;
    - b) DROP TRIGGER ALL ON table_name;
    - c) DISABLE TRIGGER ON table_name;
    - d) REMOVE ALL TRIGGERS FROM table_name;

19. 行链（Row Chaining）和行迁移（Row Migration）的区别是什么？
    - a) 行链是指一行数据跨多个数据块存储，行迁移是指一行数据从一个数据块移动到另一个数据块
    - b) 行链是指表的索引结构，行迁移是指表的数据结构
    - c) 行链和行迁移没有区别
    - d) 行链是指数据块中有未使用的空间，行迁移是指行的数据被移动到另一个数据块

20. 如何在Oracle中指定用户的缺省表空间和临时表空间？
    - a) CREATE USER username IDENTIFIED BY password DEFAULT TABLESPACE default_tablespace TEMPORARY TABLESPACE temp_tablespace;
    - b) ALTER USER username SET DEFAULT TABLESPACE default_tablespace TEMPORARY TABLESPACE temp_tablespace;
    - c) SET USER username DEFAULT TABLESPACE default_tablespace TEMPORARY TABLESPACE temp_tablespace;
    - d) MODIFY USER username SET TABLESPACE default_tablespace TEMPORARY TABLESPACE temp_tablespace;

#### Week 15

21. 位图索引适用于哪种列？
    - a) 唯一列
    - b) 非重复值较多的列
    - c) 重复值较多的列
    - d) 日期列

22. 如何在PL/SQL中创建基于函数的索引？
    - a) CREATE INDEX index_name ON table_name(column_name FUNCTION column_name);
    - b) CREATE FUNCTION INDEX index_name ON table_name(column_name);
    - c) CREATE INDEX index_name ON table_name(FUNCTION column_name);
    - d) CREATE INDEX index_name ON FUNCTION table_name(column_name);

23. 如何在SQL*Plus中查看SQL执行计划？
    - a) SET AUTOTRACE ON
    - b) SHOW EXECUTION PLAN
    - c) EXPLAIN PLAN FOR
    - d) TRACE EXECUTION PLAN

24. 在Oracle中，ANALYZE语句的作用是什么？
    - a) 分析表数据分布的统计数据，写入数据字典
    - b) 更新表的数据
    - c) 删除表中的数据
    - d) 创建表的索引

25. 全表扫描的一个常见原因是什么？
    - a) 表中有合适的索引
    - b) 表数据量很小
    - c) 使用了不合适的条件，例如`<>`、`IS NULL`
    - d) 表空间已满

#### Week 16

26. 事务的一致性条件包括哪些？
    - a) 事务开始前后，数据库必须满足一定的约束条件
    - b) 事务执行中，数据库可以不满足任何约束条件
    - c) 事务开始前后，数据库中的所有数据都必须相同
    - d) 事务执行中，数据库可以部分满足约束条件

27. 如何在Oracle中保证事务的一致性？
    - a) 使用日志机制和相应的修复机制
    - b) 仅使用日志机制
    - c) 仅使用检查点
    - d) 不需要特殊措施

28. 在数据库系统中，操作原语是指执行基本数据库操作的最小单元。以下哪一项不是操作原语？
    - a) INPUT(X)
    - b) READ(X,t)
    - c) WRITE(X,t)
    - d) PROCESS(X)

29. 如何手动创建数据库实例？
    - a) 使用CREATE DATABASE命令
    - b) 使用ALTER DATABASE命令
    - c) 使用CREATE INSTANCE命令


    - d) 使用INITIATE DATABASE命令

30. 在Oracle数据库中，SHUTDOWN IMMEDIATE命令的作用是什么？
    - a) 立即关闭数据库并回滚未提交的事务
    - b) 强制关闭数据库而不回滚未提交的事务
    - c) 正常关闭数据库，等待所有连接退出后再关闭
    - d) 启动数据库实例

#### Week 17

31. 函数依赖（Functional Dependency）描述了什么？
    - a) 表之间的关系
    - b) 属性之间的约束关系
    - c) 数据库的性能
    - d) 数据库的安全性

32. 数据库规范化的主要目的是？
    - a) 提高数据库的存储空间
    - b) 减少数据的冗余和提高数据的一致性
    - c) 增加数据的冗余
    - d) 降低数据库的性能

33. 在ER图中，哪种符号表示实体集？
    - a) 矩形
    - b) 椭圆
    - c) 菱形
    - d) 三角形

34. 如果实体集E到F的联系是多对一，那么在ER图中如何表示？
    - a) 箭头指向F
    - b) 箭头指向E
    - c) 用双箭头表示
    - d) 不使用箭头

35. 如果一个实体集的属性可以唯一标识实体集中的每个实体，该属性称为？
    - a) 候选码
    - b) 主码
    - c) 外码
    - d) 关键字

#### Week 18

36. 在PL/SQL中，如何创建一个包（Package）？
    - a) CREATE PACKAGE package_name IS ... END package_name;
    - b) DECLARE PACKAGE package_name IS ... END package_name;
    - c) SET PACKAGE package_name IS ... END package_name;
    - d) CREATE PACKAGE BODY package_name IS ... END package_name;

37. 如何调用包中的过程（Procedure）？
    - a) EXECUTE package_name.procedure_name(param1_value, param2_value);
    - b) RUN package_name.procedure_name(param1_value, param2_value);
    - c) CALL package_name.procedure_name(param1_value, param2_value);
    - d) PERFORM package_name.procedure_name(param1_value, param2_value);

38. Oracle 19c中，哪种函数被LISTAGG函数替代？
    - a) WM_CONCAT
    - b) GROUP_CONCAT
    - c) STRING_AGG
    - d) STRING_JOIN

39. 在PL/SQL中，%TYPE声明方式的优点是什么？
    - a) 保持数据类型一致性
    - b) 提高代码的执行效率
    - c) 增加代码的可读性
    - d) 减少代码的复杂性

40. 在PL/SQL中，如何声明一个记录类型变量，该变量的结构与游标的行结构相同？
    - a) v_record cursor%ROWTYPE;
    - b) v_record cursor%TYPE;
    - c) v_record cursor%RECORD;
    - d) v_record cursor%STRUCT;

### 答案

1. c
2. a
3. b
4. c
5. c
6. b
7. c
8. a
9. a
10. b
11. b
12. b
13. b
14. a
15. a
16. a
17. a
18. a
19. a
20. a
21. c
22. d
23. a
24. a
25. c
26. a
27. a
28. d
29. a
30. a
31. b
32. b
33. a
34. a
35. b
36. a
37. a
38. a
39. a
40. a