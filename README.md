# [首页查询更多项目](https://github.com/GraduationProject-springboot) 包安装运行


# 0045springboot古典舞在线交流平台的设计与实现

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV16ia6epENY?p=46)


# 第一章 绪论
## 1.1研究背景
在当今的社会，可以说是信息技术的发展时代，在社会的方方面面无不涉及到各种信息的处理。信息是人们对客观世界的具体描述，是人们进行交流与联系的重要途径。人类社会就处在一个对信息进行有效合理的加工中。它将促进整个社会的发展。随着社会信息技术的提高，计算机已被广泛应用于当今社会的各个领域，成为推动社会发展的首要技术动力。

一个行业发展起来，自然会诞生相关的交流网站，随着经济的快递发展，学习舞蹈的人越来越多，在众多舞种中，学习古典舞的人也在不断增多，传统古典舞交流的方式有时间地点的限制，在当今社会已经无法满足用户的需求，针对这一情况，结合目前计算机技术的发展，特开发了本古典舞在线交流平台。在互联网的迅速发展下，局域网的普及，为建立古典舞在线交流平台的设计与实现提供了基础条件。古典舞在线交流平台与传统的古典舞交流方式相比，有着无法比拟的优点，网络共享、传播速度快的特点，用户可以随时随地进行古典舞交流，同时管理员通过计算机对系统信息进行全面管理，大大提高了古典舞交流效率。
## 1.2 设计原则
在开始开发项目之前，必须要先考虑项目的实用性、科学性，以及该项目是否能够真正让用户受益并尽可能的发挥项目的作用。因此，在开发前，通过以下几条原则对项目进行判断：

（1）可行性原则。项目需要保证经济可行性和技术可行性，这包括了项目在浏览端、服务端等方面上的经济和技术上是可以达成的。

（2）适应性原则。项目要保证可维护性和可扩展性，这是每个非短期项目都需要考虑的，并且不论是维护还是扩展，都必须要建立在适应用户的正常需求的基础上。

（3）安全性及保密性原则。要充分保证用户信息的安全性和保密性，不能因为开发上的疏忽，导致用户的信息泄露。

（4）系统工程原则。为了确保项目的整体性，在项目调查、项目分析、项目设计、项目开发的过程中，都需遵从项目工程的方法和步骤逐步进行。

（5）统一规划、分期实施、逐步完善原则。项目开发的过程中，要按照规划、分期实施，特别是要注意在项目开发过程中要有条理，从点到面，一步步完善，不要贪图进度，要循环渐进的对项目进行开发。
## 1.3 论文组织结构
第一章主要是简单的介绍下设计本网站的研究背景、设计原则，在这一章里主要是让大家了解下我的设计的前因后果，为接下来我的其它章节做铺垫。

第二章主要是介绍在设计过程中所涉及到的技术。

第三章主要是介绍下设计这个网站所需要的需求以及我们的功能需求分析，因为只有更好的分析清楚我们的功能需求才能更好的完成我们的设计。

第四章网站系统设计，主要介绍了网站结构的设计，这一章主要是为了能让大家更好的了解网站的一些基本设计信息。

第五章系统的实现，介绍了系统每个模块的设计与实现，让大家能清晰的了解系统的主要功能。

第六章系统的测试，这章主要是测试下各个部分每个功能是否能用，看下是否有错误。

10

10
# 第二章 相关技术介绍
## 2.1Java技术
Java是一种非常常用的编程语言，在全球编程语言排行版上总是前三。在方兴未艾的计算机技术发展历程中，Java的身影无处不在，并且拥有旺盛的生命力。Java的跨平台能力十分强大，只需一次编译，任何地方都可以运行[9]。除此之外，它还拥有简单的语法和实用的类库，让编程人员可以尽可能将精力集中在问题的求解上，并且许多开源项目和科研成果都是采用它实现的。

在1995年这一年的5月份，著名的Sun Microsystems公司在程序开发设计上面郑重推出一种面向对象开发的程序设计语言——Java，最开始的时候Java是由詹姆斯.高斯林这位伟大的JAVA之父来进行主导，但是在后来由于各种原因，让甲骨文公司这个针对商业程序创建了oracle大型数据库的公司收购了Java。Java的平台总共算下来有3个，分别为javaME和javaSE以及javaEE这3个java平台。下面将对其进行分别介绍。

（1）在电脑桌面程序的开发上面需要选择JavaME，这个用得也比较多。

（2）企业也会根据工作以及业务需要开发各种软件，那么就会选用JavcEE这个支持企业版软件的开发的Java平台，JavcEE主攻运用在企业领域上面的web应用，JavcEE也在javaSE的基础上获得了比如jsp技术 ，Servlet技术等程序开发技术的支持。

（3）现在生活中手机的普及化，也使得手机端这样的移动设备的软件的兴起，JavaME这个迷你版java平台就能运用于移动端的软件开发操作。
## 2.2MYSQL数据库
MySQL是典型的关系数据库系统，拥有开源免费、稳定、高效等特点，一直是中小型web项目的最佳数据库选择。MySQL作为当今IT领域使用人数最多的开源关系型数据库软件之一，在2018年的数据库使用率排名中位居第二，仅次于目前为止最成功的商业版数据库Orcle[12]。MySQL最大的优势之一就是无偿使用，这也是它成功的关键。

MySQL支持标准化数据库查询语言SQL。MySQL是一款非常适合个人开发者或小型组织开发团体的数据库管理系统，因为它是开源并且免费的，体积小、速度快、成本低以及其最重要的一点开放源码，深受程序设计人员的喜爱，这也让它成为了许许多多中小型开发网站数据库的首选，同时提供了多种开发的连接API。MySQL将数据的存放按照记录之间的关系存放到了不同的表中，减少了数据的冗余并且提高了开发的工作效率。MySQL支持开发中需要用的大型数据库，并能处理数以万计的记录。因为MySQL是开源的软件，所以在项目的预算中的时候不用花费额外的资金，大大降低了开发的总体成本，这也是MySQL数据库在中小型企业和独立的开发者中广泛流行的原因[11]。
## 2.3 B/S结构 
在早期的程序开发中，使用得最多的莫过于C/S架构了，现在的生活中软件在生活的各个方面落地，使用了C/S架构开发出来的软件也是不在少数的，比如企业日常办公使用到的微软的OFFICE软件，我国自己研发的文档处理软件WPS，还有娱乐软件腾讯的QQ，腾讯的微信，以及电脑上安装的杀毒软件金山杀毒软件，瑞金杀毒软件等都是C/S架构。但是在Internet网络盛行之后，鉴于大家对数据信息共享的需求，在原来的C/S架构上进行了升级改进之后，有了现在的主流架构B/S架构，B/S架构就是在C/S架构上多了一个浏览器，让原来的直接访问服务器的方式，变成了通过浏览器去访问服务器。充分运用到了当下不断成熟的浏览器技术。也让软件的开发成本以及维护成本降低了。可以说B/S这种新型的架构模式让软件的开发变得便利化。
## 2.4 Spring Boot框架
Spring Boot是一个简化程序设置的拥有开箱即用的框架，它主要的优点是根据程序员不同的设置而生成不同的代码配置文件，这样开发人员就不用每个项目都配置相同的文件，从而减低了开发人员对于传统配置文件的时间，提高了开发效率。它内嵌Tomcat服务器，简化了Maven的配置，自动配置Spring，通过这样的框架，开发人员就不用头疼各种配置文件，可以减少时间，同时提高了代码的整体性，使开发人员工作效率大大提高。


# 第三章 系统分析
## 3.1 可行性分析
需要使用大部分精力开发的古典舞在线交流平台为了充分降低开发风险，特意在开发之前进行可行性分析这个验证系统开发是否可行的步骤。本文就会从技术角度，经济角度，还有操作角度等进行综合阐述。
### 3.1.1技术可行性
本文将开发的系统，将采用的关键技术包括JAVA编程语言、B/S架构、MYSQL数据库存储技术等。另外，程序开发需要在自己电脑上安装的软件并不多，在win7操作系统的大环境下，能够完全搭建好程序开发的操作环境，比如开房工具，MYSQL数据库工具，以及处理程序图片的Photoshop工具等都能安装在自己的电脑上。总的说来，开发这个程序在技术上是可以实现的，该项目的开发是有保障的。
### 3.1.2经济可行性
开发这个程序软件并不会涉及到经济上面的开销，在开发软件的选择上也不会额外付费安装软件，在开发软件的官网上面就可以下载需要的软件，并根据提示的安装步骤安装软件到自己的电脑上面。因此，该项目的实施在经济上完全可行。
### 3.1.3操作可行性
操作可行性主要是针对系统用户而言，一个系统再完美，技术再先进，用户不去使用，或者用户根本不会使用，该系统存在的价值也是不大的。本系统拟采用的是B/S架构，用户只要通过点击浏览器即可轻松访问，而用户对浏览器操作非常熟练，所以从用户的角度而言，没有任何学习成本，因此，操作上是可行性的。
### 3.1.4时间可行性
从时间上看，在三个月的时间里学习相关知识，开发本古典舞在线交流平台，时间上是有点紧，但是不是不可能实现，在做毕业设计的这几个月里，我通过努力使得功能应该基本可以实现。

从上面几个部分的可行性分析得出，这次开发的古典舞在线交流平台在开发上面没有什么大问题，值得开发。
## 3.2系统性能分析
### 3.2.1 系统安全性
程序在使用中是不允许其他访问者随意窃取程序里面的隐秘信息，也不允许其他操作者越权操作其他管理用户操作的功能，要真正杜绝这些现象就必须在程序开发之前把程序的安全性给考虑进去。

比如现在很多程序都会把用户注册的功能给考虑进去，让用户在注册页面功能区填写自己的个人信息，这些数据信息涵盖了用户本人的姓名，用户对程序登录设置的密码，用户经常使用的邮箱，用户的常用联系方式还有用户的所住地址等信息，这些信息都是设计到用户本人的隐私，那么这些信息在传输给程序后台时，是需要进行管理并保存至对应的数据库文件里面。要是有人恶意窃取程序的数据信息，也就会让那些注册了此程序软件的用户的个人隐秘信息都会遭到泄露。这些信息落入其他不法分子手里，他们极有可能根据用户的隐私信息去骚扰用户，并把这些信息用于各种商业用途谋取其他非法的利益。所以数据安全性是一个系统能不能使用的首要标准。
### 3.2.2 数据完整性
数据完整性是确保数据信息是否具有可靠性，是否具有参考价值的一个重要因素，数据信息只描述一部分，或者必有的数据信息反而为空等现象都是代表着这个数据信息不完整，有数据缺陷，这是个很严肃的问题，因为这样的数据信息跟垃圾信息没什么两样。

说到数据完整性，不得不提最常用的程序表单功能。这些表单主要就是提取广大用户的数据信息的，需要广大用户根据表单上的要求，填写自己的姓名信息，以及自己的联系方式信息，有些也会有额外的信息填写要求，有必须要填的选项，也有不需要必填的选项。假如广大用户为了保护自己的隐私，或者不想受到其他人的骚扰，不填写必填项等信息，广大用户在最后提交此表单的时候，往往都是提交不了的。

由于数据表之间也会存在一定的联系，所以同一个数据也会出现在另一个表格里面，那么这两个表格记录的同一个数据应该是一样的。不能够是同样的数据信息在不同表中不一样。
### 3.2.3系统可扩展性
一切事物都是一直在发展，程序员开发软件也需要带着发展的思维去进行软件开发操作，这样的话，开发出来的程序在应对管理所需时，也会相对应的进行程序升级与更新。不论是功能完善还是数据库升级都能在原来的基础上对原有程序进行迭代升级。让开发出来的程序能够走得越来越远。这也是广大用户对程序软件的使用要求。
## 3.3系统流程分析
### 3.3.1注册流程
未有账号的用户可进行注册操作，用户注册流程图如图3.1所示。

![](/md/blog.001.png)

图3.1注册流程图
### 3.3.2登录流程
登录模块主要满足了管理员和用户的权限登录，用户登录流程图如图3.2所示。

![](/md/blog.002.png)

图3.2 登录流程图
### 3.4.3发帖流程
用户发帖前提必须是登录后才能进行，发帖内容不能为空，且合法才能进行提交发表成功。详见图3.3所示。

![](/md/blog.003.png)

图3.3 发帖流程图
## 3.4系统功能分析
本古典舞在线交流平台主要分管理员和用户两大功能模块，下面将详细介绍管理员和用户分别实现的功能。
### 3.4.1用户功能分析
用户在系统前台可查看系统信息，包括首页、服务、课程、视频、论坛交流、舞蹈资讯等，用户要想实现发帖、服饰购买等操作，必须登录系统，没有账号的用户可进行注册操作，注册登录后主要功能模块包括个人中心、我的订单、我的地址、服饰管理、课程管理、视频管理、论坛交流管理以及我的收藏管理。用户用例图如图3.4所示。

![](/md/blog.004.png)

图3.4 用户用例图
### 3.4.2管理员功能分析
管理员可登录系统后台对系统进行全面管理操作，管理员主要功能模块包括个人中心、会员用户管理、服饰管理、课程管理、视频管理、论坛交流管理、服务类型管理、视频分类管理、课程类型管理、系统管理以及订单管理。 管理员用例图如图3.5所示。

![](/md/blog.005.png)

图3.5 管理员用例图

# 第四章 系统设计
## 4.1系统概要设计
本古典舞在线交流平台采用B/S结构来开发，这种结构是在互联网兴起后出现的，是一个适用于互联网环境下的模型结构，用户只要能上网通过浏览器就可以在任何时间、任何地点的使用。系统工作原理图如图4-1所示：

![](/md/blog.006.png)

图4.1 系统工作原理图
## 4.2 系统结构设计
系统整体设计是一个将一个庞大的任务细分为多个小的任务的过程，这些小的任务分段完成后，组合在一起形成一个完整的任务。本古典舞在线交流平台主要包括用户功能模块和管理员功能模块，系统功能模块图如图4.2所示。

![](/md/blog.007.png)

图4.2 系统功能模块图
## 4.3 数据库设计
### 4.3.1数据库E-R图设计
E-R图是一种描述显示数据类型间的关系的数据描述方法，E-R图可以完整地映射出现实模型的关系。E-R图中的三个最为重要的元素就是实体、属性、关系。E-R图即由这三点组成。

实体：E-R图中数据的实体，用矩形表示上面为实体名，下面为实体属性，实体包含主外键等关系。

属性：E-R图中的属性，是指实体的属性，实体由多条属性所构成，属性拥有自己的数据类型，数据大小。属性的优劣决定了E-R图中实体的健全性、完整性。

关系：E-R图中的关系是指实体之间的关系，用菱形来表示实体间的关系，这些菱形关系的联系上有着一对多或多对多的数据联系，这些构成了E-R图的关系，E-R图的关系紧密连接了实体，使实体间的关联性更加的显著、易懂。本古典舞在线交流平台的E-R图如下所示：

（1）论坛交流信息实体E-R图如图4.3所示：

![](/md/blog.008.png)

图4.3  论坛交流信息实体属性图

（2）管理员信息实体E-R图如图4.4所示：

![](/md/blog.009.png)

图4.4  管理员信息实体属性图

（3）订单信息实体E-R图如图4.5所示：

![](/md/blog.010.png)

图4.5 订单信息实体属性图

（4）服饰信息实体E-R图如图4.6所示：

![](/md/blog.011.png)

图4.6  服饰信息实体属性图

（5）用户信息实体E-R图如图4.7所示：

![](/md/blog.012.png)

图4.7用户信息实体属性图
### 4.3.2数据库表设计
古典舞在线交流平台采用MYSQL数据库作为数据存储，下面介绍数据库中的各个表的详细信息。

表4.1 forum论坛交流信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|title|varchar|200|是|帖子标题|
|content|longtext||是|帖子内容|
|parentid|bigint|20|是|父节点编号|
|userid|bigint|20|是|用户编号|
|username|varchar|200|是|用户名|
|isdone|varchar|200|是|状态|

表 4.2  users管理员信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|username|varchar|100|是|用户名|
|password|varchar|100|是|密码|
|role|varchar|100|是|角色|
|addtime|timestamp||是|新增时间|

表 4.3  orders订单信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|下单时间|
|orderid|varchar|200|是|订单编号|
|tablename|varchar|200|是|商品表名|
|userid|bigint|20|是|用户编号|
|goodid|bigint|20|是|商品编号|
|goodname|varchar|200|是|商品名称|
|picture|varchar|200|是|商品图片|
|buynumber|int|11|是|购买数量|
|price|float||是|价格|
|discountprice|float||是|折扣价格|
|total|float||是|总价格|
|discounttotal|float||是|折扣总价格|
|type|int|11|是|支付类型|
|status|varchar|200|是|状态|
|address|varchar|200|是|地址|
|tel`|varchar|200|是|电话|
|consignee|varchar|200|是|收货人|

表4.4  fushi服饰信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|shangpinbianhao|varchar|200|是|商品编号|
|mingcheng|varchar|200|是|商品名称|
|tupian|varchar|200|是|图片|
|leixing|varchar|200|是|类型|
|xiangxicanshu`|longtext||是|详细参数|
|thumbsupnum|int|11|是|赞数|
|crazilynum|int|11|是|踩数|
|clicknum|int|11|是|点击次数|
|price|float||是|价格|

表4.5  huiyuanyonghu用户信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|zhanghao|varchar|200|是|账号|
|mima|varchar|200|是|密码|
|xingming`|varchar|200|是|姓名|
|xingbie|varchar|200|是|性别|
|`shouji`|varchar|200|是|手机|
|youxiang|varchar|200|是|邮箱|
|shenfenzheng|varchar|200|是|身份证|
|zhaopian|varchar|200|是|照片|
|money|float||是|余额|


# 第五章 系统的实现
## 5.1 用户功能模块的实现
### 5.1.1系统主界面
用户进入本系统可查看系统信息，主要包括首页，服饰，课程，视频以及论坛交流等，系统主界面展示如图5.1所示。

![](/md/blog.013.png)

图5.1系统主界面
### 5.1.2用户注册界面
没有账号的用户可进入注册界面进行注册操作，用户注册界面展示如图5.2所示。

![](/md/blog.014.png)

图5.2  用户注册界面
### 5.1.3论坛交流界面
用户在论坛交流界面可查看已有交流信息，并可选择查看详情，论坛交流界面展示如图5.3所示。

![](/md/blog.015.png)

图5.3 论坛交流界面
### 5.1.4课程详情界面
用户可选择课程查看详情信息，登录后可进行加入购物车或者购买操作，课程详情界面展示如图5.4所示。

![](/md/blog.016.png)

图5.4  课程详情界面
### 5.1.5购物车界面
用户在购物车界面可查看购物车商品，并可修改数量、删除或者提交订单等，购物车界面展示如图5.5所示。

![](/md/blog.017.png)

图5.5 购物车界面
### 5.1.6我的订单界面
用户可查看个人订单信息，我的订单界面展示如图5.6所示。

![](/md/blog.018.png)

图5.6 我的订单界面
## 5.2 管理员功能模块的实现
### 5.2.1管理员登录界面
管理员要想进入系统后台对系统进行管理操作，必须登录系统后台，管理员登录界面展示如图5.7所示。

![](/md/blog.019.png)

图5.7  管理员登录界面
### 5.2.2会员用户管理界面
管理员可增删改查会员用户信息，会员用户管理界面展示如图5.8所示。

![](/md/blog.020.png)

图5.8  会员用户管理界面
### 5.2.3服饰管理界面
管理员可增删改查服饰信息，服饰管理界面展示如图5.9所示。

![](/md/blog.021.png)

图5.9 服饰管理界面
### 5.2.4课程管理界面
管理员可增删改查课程信息，课程管理界面展示如图5.10所示。

![](/md/blog.022.png)

图5.10  课程管理界面
# 










