# 基于Sass的CSS基础库
##### 20180110（宜破旧立新）：
```
再平庸不过的人都会因为摧毁了某样东西而变得强大

            --《苔蕾丝•德斯盖鲁》费朗索瓦•莫利亚克
```

## Usage - 使用
- 前提条件：项目配置了SASS
- 在你项目根目录clone当前项目

```
git clone git@github.com:careteenL/careteen-common-ui.git
```
可在你项目 global.css/scss 文件中import main.scss
```
@import ./careteen-common-ui/main.scss
```
## Core - 核心文件
- main.scss      (入口文件，引入所有scss文件)
- global.scss    (全局样式)
- _reset.scss    (样式归零)
- _base.scss     (基础变量：常用颜色、字体...)
- _mixin.scss    (功能样式，包括：mixin(混合)、%(placeholder选择器)、function(函数) 三个部分)

## Else - 其他
- 刚进入工作初期，每次切图时都会翻开曾经做过的项目或某个页面开始Ctrl C && Ctrl V ，若是遗漏还可能带来一定的debug成本，使得自己工作效率不高。
- 其实切图时，很多样式片段都能复用。从开始工作到现在，积累了一些公用的样式片段，以语义化的方式命名，可传参使用，避免翻箱倒柜复制粘贴。提高开发效率。
- 我将持续完善本css基础库。一方面记录在切图时遇到的问题，另一方面将自己的一些想法和大家分享，若有不恰当之处、或更优处理方案，还请指出，一起讨论，互相学习成长。
