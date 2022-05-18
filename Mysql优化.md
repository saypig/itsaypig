# Mysql优化

## explain分析sql语句执行效率

例：explain SELECT * FROM `sys_dept`

![image-20220518092418194](C:\Users\novots\AppData\Roaming\Typora\typora-user-images\image-20220518092418194.png)

id：查询编号

select_type：查询类型

table：查询的表

type：是否走索引

key：索引列

key_len：索引长度

rows：影响行数

## 慢日志查询分析

开启慢sql日志，超过设置时间记录慢日志，可sql开起，也可配置开起。

## show profile分析

分析一句sql的执行过程，包括cpu及内存，完成的sql执行经过。

## druid连接池

druid可监控数据慢sql.