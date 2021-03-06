# PSD 交付规范

- pubdate: 2013-6-18 15:48:51

----------------

> 前端在做页面时，需要从设计师的 UI 文件中切图。为了使我们工作协作更加顺畅和高效，这里提出一些建议。
>
> 有些时候，设计师一个小小的改进，会给我们前端带来极大的方便。

## 最重要

1. 忠实原型 PRD 和交互设计，有问题随时沟通，可以创新，但是不可以背离；不然大家都要返工了，呜呜呜~~~
2. 设计师、前端、后端可以一起讨论下模块的命名约定，前端容易理解设计师的产出，后端容易理解前端的产出，然后大家就一致啦。


## 分组规范

好处：

1. 一目了然，方便自己拖动重用，提高效率；
2. 易于维护方便后期设计稿修改；
3. 方便前端切图；

建议：

1. 合理分组，避免不同模块的图层混杂
    - 按模块划分
    - 按效果划分
2. 合理命名
    - 以前端规范为范本，扩展出设计稿分组规范
3. 删除无用的图层，以减小文件体积
    - “过程”图层
    - 废弃图层

范例：

    topbar 顶部工具条
    header 头部
        logo
        nav
    banner
        login-panel
        slide
    content 主区域
        main
            publisher
            blog-recomand
            feed-list
                feed-item01
                feed-item02
                feed-item03
        aside
            search
            menu
            about
    footer 尾部
    document 存放背景效果图
    背景 唯一一个顶级图层，透明背景


## 字体图层

要点：

1. 防止特殊字体变形
2. 图层栅格化

建议：

1. 文案可能会变化的字体图层，请提供相关字体文件；
2. 文案不变的字体图层，请进行栅格化（或提供相关字体文件）；
3. 多个图层达到特殊文字效果的，可以考虑合并图层（如果不宜合并，可以考虑划分为单一的图层分组）。

## 状态图层/分组

1. 如果有的页面组件有多种状态（如按钮），请注明；
2. 状态图层/分组，命名统一约定；

## 样式表

1. 图标尺寸的一致性，如16\*16, 32\*32, 64\*64等等；
2. 字体，字号的一致性；
3. 页面配色的说明；

## 边界值考虑

1. 比如如果没有内容怎么显示？ 如果文字太多怎么显示等等；
2. 多和需求分析师、交互设计师沟通，甚至前端工程师；

## 复杂效果的运用

1. 比如图案混合等高级效果，如果图案混合的两个图层是一个整体，那么可以用；如果不是一个整体，最好不用，因为可能造成切图的困难。