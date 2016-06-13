#iOS Dallas构架
##前言
*  `Dallas`，取名来源于NBA，为满足未来开发多款APP的需求，需要将业务进行拆分，开发更多独立的模块，dallas的初衷就是为了实现这样的需求；

##设计原则
*  所有模块的设计，需要满足六大原则，
*  1、单一职责原则
*  2、里氏替换原则
*  3、依赖倒置原则
*  4、接口隔离原则
*  5、迪米特法则
*  6、开闭原则

##一、概述
* 1、此工程主要放置基础控件的管理库，对外仅提供Framework,.a包；
* 2、一级目录仅存放文件夹；且一级目录下面亦需要提供README.md文件，
     用于描述此文件所提供的模块，越详尽越好；
* 3、所有子工程，提供三个Targets，`Framework`、`Aggregate`、`TestApp`，其中测试APP，均可以独立运行；
* 4、关于命名，所有模块的命名，均以M开头，以Framework结尾；
* 5、关于注释，请使用`VVDocumenter`进行描述的添加；
* 6、关于代码规范，请参阅 http://google-styleguide.googlecode.com/svn/trunk/objcguide.xml
* 7、本工程的管理，基于Submodule，更新及下载请使用如下命令`git submoduel update --init --recursive`

##二、子工程（排名不分先后）

| 模块名称		|工程							| 使用中的APP	|    备注	|		作者	|
|---------------|-------------------------------|-----------|-----------|----------:|
|QQ联系人控件		|MTreeFramework				    | 			|			|     Micker|
|淘宝SKU控件		|MSKUFramework				    |		    |			|	  Micker|
|日志输出控件		|MLogFramework				    |		    |			|	  Micker|
|Debug控件		|MDebugFramework			    |		    |			|	  Micker|
|全屏浏览控件		|MFullScreenFramework		    |		    |			|	  Micker|
|淘宝商详控件		|MDetailFramework			    |		    |			|	  Micker|
|Section控件		|MSectionFramework			    |		    |			|	  Micker|
|日历展示控件		|MCalendarFramework			    |		    |			|	  Micker|

##三、发布
* 所有子Framework的，可以根据需求，进行单独编译

##四、博客
[Micker.cn](http://micker.cn)