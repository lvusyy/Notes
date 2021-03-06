# UML 笔记

## 一：概述：UML是什么

UML是一种统一建模语言。可以用于项目设计过程的可视化。

是用于制造软件蓝图的图片语言，描述的是一个实时系统

> 什么是建模：建模就是把现实中的使建立一个模型，使人能够接受，能够理解
>
> 比如说地图，地址就是一种导向模型，地图上有很多图标，线，分别代表各种含义

## 二：UML的规范

有四个部分

1. 定义图标和元素符号以及符号的含义的上层结构
2. 定义上层建筑基于的核心元模型的基础设施
3. 定义模型元素规则的OCL语言
4. The UML Diagram Interchange that defines how UML 2 diagram layouts are exchanged

## 三：UML的元素

UML提供了可视化系统架构蓝图的方法，其中包含以下元素

1. 所有活动（工作）
2. 系统的各个组件
   1. 以及他们如何跟其他软件组件交互
3. 系统怎么运行
4. 实体如何与其他交互（组件和接口）
5. 外部用户界面



## 四：UMl的概念模型
为了了解什么是UML的概念模型，首先我们要知道什么叫做概念模型，以及它有什么用？

概念模型： 一个概念模型可以定义为由概念和关系构成的模型
绘制UML图之前，第一步要做的事就是创建一个概念模型，它有助于了解现实中的实体以及他们是如何相互作用的

软件的需求分析后，就得到了一个模型，这个模型就是概念模型

如何学习UML概念模型？
UML的概念模型可以学习以下三个主要元素来掌握
1. UML构建块（building blocks）
2. 用规则来连接构建块
3. UML的常用机制

## 五：面向对象的概念
UML可以被描述为面向对象分析和设计的接班人（嗯？就是面向对象的继承人吧，大概。。）
一个对象包含数据和控制数据的方法
数据表示对象的状态
一个类描述一个对象，这些类也形成一个层次结构以用来模拟现实世界的系统
>层次表现为继承，也就是说，类与类之间通过继承来形成各种层次关系，用来模拟现实世界的系统
> 并且类也可以按照需求以不同的方式关联

### 5.1 对象
对象是存在我们现实中的实体，面向对象中的抽象、继承、封装、多态都可以用UMl图来表示
UML很厉害的，可以表示面向对象分析和设计中的存在的所有概念，因此，在学习UML图之前，了解一下面向对象的概念是非常有必要的
以下是面向对象世界的一些基本概念（纯当复习的说）
1. 对象(Object)：对象表示一个实体和一个基本building block(构建块)
2. 类（class）：类是一个对象的蓝图
3. 抽象(Abstraction): 抽象表示一个真实世界的实体的行为
4. 封装：封装是把数据绑定在一起并将其从外界隐藏的一种机制
5. 继承：继承是从现有的类创建新类的一种机制
6. 多态：多态定义了类以不同形式存在的机制

### 5.2 OO的分析和设计
OO可以定义为调查对象,设计意味着识别对象的协作
OO分析最重要的目的就是识别要设计的系统的对象，这个分析也可以用于已完成的系统。
只有当我们能够识别系统中的对象时，才有可能进行有效的分析
在识别对象之后，理清它们之间的关系并最终产生设计

OO分析的设计的目的可以总结如下
1. 识别系统中的对象
2. 理清对象之间的关系
3. 使用OO语言，制作一个可执行的设计文件

### 5.3 OO的应用和实施
有三个基本步骤
OO Analysis → OO Design → OO implementation using OO languages
详细描述的话，大概是酱紫
1. 在OO分析中，最重要的就是识别对象并以适当的方式描述他们。
   如果这个过程很容易，那么下一个工作-设计就会很简单
   这个对象应该确定它的责任，责任就是对象执行的功能，每一个对象都有一些类型的责任来执行
   当这些责任联合起来时，系统的目的就可以得以实现
2. 接下来就是OO的设计，在这个阶段中，重点放在要求和实习上。
    在这个阶段，对象是根据他们预期的联系来合作的，合作完成，设计也就是完成了
    （也就是说，在这个阶段，要负责对象和对象之间，是怎么协作的，要想明白这一点）
3. 第三个阶段就是实施，在这个阶段，设计主要是通过面向对象的语言来实现的
   比如说JAVA，C++

### 5.4 UML在OO设计中的作用
UML图中的类图，对象图，协作图，交互图，都是基于对象来设计的
因此，OO设计和UML就是拴在同一根绳子上的蚂蚱。
而且呢，UML的输入其实就是OO的分析和设计



## 六：快速开始

以骰子为例

确定问题领域（我们要干什么）

> 软件模拟游戏者投两个骰子，如果总点数是7则win，否则输

用例（这个软件是如何运行的，举个运行的例子）

1. 游戏者请求骰子
2. 系统展示结果，7则win，否则die

定义领域模型（业务模型）

> 最重要的是识别问题中的概念 ,在骰子游戏中，有游戏者，骰子，骰子游戏这几个概念，这几个概念中的联系

对象的定义-职责和协作







## 六 Building Blocks（构建块）
本章节主要讲building blocks。它可以被定义为
1. Things(事)
2. 关系
3. 图表

### 6.1 Things(事)
Things是UML构建块中非常重要的部分，它可以是
1. 结构(Structurl)
2. 行为（Behavioral）
3. 分组
4. 注释

#### 6.2 Structurl

Structurl 定义了模型的静态部分，它代表了物理还有概念元素，以下是对Structurl的简要描述

1. Class Class代表了代表一组具有相似职责的对象![图示](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/class_structurl_things.jpg>)
2. Interface Interface定义了一组操作，它们指定了一个类的责任![图示](https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/interface_structural_things.jpg)
3. Collaboration Collaboration定义了元素之间的协作![图示](https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_collaboration.jpg)
4. Use case UseCase代表了系统针对特定目标而执行的一系列操作![图示](https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_usecase.jpg)
5. Component  Component代表了系统的物理部分![图](https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_component.jpg)
6. Node 一个Node可以定义为运行中存在的物理元素![图](https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_node.jpg)

#### 6.3 Behavioral

一个Behavioral thing 由模型的动态部分组成，下面这些就是Behavioral thing 

1. **Interaction(相互作用) ** Interaction 被定义为一种行为，由一组信息在元素中的交换以完成特定的任![图片](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_message.jpg>)

2. state machine  state mechine在对生命周期中的对象状态非常有用![state machine](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_state.jpg>)

   它定义了对象经过事件响应过程中的状态变化，而事件是造成对象状态变化的重要因素

#### 6.4 Grouping

Grouping Of Things可以被定义为将UML模型中的元素组合在一起的机制，这样的话只有一个分组可用

Grouping things 

>  特别的：package :package是唯一可以用于搜集结构和行为的Grouping things 
>
>  ![package](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_package.jpg>)

#### 6.5 Annotational Things

Annotational things可以被定义备注，描述，和UML模型元素中的注释

![note](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_note.jpg>)

### 7.1：Relationship（关系）

Relationship 是UML一个重要的组成部分，它显示了元素是如何关联的，这个关联描述了应用程序的功能

有四个关系可用

1. Dependency(依赖)

   依赖是两个元素之间的关系，其中一个元素的变化也会影响到另一个元素![依赖](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_dependency.jpg>)

2. Association(关联)

   关联也是描述两个元素之间的关系，不过这种联系比较弱![association](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_association.jpg>)

3. Generalization(概括，泛化)

   Generalization基本定义了广义元素和特定元素之间的关系，它基本描述了对象世界的继承关系![generaliztion](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_generalization.jpg>)

4. Realization(实现)

   实现可以被定义为两个元素之间的关系，其中一个元素描绘了一些责任，没有被执行

   另一个元素则被执行，这种关系存在于接口的情况下![realization](<https://raw.githubusercontent.com/XHang/Notes/master/src/main/resources/UMLPicture/uml_realization.jpg>)

### 8.1 UML图表分类

   UML是这篇文章讨论的最终结果

   所有的元素和关系都用来做一个完整的UML图，整个图表示系统

   UML包括九个图表，这将在下面的几个章节来介绍它

   1. Class diagram 类图
   2. Object diagram 对象图 
   3. Use case diagram
   4. Sequence diagram 序列图
   5. Collaboration diagram 协作图
   6. Activity  diagram 活动图
   7. Statechart  diagram 状态图
   8. Deployment diagram 部署图
   9. Component diagram 组件图

   ## 第七章： UML的体系结构
   在设计系统之前，架构的设计要考虑不同观点。
   这些观点可以是
   1. 设计
   2. 实现
   3. 处理
   4. 部署

   这些观点通过用例图连接起来。用例代表了系统的功能

   因此，这些观点和用例有关

   1. 设计：一个系统由类和接口协作完成，UML提供了类图和对象图来支持这一点

   2. 实现：组装在一起的组件可以实现一个完整的物理系统

      UML通过组件图可以支持这一点

   3. 过程：定义了系统的流程，在UML中，可以通过使用相同的元素来支持这一个观点

   4. 部署代表构成系统的硬件的物理节点。

      UML通过部署图来支持这个观点

   ## 八：UML建模类型

   区分不同的UML模型是至关重要的

   不同的模型用于不同的UML建模。有三种不同的UML建模类型

   ### 8.1 结构建模

   ​结构建模捕捉系统的静态部分。它们包含以下内容

1. 类图
2. 对象图
3. 部署图
4. 

   ​

   ​

