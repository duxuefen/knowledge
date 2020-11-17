#  有关Redis的命令

##  Redis更新操作

**写流程（更新策略）**

1. 先淘汰 cache（删除缓存）；
2. 再写 DB（更新数据库）。

**读流程**

1. 先读 cache，如果数据命中 hit 则返回；
2. 如果数据未命中 miss 则读 DB；
3. 将 DB 中读取出来的数据入缓存

## Redis的RedisTemplate(模板)[的使用](https://blog.csdn.net/aoxiangzhe/article/details/93164823)

