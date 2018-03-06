# 基于Sass的CSS基础库
##### 20180110（宜破旧立新）：
```
再平庸不过的人都会因为摧毁了某样东西而变得强大

            --《苔蕾丝•德斯盖鲁》费朗索瓦•莫利亚克
```

## Usage - 使用

前提条件：项目配置了SASS

在项目存放公用资源目录下`git clone`

```
git clone git@github.com:careteenL/careteen-common-ui.git
```
随后
```
// 先在项目入口处 加入 normalize.scss ，里面包括 global 和 reset
require('公用资源目录/careteen-common-ui/normalize.scss')

// 然后再在需要使用可复用的css代码片段的 scss 文件中 import util.scss
@import '公用资源目录/careteen-common-ui/util.scss'

```
你项目的所有图片资源可放置在 `img` 目录下统一管理

引入`util.scss` 后通过 `@include bg('img_name.png')` 即可使用图片作为背景

** 注意： **

- 可将你当前项目的 字体、字体大小、颜色、z-index等统一的风格 在`core/_base.scss`中修改
- 若有可复用的CSS代码片段，可在`core/_mixin.scss`文件中加入
- 提交代码前在`公用资源目录/careteen-common-ui/`目录下删除`.git`文件，否则无法生效

## Core - 核心文件

- `normalize.scss`      (入口文件，引入_global和_reset文件)
- `util.scss`           (工具文件，引入_base和_mixin文件)
- `_global.scss`        (全局样式)
- `_reset.scss`         (样式归零)
- `_base.scss`          (基础变量：常用颜色、字体...)
- `_mixin.scss`         (功能样式，包括：mixin(混合)、%(placeholder选择器)、function(函数) 、media(媒体查询)几大部分)

## Else - 其他
- 刚进入工作初期，每次切图时都会翻开曾经做过的项目或某个页面开始Ctrl C && Ctrl V ，若是遗漏还可能带来一定的debug成本，使得自己工作效率不高。
- 其实切图时，很多样式片段都能复用。从开始工作到现在，积累了一些公用的样式片段，以语义化的方式命名，可传参使用，避免翻箱倒柜复制粘贴。提高开发效率。
- 我将持续完善本css基础库。一方面记录在切图时遇到的问题，另一方面将自己的一些想法和大家分享，若有不恰当之处、或更优处理方案，还请指出，一起讨论，互相学习成长。
