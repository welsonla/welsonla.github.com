---
title: Learning-figma-day-2 自定义样式与组件
date: 2022-12-10 17:02:15
categories: Design
keywords: figma
tags:
- design
- figma
- study
---

只是记录一下学习Figma过程中的一些笔记，可能会有更多更方便的使用技巧。

### 本地样式


#### 添加本地样式
在Figma 中不论是字体、颜色、样式等都可以添加为自定义的样式，操作步骤如下

点击属性右上的图标，弹出窗口中点击`+`按钮即可

![](/uploads/figma-local-style@2x.png)

#### 使用本地样式

之后我们再次点击此处就可以看到我们添加到自定义样式, 右侧的调整按钮是我们可以对保存的本地样式进行调整，这样调整后的样式会将使用该样式的元素同步进行更新，比如统一修改App的导航栏颜色、Tabbar的选中颜色等

![](/uploads/figma-local-style-list.png)


#### 取消样式关联
如果我们使用了本地样式，但是想自己对该样式进行单独的修改, 如应用了阴影等设置，但是想单独调整下阴影的大小，则点击该样式右侧的断开链接图标即可

![](/uploads/figma-local-style-unlink.png)

#### 本地样式列表
本地样式在我们鼠标单击空白处会在右侧的属性栏中进行显示，我们可以直接在此处对本地样式进行修改与删除，假如我们需要对设计统一修改色调就可以直接修改某一个本地样式
![](/uploads/figma-local-styles-list.png)


### 本地组件

本地组件是为了更好的复用与批量修改，比如我们的新闻列表，每个条目的标题与简介、缩略图都是统一的，我们就可以做一个条目的组件来统一管理他们的样式，假如我们更新的标题的字号与颜色，所有使用到该组件的地方都会进行同步的修改，这样节省了我们每个都去单独修改的时间，也更方便让相同设计元素进行复用，降低设计更新的时间成本。


一般我们在一个设计稿中将所有的组件都放在同一个Frame中集中管理，不要在页面中创建组件，这样会在后期查找父组件比较费力，我们将一个设计稿中的本地组件都放置在同一个Frame中，这样不仅方便查找，而且比较清晰。


创建组件的快捷键为`Opt + CMD + K`, 也可以选中你的元素后，点击顶部的创建组件按钮

![](/uploads/figma-create-component.png)

创建完毕组件之后，我们就可以按住`Opt`+拖动组件快速使用一个组件，多次复制之后，我们就能快速的完成一个新闻列表样式，我们可以单独对每个子组件的标题与描述进行修改，而不会影响父组件

![](/uploads/figma-component-list.png)

当我们对父组件的属性进行修改时，子组件也会同步的更新样式, 可能这就是设计中的面向对象概念吧

![](/uploads/figma-component-update.png)

#### 父组件与子组件概念
父组件与子组件的特点总结(不全面):
- 更新父组件会同步将样式同步给使用到的子组件
- 子组件可以单独更新自己的文本、高度，而不会影响父组件
- 子组件如果想单独更新组件某些样式，可以同样断开链接之后进行单独的修改，方法同本地样式



#### 本地库

本地样式与本地组件都会显示在本地资源库中，位置在Layers右侧的Assets栏目中, 从图中可以看到，我们将所有的组件放置在同一个Frame中的优势也显示出来了，这样就不会去多个页面下去寻找定义的组件，也节省了一部分的时间,本地库中的组件，我们可以直接拖动到设计页面中进行使用。

![](/uploads/figma-assets.png)