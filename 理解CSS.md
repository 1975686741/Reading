### CSS是什么？
- Cascading Style Sheets
- 用来定义页面元素的样式
   - 设置字体和颜色
   - 设置位置和大小
   - 添加动画效果

### CSS是如何工作的？

![QQ截图20230117235027.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/0751c9402cfc4a659e699a89f8f4d567~tplv-k3u1fbpfcp-watermark.image?)
### 选择器
- 找出页面中的元素，以便给他们设置样式
- 使用多种方式选择元素
    - 按照标签名、类名或id
    - 按照属性
    - 按照DOM树中的位置
- **基本选择器：**
    -   标签选择器：针对**一类**标签
            -   ```
                p{ font-size:14px; }
                ```
    -   ID 选择器：针对某**一个**特定的标签使用， 规定用`#`来定义
            -   ```
                #mytitle{ border:3px dashed green; }
                ```
    -   类选择器：针对**你想要的所有**标签使用， 规定用圆点`.`来定义
            -   ```
                .one{ width:800px; }
                ```
    -   通用选择器（通配符）：通配符`*`：匹配任何标签
            -   ```
            * {
            margin-left: 0px;
            margin-top: 0px;
            }
                ```
 ### 组合
 
**直接组合**
AB
满足A同时满足B
示例：input:focus

**后代组合**
AR
选中B，如果它是A的子孙
示例：nav a

**亲子组合**
A> B
选中B，如果它是A的子元素
示例：section> p

**兄弟选择器**
A~ B
选中B，如果它在A后且和A同级
示例：h2~ p

**相邻选择器**
A+ B
选中B，如果它紧跟在A后面
示例：h2+p

### 颜色
RGB HSL RGBA（Alpha透明度）
### 字体 font-family
使用Web Fonts

```<style>
@font-face {
font-family; " NMegrim " ;
src :
url(https://fonts.gstatic.com/s/megrim/v1
1/46kulbz5WjvLqJZVam_hVUdI1w.woff2)
format('woff2');
}
h1 {
font-family: Megrim, Curs ive;
}
</style>

```

### 行高 line-height
句子之间的距离
###  white-space
-   `normal`

    连续的空白符会被合并，换行符会被当作空白符来处理。换行在填充「行框盒子 ([line boxes](https://www.w3.org/TR/CSS2/visuren.html#inline-formatting))」时是必要。

-   `nowrap`

    和 normal 一样，连续的空白符会被合并。但文本内的换行无效。

-   `pre`

    连续的空白符会被保留。在遇到换行符或者[`<br>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/br)元素时才会换行。

-   `pre-wrap`

    连续的空白符会被保留。在遇到换行符或者[`<br>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/br)元素，或者需要为了填充「行框盒子 ([line boxes](https://www.w3.org/TR/CSS2/visuren.html#inline-formatting))」时才会换行。

-   `pre-line`

    连续的空白符会被合并。在遇到换行符或者[`<br>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/br)元素，或者需要为了填充「行框盒子 ([line boxes](https://www.w3.org/TR/CSS2/visuren.html#inline-formatting))」时会换行。

**`break-spaces`** 与 `pre-wrap`的行为相同，除了：

-   任何保留的空白序列总是占用空间，包括在行尾。
-   每个保留的空格字符后都存在换行机会，包括空格字符之间。
-   这样保留的空间占用空间而不会挂起，从而影响盒子的固有尺寸（最小内容大小和最大内容大小）。

### CSS调试
- 右键点击页面，选择【检查】
- 使用快捷键
    - ctrl + shift + I  (windows)
    - cmd + opt + I (mac)
