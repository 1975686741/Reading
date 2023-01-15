
### 什么是前端
+ 解决GUI人机交互问题
+ 跨终端
    + PC/移动浏览器
    + 客户端/小程序
    + VR/AR 等
+ Web技术栈

### 前端技术栈

![QQ截图20230115212507.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/3e8a609f9c264438aeda4778f7e44930~tplv-k3u1fbpfcp-watermark.image?)

### 前端应该关注哪些方面
+ 美观
+ 功能
+ 性能
+ 无障碍
+ 安全
+ 兼容

### HTML是什么
HyperText(图片、标题、链接、表格等) Markup Language，是一种[标记语言](https://baike.baidu.com/item/%E6%A0%87%E8%AE%B0%E8%AF%AD%E8%A8%80/5964436?fromModule=lemma_inlink)。它包括一系列[标签](https://baike.baidu.com/item/%E6%A0%87%E7%AD%BE/2440469?fromModule=lemma_inlink)．通过这些标签可以将网络上的[文档](https://baike.baidu.com/item/%E6%96%87%E6%A1%A3/1009768?fromModule=lemma_inlink)格式统一，使分散的[Internet](https://baike.baidu.com/item/Internet/272794?fromModule=lemma_inlink)资源连接为一个逻辑整体。HTML文本是由HTML命令组成的描述性[文本](https://baike.baidu.com/item/%E6%96%87%E6%9C%AC/5443630?fromModule=lemma_inlink)，HTML命令可以说明[文字](https://baike.baidu.com/item/%E6%96%87%E5%AD%97/612910?fromModule=lemma_inlink)，[图形](https://baike.baidu.com/item/%E5%9B%BE%E5%BD%A2/773307?fromModule=lemma_inlink)、[动画](https://baike.baidu.com/item/%E5%8A%A8%E7%94%BB/206564?fromModule=lemma_inlink)、[声音](https://baike.baidu.com/item/%E5%A3%B0%E9%9F%B3/33686?fromModule=lemma_inlink)、[表格](https://baike.baidu.com/item/%E8%A1%A8%E6%A0%BC/3371820?fromModule=lemma_inlink)、[链接](https://baike.baidu.com/item/%E9%93%BE%E6%8E%A5/2665501?fromModule=lemma_inlink)等。
### html的语法
+ 标签和属性**不区分大小写，推荐小写**
+ 空标签可以不闭合，比如input、meta
+ 属性值推荐用双引号包裹
+ 某些属性值可以省略，比如required、 readonly


##### 浏览器在拿到html之后会把html代码进行解析，解析出一个DOM树。

### 什么是DOM树？

![QQ截图20230115214250.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/f8a58394806745efbf81581e6d4cd41c~tplv-k3u1fbpfcp-watermark.image?)
把html的代码转化成对应的树形结构，里面对应的每个节点称之为DOM节点。
### html的常用标签
**标题：** `h1></h1>` ~ `<h6></h6>`,用于表示文档的各级标题，级数越大字体大小越小。  
**列表**：`<ol><li>...</li></ol>`，有序列表。  
`<ul><li>...</li></ul>`，无序列表。  
`<dl><dt>...</dt><dd>...</dd></dl>`，描述列表。  
**链接**：`<a></a>`，href属性：链接到的地址；target属性：跳转页面的方式，如：`_blank`为在新页面打开该网页、`_self`为在当前页面打开该网页。  
**图片**：`<img>`，`src`属性：图片的地址，`alt`属性：当图片未正常加载时显示的文本。该标签可以不闭合。  
**音频**：`<audio></audio>`，`src`属性：音频地址，`controls`属性：是否显示浏览器默认的音频控件。  
**视频**：`<video></video>`，`src`属性：视频地址，`controls`属性：是否显示浏览器默认的视频控件。  
**输入框**：`<input>`，`type`属性：输入框的类型，如`password`会自动将输入的值变成不可见类型。`input`标签具有非常丰富的type类型，可以在[MDN](https://link.juejin.cn?target=https%3A%2F%2Fdeveloper.mozilla.org%2Fzh-CN%2Fdocs%2FWeb%2FHTML%2FElement%2FInput "https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/Input")上查询。该标签可以不闭合。  
**数据列表**：`<datalist><option>...</option></datalist>`，一般通过`id`属性绑定拥有`list`属性的`input`输入框使用，`option`中的内容作为该`input`输入框提示信息。`option`在父元素中只存在这种标签时可以不闭合。  
**文本框**：`<textarea></textarea>`,允许调整大小并输入多行文字的输入框。  
**下拉选项框**：`<select><option>...</option></select>`，`option`为下拉框的选项内容。  
**引用**：
-   `<cite></cite>`，短引用。  
-   `<q></q>`，短引用。`q`区别于`cite`，会将包裹的文本用双引号引用，而`cite`则是显示成斜体。  
-   `<code></code>`，将文本以代码的样式引用。  
-   `<blockquote></blockquote>`，块级引用，可以引用多行文本。`cite`属性：引用文本的地址。  
-   `<pre></pre>`，包裹的文本将保留空白符，并用源格式在浏览器页面中显示出来。
-   `<strong></strong>`，加粗包裹的文本，强调文本重要性。
-   `<em></em>`，将包裹的文本变成斜体，表示强调。  
**内容划分**

![QQ截图20230115213658.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/ff2cba05c0a04813a3e026c24d3036d4~tplv-k3u1fbpfcp-watermark.image?)
### 语义化是什么
+ HTML中的**元素、属性及属性值**都拥有某些含义
+ 开发者应该遵循**语义**来编写HTML
+ 有序列表用ol：无序列表用ul
+ lang 属性表示内容所使用的语言

### 如何做到语义化
- 了解每个标签和属性的含义
- 思考什么标签最适合描述这个内容
- 不使用可视化工具生成代码
### 个人思考与总结
通过这节课的学习，对于前端的认识更近一步，同时也对HTML的知识和HTML的语义化也有了更深的理解，html是向用户传达内容而不是样式，是一种结构层；同时也明白了，日后我们在进行软件开发时，语义化的重要性，使得我的基础更加牢固了，收益颇丰！
