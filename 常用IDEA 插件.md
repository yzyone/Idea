
### 好用且常用的 IDEA 插件！ ###


## 一、前言 ##

IDEA 全称 IntelliJ IDEA，是java编程语言开发的集成环境。IntelliJ在业界被公认为最好的java开发工具。

不是我说的喔，百度百科说的... IDEA 如此好用，插件库也是很强大的，俗话说：“工欲善其事必先利其器”，不安排几个插件都不好意思说你开发工具用的是 IDEA ，接下来将介绍插件的安装方式。

## 二、IDEA 插件安装 ##

在使用插件之前，你需要了解 IDEA 的插件安装方式，安装 IDEA 插件是非常方便的，你只要知道插件的名字就可以直接安装， IDEA 插件安装有两种方式：

**1、在线安装**

在 IDEA 中选择：File —> Settings —> Plugins
你可以直接在开发工具输入插件的名字搜索安装，例如安装Lombok插件：


**2、离线安装**

进入 IDEA 下载插件官网：https://plugins.jetbrains.com，输入插件的名字搜索，下载插件对应 IDEA 版本的插件包

在 IDEA 中选择：File —> Settings —> Plugins —> Install plugin from disk —> 选择下载好的插件包进行安装


TIP： 安装完成之后，重启 IDEA 就行了。本文使用的 IDEA 版本为2020.1，IDEA 使用最新版本的话，可能对应的第三方插件的版本没跟上导致不能使用。熟悉完插件安装方式之后，接下来将介绍近二十余款常用的 IDEA 插件

## 三、插件 ##

**1、Lombok**

Lombok 项目是一个 Java 库，它会自动插入编辑器和构建工具中，Lombok提供了一组有用的注释，用来消除Java类中的大量样板代码。仅五个字符(@Data)就可以替换数百行代码从而产生干净，简洁且易于维护的Java类，使用 Lombok 时候需要安装 Lombok 插件和对应依赖

使用 Lombok 时候需要添加依赖：
    
    <dependency> 
      <groupId>org.projectlombok</groupId>  
      <artifactId>lombok</artifactId>  
      <version>1.18.12</version>  
      <scope>provided</scope> 
    </dependency>

更多Lombok用法查看：https://projectlombok.org


**2、Grep Console**

在启动应用时或调试时，IDEA 控制台输出一大堆日志，想要快速找到自己需要类型的日志是很麻烦的，此时使用此插件可以快速定位到自己想要的类型日志，比如 TRACE 、 DEBUG 等，也可以单独打开标签页显示自己需要的日志，日志分类也可以配置自己喜欢的颜色。



**3、Maven Helper**

查看和管理maven依赖的插件，可以展示pom.xml文件中的依赖以列表或树的形式，该插件可以很直观的帮你分析和排除冲突依赖


**4、GenerateAllSetter**

一款效率插件，它主要提供以下功能：

通过alt+enter对变量类生成对类的所有setter方法的调用

当两个对象具有相同的字段时生成一个转换器

当返回类型为List Set Map时生成默认值

在所有getter方法上生成对assertThat的调用



**5、Rainbow Brackets**

如果代码没有被格式化的话，阅读起来很痛苦，就算被格式化了，几千行代码，各种if嵌套，阅读起来连个结尾括号都找不到(如果你说你会折叠，当我没说)，也是很痛苦的，此时这个插件就能忙上很大的忙，能帮你快速定位到代码块中的上下文，突出显示，彩虹括号。

使用：

1、Ctrl+右键单击，高亮显示所选代码块



2、Alt+右键单击，其他全部为灰色，突出显示选中代码块



更多使用可以参考 github 地址：https://github.com/izhangzhihao/intellij-rainbow-brackets

**6、Json Helper**

该插件提供了一个易于使用的工具窗口，可以直接在您的IDE中执行JSON字符串操作，不用再打开网站格式化JSON啦，该插件提供了如下功能：

美化您的丑陋json

丑化你漂亮的json

转义你的json

解除转义json

支持JMES json路径搜索。请参阅此处的示例：https://jmespath.org/

对变量声明解析的实验支持。例如public final String json = "{"key":"value"}";变成原始的美化json

Json检查允许嵌套json。也适用于JSON临时文件


**7、SequenceDiagram**

SequenceDiagram 插件可以根据代码调用链路自动生成时序图，这对梳理工作中的业务代码有很大的帮助，堪称神器，暴赞！




TIP：双击顶部的类名可以跳转到对应类的源码中，双击调用的方法名可以直接跳入指定方法的源码中

**8、Alibaba Java Coding Guidelines 和 SonarLint**

1)、Alibaba Java Coding Guidelines

阿里巴巴代码规范约束插件，对代码规范等很有帮助，可以养成良好的代码规范，编程风格

扫描整个项目：



扫描代码后，将不符合规约的代码按 Blocker(崩溃)、Critical(严重)/Major(重要) 三个等级显示在下方，双击可以定位至代码处，右侧窗口还有针对代码的批量修复功能。

如果觉得扫描整个项目太浪费时间且影响性可以能扫描单个文件：



TIP：阿里编码规约扫描，默认是开启实时监测的，此功能可能会引起 IDEA 卡顿，可以点击 关闭实时检测功能 将其关闭，在编码完成后再主动扫描文件。

2)、SonarLint

SonarLint 是一个免费的IDE扩展，允许您在编写代码时修复错误和漏洞！与拼写检查器一样，SonarLint会动态地突出显示代码问题，并提供明确的修复指导，以便在代码提交之前修复这些问题。在流行的IDEs（Eclipse, IntelliJ, Visual Studio, VS Code）和流行的编程语言，SonarLint 帮助所有开发人员编写更好、更安全的代码！



区别：
这两款插件的侧重点不同：
AlibabaJavaCodingGuidelines 插件比较关心的是代码规范，编码风格上的，例如，命名规范，注释，代码行数等

SonarLint 插件比较关心代码正确性，存在的问题，风险，漏洞等，例如，重复代码，空指针，安全漏洞等
使用 AlibabaJavaCodingGuidelines 插件来规范代码，使用 SonarLint 来提前发现代码问题，配合起来提高工程整体的代码质量，并且能够在编码阶段规避风险，提高程序的健壮性。

**9、Translation**

一款翻译插件，再也不用切换窗口到浏览器或翻译软件中搜索了，也可以通过 TranslateandReplace 汉字翻译为驼峰命名的英语，在定义方法名或属性变量时很方便。




IDEA 插件仓库中还有很多优秀的插件，没有最好的只有更适合的，其他插件慢慢探索吧。

© 著作权归作者所有,转载或内容合作请联系作者