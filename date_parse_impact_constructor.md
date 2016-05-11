[返回首页](http://www.caoyangyang.cn/)
# 会让我犯迷糊Date的边边角角
###先看下面两个生成Date的方法

```
new Date("2011-1-1")
>Sat Jan 01 2011 00:00:00 GMT+0800 (CST)
new Date("2011-01-01")
>Sat Jan 01 2011 08:00:00 GMT+0800 (CST)
```
为什么生成了两个不一样的日期,

原因是利用字符串生成dete类型数据时，其实是做了两步

```
1.利用Date.parse将字符串转化为毫秒数
2.将得到的毫秒数转换为Date
```
说白了就是 new Date("2011-1-1")实际是new Date(Date.parse("2011-1-1"))

而两次new Date结果不一样的原因就是

```
Date.parse("2011-01-01")
>1293840000000
Date.parse("2011-1-1")
>1293811200000
```
而parse结果不一样的原因，下次聊。

