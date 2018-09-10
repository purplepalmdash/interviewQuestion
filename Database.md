### CRUD
参考:    
https://blog.csdn.net/bruesz/article/details/2006957


在很多技术性的文章，特别是有关数据库类的文章中，经常会看到一个缩写“CRUD”，那什么是CRUD呢？
CRUD其实是数据库基本操作中的Create(创建)、Retrieve(读取)、Update（更新）、Delete（删除）。而这里的Create(创建），就我理解而言，应该是增加记录的意思吧（不知道对不对），而不应该是创建数据库表的那个创建的意思。我们平常所说的增删改，也即是这里的Create、Delete、Update。
其实我觉得Read与其他3个操作放在一起感觉怪怪的，其他3个都是对数据库中数据的实际操作（会导致原始数据的变动)，但Read仅仅只是数据的读取而已，为何要把它与其它3个操作放在一起，就只有原创者知道了。即使放在一起，也应该有所区别，我觉得RCUD或者RUCD的缩写是不是更好一些 :)。

注：（2017.2.9）这是一篇很久之前写的文章了，远到忘了还写过这么无聊的文章 ￼， 现在重新看起来当时还是不是很成熟，将就改了俩点：1. R是Retrieve，不是Read   2. 当是觉得Retrieve比较跟其他几个不太一样，是以数据库为为主体，但是如果以观测体的角度（Retrieve：从数据库中重新提取数据），这四个操作其实还是比较类似的。

最后，再列一下SQL中对应与CRUD的语句 (其中的T是Table的名称)：

```
Create:
insert into T(...) values(...);
Read:
Select ... From T Where...；
Update：
Update T Set... Where...;
Delete:
Delete From T Where...；
```
