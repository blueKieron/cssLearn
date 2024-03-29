## bfc（**Block Formatting Context**）
> 实现bfc方法
> 1.**body根元素**
> 2.**设置浮动，不包括none**
> 3.**设置定位，absoulte或者fixed**
> 4.**行内块显示模式，inline-block**
> 5.**设置overflow，即hidden，auto，scroll**
> 6.**表格单元格，table-cell**
> 7.**弹性布局，flex**

## 相对单位大小
> |单位|相对于|
> |---|---|
> |`em`|在 font-size 中使用是相对于父元素的字体大小，在其他属性中使用是相对于自身的字体大小，如 width|
> |`ex`|字符“x”的高度|
> |`ch`|数字“0”的宽度|
> |`rem`|根元素的字体大小|
> |`lh`|元素的 line-height|
> |`vw`|视窗宽度的 1%|
> |`vh`|视窗高度的 1%|
> |`vmin`|视窗尺寸的 1%|
> |`vmax`|视图寸的 1%||

> *percent: 如果将元素的字体大小设置为百分比，那么它将是元素父元素字体大小的百分比。如果使用百分比作为宽度值，那么它将是父值宽度的百分比*
> *使用百分比作为元素外边距（margin）或填充（padding）的单位时，值是以包含块的**内联尺寸**进行计算的，也就是元素的水平宽度。在我们的示例中，所有的外边距或填充都是宽度的 10%。请记住一个事实，当你使用百分比作为元素外边距或填充的单位时，你将得到一个相同尺寸的外边距或填充。*

> 当使用 `object-fit` 时，替换元素可以以多种方式被调整到合乎盒子的大小。*cover fill contain*
> 在对替换元素使用各种 CSS 布局时，你可能会发现他们的表现方式与其他元素有一些细节上的差异。例如，flex 或者 grid 布局中，默认情况下元素会被拉伸到充满整块区域。但是
 图像不会被拉伸，而会对齐到网格区域或者弹性容器的起始处。
>  为了强制图像拉伸，以充满其所在的网格单元，你必须做类似于下面的事情：
>  ``` css
> img {
>  width: 100%;
>  height: 100%;
>}
>  ```

## css原生变量
> ```  css
>  :root {
>     --main-bg-color: brown;
>  }
>  ```
>  ```
>  .five {
>      background-color: var(--main-bg-color);
>   }
>  ```

## 特性查询
> 特性查询允许你测试一个浏览器是否支持任何特定的一个 CSS 特性。这就是说，你可以写一些面向不支持某项特性的浏览  器的 CSS，然后检查以了解浏览器是否支持，如果支持的话就可以加进你的复杂布局了。
> ``` css
> @supports (display: grid) {
>  .item {
>      width: auto;
>   }
> }
> ```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcyODY1ODgyOSwtMTQzMTA2MDAxMywzND
U3Njk2MzcsLTY0OTQxOTA1Myw1NDQwNTc4NTMsMTM0MzE0NzE5
NSwtMTU3OTI3ODQxNywxMjU5NTM2NzVdfQ==
-->