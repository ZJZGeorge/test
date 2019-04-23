# PsychoR编程练习——混合线性模型

主要需求
-------------------------------------------------------

已有研究表明不同句子类型（如双宾结构句子（DO句）与介词-宾语结构句子（PO句））会引导个体说出同样类型的句子。现想研究上述的情况（称为启动效应）是否会受读写能力影响，即不同读写能力水平的个体内启动效应是否存在。

需求具体描述（使用混合效应模型）
-------------------------------------------------------

双宾结构句子（DO句）与介词-宾语结构句子（PO句）的启动效应比较：

- 启动句类型为DO条件下产出的DO是否显著多于启动句类型为PO或Baseline条件下产出的DO
- 启动句类型为PO情况下产出的PO是否显著多于启动句类型为DO或Baseline条件下产出的PO

文盲（读写能力低）与非文盲（读写能力高）被试间的启动效应是否有显著差异：

- 文盲与非文盲被试在DO句启动效应中是否有显著差异
- 文盲与非文盲被试在PO句启动效应中是否有显著差异


数据信息：
-------------------------------------------------------

数据形式为数据框，变量如下：

- experiment（实验编号）：
- literacy（被试读写能力）：，低水平与高水平
- subjectid（被试编号）：
- item（实验题目）：
- prime（启动句类型）：PO，DO，Other三个类型
- PO：是否输出PO句
- DO：是否输出DO句
- Other：是否输出其他类型句子

数据格式：csv格式
需要进行数据预处理（literacy变量需删除中文备注）

R包工具：

- lmerTest
- effects
- emmeans

[数据链接](https://trello.com/c/nWaWJ0yn/2-%E6%B7%B7%E5%90%88%E6%95%88%E5%BA%94%E6%A8%A1%E5%9E%8B)

[参考资料1](https://mp.weixin.qq.com/s?__biz=MzA3MTM3NTA5Ng==&mid=2651059893&idx=1&sn=35f2f6ead21d29cd965769aa09f8418f&chksm=84d9d722b3ae5e34534b1f9942cf1c342fd2b2111d665422f61e8bb637835c75568293c59a67&mpshare=1&scene=1&srcid=0222zlf5z0GcLaU2T2T18iyW&key=596bb344bde38dd2bc9a235f658f2c2935e5fed540616f0654acaefe465244e466c116c9b45e0cacc8d06653c6122f722e380a393cdb0ce3ae1a81e754df31ef03abff6625184d8259439b22ce28e958&ascene=1&uin=MTI0ODI4NTU4NA%3D%3D&devicetype=Windows+7&version=62060739&lang=zh_CN&pass_ticket=gKkIZgcxOI20b78lW5%2FKwanphm4M4RGiIdZripo8CSbwan89%2FYYCcZ9QySenp7wU)

[参考资料2](https://mp.weixin.qq.com/s?__biz=MzU5MjEwODg1OA==&mid=2247483973&idx=1&sn=d3b41cb1b0c2268441c658653de10d62&chksm=fe258e10c9520706d992850becd31346fbd7996ef09e2246196fe2df336435eff4afd35313cf&mpshare=1&scene=1&srcid=&key=e6e0bf5c3f2e82db6efde1ec3996478fb9c9e2308e3da0b3617005c126749b76450db2414baed8e96f51e76777a26713e0c2c41759bc947300f8bed69b9ce2f272cde15743cdac3c8f8857119ef1f508&ascene=1&uin=MTI0ODI4NTU4NA%3D%3D&devicetype=Windows+7&version=62060739&lang=zh_CN&pass_ticket=rH3DdQRfPfw%2B%2BPIKgpNNzXRfi131%2FpwgXHv5uMU%2BlRj2fnx5fsedc%2BKMarWfkPwl)
