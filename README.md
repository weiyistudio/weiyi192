# weiyi192
基于Web的网上药店管理系统的设计与实现


# 基于Web的网上药店管理系统的设计与实现

#### 介绍
   

随着计算机网络技术的快速发展，也随着中国的经济迅速发展，近些年的医疗条件已经有了很大的改善，但是疾病的种类仍然是不断地增加。致使国人对药品的需求量也随之不断加大，然而市面上各个药店在药品管理以及药品销售方面，都采用了传统方式（手工管理和到店选购），这种传统的管理及销售方式，存在着很大的弊端，首先药品信息和数据庞大且纷乱复杂，整理统计费力费时，其次是手工统计操作效率低、保密性差，另外时间一长，将产生大量的资料，这对于查找、更新和维护都带来了不少的困难，这对管理者来说会造成诸多的不便，更有可能疏忽一些细节。
对于以上存在的问题，都反应出了对药品的管理和销售，需要进行信息化，药店如果采用计算机系统化、以及互联网信息化管理以及销售的方式，那么既能满足群众对药品的需求，也能避免很多药品管理弊端。
《基于Web的网上药店管理系统的设计与实现》的研究，是以Web技术为核心，设计出的基于B/S架构的管理系统。其特点可以在线展示药品信息、使用户通过网络上看到的相关的药品信息，同时可以根据自己想需要购买所需药品。基于Web的网上药店管理与销售系统完成用户及管理员身份验证、对药品信息查询及修改，销售管理等功能，其中最重要的就是药品的销售功能，对销售情况的统计，以及对库存中药品数量的管理功能等。作为一个完整的系统，为了保证系统的安全运行，还必须要对使用者用户的身份进行验证 





#### 项目说明


在本系统中，为了保证用户安全舒适的通过网络环境对药品进行购买，设计简单易用的业务操作流程：用户可以注册登录网站，登录后，用户能够浏览网站的详细内容，提供搜索引擎，使用户能够按特定的条件对所需的药品进行搜索，用户下定单购买药品，用户也修改定单的购买数量，查看定单等。

![输入图片说明](https://images.gitee.com/uploads/images/2021/1028/000059_f9915b90_8650135.png "屏幕截图.png")

对于典型的数据库管理系统，尤其是对这样的数据信息量比较大的网络管理系统，必须要满足使用方便、操作灵活等设计要求。本系统在设计时应该满足以下的功能需求：
（1）顾客可以方便地查看药品信息。
（2）顾客可以方便的对购物车中的药品进行增加、删除、修改和下订单。
（3）顾客可以方便的查找药品。
（4）管理员可以方便地添加、删除、修改药品信息。
（5）管理员可以方便地添加、删除、修改和查看药品分类。
（6）管理员可以方便地查看订单，可以方便地进行药品发货操作。

![输入图片说明](https://images.gitee.com/uploads/images/2021/1028/000118_bd1200ae_8650135.png "屏幕截图.png")

在用例图中，角色用于描述与系统功能有关的外部实体。通过对网上药品管理与销售系统的分析，确定系统中的角色：用户、管理员。在确定角色的基础上，确定用例。基于Web的网上药店管理与销售系统中的用例有：用户注册、用户登录、药品查询、查看购物车、下订单、查看订单、药品管理、药品分类管理、订单管理。 
出来用用例图描述系统需求外，还可以用文字对每个用例进行需求说明，更具体地描述该用例与角色的交互。
用户注册：为顾客提供注册的功能，使管理员能够清楚了解每个顾客的个人信息。
用户登录：为顾客提供身份确认的功能，保证合法的权利。
药品查询：用户进行查询，方便、快捷地找到要找的药品信息。
查看购物车：为了方便顾客购物，每个用户都有一个购物车，用户在购买时可以更改药品数量。
下订单：用户对订单信息进行确认后提交订单，管理员将在未处理的订单页面查看到此订单。
查看订单：用户能够对下过的订单信息进行查询。
药品管理：管理员能够对药品信息进行增删改查的操作。
药品分类管理：管理员能够对药品分类信息进行增删改查的操作。
订单管理：管理员能方便地查看所有的订单信息、发货状态和对订单进行发货的操作。


基于Web的网上药店管理与销售系统可分为后台管理员部分和前台用户两大部分。前台主要完成的功能是针对消费者的，包括药店药品分类、药品查询、购买药品等。在现实生活中的超市里每个消费者都有一个购物车，在这里也为用户建立了一个购物车，只是这里的购物车是虚拟的，但是它却具有现实生活中购物车的功能。
后台的主要功能是增加、删除药品信息，查询药品信息、设定药品信息，对药品的类别进行管理，查询统计销售信息。
把数据存储到数据库：用户帐号信息，药品信息，药品分类信息，用户地址信息，以及购物车等信息应当长期存储到磁盘上的数据库中，即使系统出现电源故障也不至于丢失用户信息。
并发控制：当多个线程在同一时刻试图访问同一资源时，并发控制将成为一个重要的问题。
处理用户会话：当基于Web的网上药店管理与销售系统需要同时处理多个用户的并发访问，因此必须维护每个用户的会话信息。

![输入图片说明](https://images.gitee.com/uploads/images/2021/1028/000148_0f351f66_8650135.png "屏幕截图.png")



#### 项目截图

![输入图片说明](https://images.gitee.com/uploads/images/2021/1028/000222_64810a03_8650135.png "屏幕截图.png")


![输入图片说明](https://images.gitee.com/uploads/images/2021/1028/000239_b11a3ad4_8650135.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2021/1028/000312_4ef2e94c_8650135.png "屏幕截图.png")

#### 求助热线




代码有任何问题可联系
联系Q：2762501186

                            
![输入图片说明](https://images.gitee.com/uploads/images/2020/1119/003728_cd598bb9_4865385.jpeg "微信.jpg")       

![输入图片说明](https://images.gitee.com/uploads/images/2021/1026/221249_847cb212_8650135.png "屏幕截图.png")


    

感谢Gitee！！  
觉得项目不错的给个Star谢谢大佬！！！
提供无偿review服务
限时加好友入群！！！
