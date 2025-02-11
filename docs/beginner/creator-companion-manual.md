---
title: Creator Companion下载和使用手册
---

# Creator Companion下载和使用手册；
![](/img/vrcd-img/tag-vrcd.png)  

### 前言//
![](/img/starter/creator-companion-manual/CreatorCompanion.png)  
**Creator Companion**（以下简称CC）是**VRChat**推出的用于辅助开发者的开发软件，功能齐全，可以做到检测，安装和替换SDK等的多个功能，并且有着英文版的官网手册，开发工具，社区资源等。

从某种意义上来说，在VRChat开发过程中CC是必不可少的工具，缺少这一工具可能会让工程开发变得十分困难，我们推荐您尽可能下载CC。

您将在此教程中了解到以下有关CC环境配置的知识，分别是：

+ **下载和设置CC**（必读）  
+ **创建工程**（必读）  
+ **更新工程**（必读）  
+ **CC默认插件列表**（必读）  

既然您选择了这个文档，我们在接下来的文章中将默认您具备建立国际网络环境的能力，**如果您无法建立国际网络环境，我们建议您阅读《Vrchat SDK装配手册》以顺利装配开发环境。**

### 下载和设置CC//
先找找看CC在哪里下载。  
我们可以在VRChat Creation网站中找到下载CC的入口，网址如下：  
https://docs.vrchat.com/docs/setting-up-the-sdk

请点击红框标注的**Here**下载CC，不出意外的话CC的下载任务此时应该已经在浏览器上进行了。

![](/img/starter/creator-companion-manual/1.png)

安装好CC，初次打开CC会看见这一个界面，点击中间蓝蓝的**Show Me Around**即可进入主界面。

![](/img/starter/creator-companion-manual/2.png)

让我们简单了解一下CC的主界面（**仅限于VRCD-VRChat入门包涉及的内容/英文界面为例**）：

**工程文件区域**显示您基于CC所创建的所有项目文件，在框中标明了该项目的名称，储存位置，项目类型，以及管理项目的入口。
**Logs**（日志）显示您在CC进行的所有操作返回的结果，可以利用这一面板大致排查自己的错误点（虽然在大部分情况下返回的结果都很莫名其妙）。

![](/img/starter/creator-companion-manual/3.png)

让我们简单了解一下CC的设置界面：

您可以在通用设置界面选择您安装的Unity编辑器的位置以手动配置（只有在您的CC无法正常识别Unity编辑器时有用），您也可以通过设置CC的备份位置以让自己的工程万无一失。

![](/img/starter/creator-companion-manual/4.png)

### 创建项目//
回到主界面，点击右上角的**Create New Project**。

![](/img/starter/creator-companion-manual/5.png)

在Select template下，有三个Unity工程模板选项：
+ **World Project是为制作世界提供的模板。**
+ **Avatar Project是为制作化身提供的模板。**
+ **World Project with UdonSharp是为制作以U#为基础建立的世界提供的模板。**  

三选一选择自己想做的项目，CC就会自动部署好该项目所需的环境。  
需要注意辨别的是，在选中的情况下再点一次相同选项为取消选择（我们提醒这一点是因为选中和未选中的差距小到无法让人轻易察觉），请仔细确认自己是否选择相应的模板。

接下来便是在**Project Name**（项目名）里为自己的项目命名，之后在**Project Location**（项目位置）中选择您打算储存项目的地方，这边建议设置为和Unity Hub设置的项目储存位置一致的地方。

点击**Create Project**按钮进行工程创建，在短暂的等待后CC会为您创建工程并且自动安装相应的插件。

![](/img/starter/creator-companion-manual/6.png)

>如果CC显示工程创建失败或您没有看见有任何工程被创建，您可以试着检查**您的Unity Hub的许可证是否过期**。

创建好项目以后，您将看到如下的界面，在这里您将看到许多来自社区与VRC官方的插件包，在大部分情况下保持默认设置足够您进行目前阶段的创作活动。  
如果您想添加/删除插件，您可以点击右侧的加减符号进行修改操作。

想打开项目瞅一瞅？  
您可以直接点击右上角的Open Project以打开项目（以World Project为例）。

![](/img/starter/creator-companion-manual/7.png)

### 添加项目//
如果您的项目是通过Unity Hub创建的，并且希望通过CC完成进一步部署与插件更新，请点击Create New Project旁的下箭头展开，点击**Add Existing Project**，选择项目所在的文件夹。

![](/img/starter/creator-companion-manual/8.png)

### 更新项目//
您需要在制作项目时定期更新组件包，我们需要进入指定的管理项目页面去更新组件包。
>如果您的项目已经未更新许久，在您通过CC打开项目时，CC会自动帮您更新项目。

![](/img/starter/creator-companion-manual/9.png)

被标有绿色向上箭头的包便是需要更新的组件包，单击便可开始更新。
>当前版本号显示项目目前使用的插件版本号，更新版本号显示目前最新的插件版本号。

![](/img/starter/creator-companion-manual/10.png)

另外，由于CC存在的各种不尽人意的网络连接与逻辑问题，我们建议您时常备份项目。