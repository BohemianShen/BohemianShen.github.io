#2023.10.16

前海汇流一面
1. 假设访问百度网站，从在浏览器输入网址，到最终页面展示出来，中间会发生哪些事情？
2. http和https的区别
3. https如果只采用单种加密方式，例如只采用非对称加密，或对称加密，会存在什么样的问题？
4. 如果缺少CA数字证书的验证，https协议可能存在什么问题？
5. TCP 3次握手
6. 握手过程中，客户端和服务端会经历哪些状态
7. 如果没有第三次握手，这样的连接为什么就不可靠了？
8. 做一道SQL题（详见下方）
数据库中有以下两张数据表：

广告表
表名：ad
字段：id, title, create_time

订单表
表名：order
字段：id, ad_id, cost, create_time

请写一条 SQL，查询订单数量前十的广告，并返回以下信息：广告ID、广告名称、订单数量总和、订单费用总和。

9. 基于你的SQL语句，你会怎样去给两张表设计索引？
11. 假设这两张表的数据量在10w以上，结合你刚才设计的索引，分析一下这个SQL查询的性能，是比较好还是比较差？
12. 一般你会怎样分析一条SQL语句的性能呢？或者怎样判断一条SQL语句是好还是不好的？
13. 针对这个语句，你能大概想象它的执行计划会是怎样吗
14. 分析一下你写的语句会命中哪些索引
15. 在explain的结果中，你提到会关注扫描行数，那针对这条语句，你觉得它的扫描行数会是多少呢
16. 说一下在innoDB存储引擎下，索引是如何实现的？
17. 说一下B+树有哪些特点？
18. 讲一下聚簇索引和非聚簇索引的区别？
19. 补全下面的代码
函数 reverse (char *s, int len) 的功能是用递归的方式逆置长度为len的字符串s。例如：若s的内容为“abcd”，则逆置后其内容变为“dcba”，请补充完整下面的代码。
void reverse (char *s, int len)
{
    char ch;
    if (____1____)
    {
        ch = *s;
        *s = * (s + len - 1);
        * (s + len - 1) = ch;
        reverse (____2____, ____3____);
    }
}
20. 
