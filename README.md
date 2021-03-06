# 概述
本项目是一个 spring 框架实现的电商类销售系统。

系统有两类用户：卖家和买家。

* 卖家可以发布内容，为内容定价，查看购买情况。
* 买家可以浏览已发布的内容摘要，选择购买，查看已购买的内容。


# 功能需求

### R1 展示（首页）
* R1.1 系统的基本界面为卖家所有内容的展示。
	* R1.1.1 展示的细节为内容的标题、图片和价格。
* R1.2 用户登陆前，展示界面有登陆按钮。
* R1.2 买家登陆后，展示界面显示用户昵称，有退出、账务两个功能按钮。
* R1.3 买家登陆后，已购买的内容上有特殊标识表明已购买。
* R1.4 买家登陆后，可以只查看未购买的内容。
* R1.5 卖家登陆后，展示界面显示用户昵称，有退出、发布两个功能按钮。
* R1.6 卖家登陆后，已出售的内容上有特殊标识表明已出售。
* R1.7 卖家登陆后，可以在展示界面删除未出售的内容。

### R2 登陆
* R2.1 用户登陆时，需要输入用户名和密码，前端将密码用MD5加密后传输。
* R2.2 登陆后，所有界面上要显示用户的昵称。

### R3 查看
点击展示中的每个内容的网格，进入查看界面，可以查看内容。

* R3.1 买家对于没有购买的内容，看到的是标题、摘要文字、当前的价格、购买按钮、全文。
* R3.2 买家对于已经购买的内容，看到的是标题、摘要文字、购买时的价格、购买按钮不可用、全文。
* R3.3 卖家看到的是标题、摘要文字、价格、全文、编辑按钮。

### R4 购买
* R4.1 在查看界面点击购买按钮，弹出确认窗口。
* R4.2 点击确认按钮就完成了购买，跳转至账务页面。
* R4.3 用户已经购买过的内容不能重复购买。

### R5 账务
* R5.1 在展示界面点击“账务”按钮，进入账务界面。
* R5.2 在账务界面以列表方式列出所有已购买的内容，每一项内容列出：
	* 标题；
	* 图片；
	* 购买的时间；
	* 购买时的价格。
* R5.3 列表的最后计算出总的金额。

### R6 发布
* R6.1 卖家在展示界面点击“发布”按钮，进入发布界面。
* R6.2 在发布界面可以输入内容的标题、摘要、图片、正文和价格，点击发布按钮即发布，回到查看界面。

### R7 内容的编辑
* R7.1 卖家在查看界面可以点击编辑按钮进入编辑界面。
* R7.2 可以修改内容的全部细节：标题、摘要、图片、正文和价格，点击提交后回到查看界面。


# 项目说明

### P1 文件结构
* war包工程： `emall-manager\emall-manager-web\`
* 前端资源： `emall-manager\emall-manager-web\src\main\webapp\`
* 逆向工程： `generatorSqlmapCustom\`

### P2 运行环境
* 数据库：`MySQL`
* JAVA版本：`1.8.0_91`
* Tomcat版本：`7.0.67`
* 测试环境：`windows 10 x64`; `Ubuntu 14.04 x64`
* 编码格式：`UTF-8`

### P3 数据库帐号
* 数据库用户名：`root`
* 数据库密码：`J06GBUrMGdG6d84c`

### P4 测试地址
* 部署测试：`106.2.110.68:8080` （现已关闭）
* 测试用户：
	* 买家：`buyer` 密码：`reyub`
	* 卖家：`seller` 密码：`relles`

