[TOC]





# 开发工具

### 大前端

* 网页

* 小程序

* 数据可视化

* 服务器

* 客户端

### 应用软件

* **C / S 架构**：

客户端服务器

可安装 可不安装的

利弊：需要安装/偶尔更新/不跨平台

​			但是大型专业应用，安全性要求较高的应用需要采用

* **B / S 架构**：  需要打开网站的

浏览器服务器

利弊：无需安装/无需更新/可跨平台

### 浏览器

* 五大主流浏览器

​		chrome	Safari	IE	Firefox	Opera

* 浏览器的内核

  内核是浏览器的核心，用于处理浏览器所得到的各种资源

  服务器 ---代码--->浏览器（处理）----->页面

* 五大浏览器 四大内核

 	 chrome ：早期使用 webkit 内核，现在用 Blink 内核
 	
 	Safari ：使用webkit 内核

​		IE：使用 Trident内核

​		Firefox：使用 Gecko 内核

​		Opera ：早期使用Presto内核（已放弃） ，现在使用 Blink 内核

### VS Code

**Visual Studio Code**（简称 **VS Code**）是一款由[微软](https://zh.wikipedia.org/wiki/微软)开发且跨平台的[免费](https://zh.wikipedia.org/wiki/免費軟體)[源代码编辑器](https://zh.wikipedia.org/wiki/集成开发环境)[[7\]](https://zh.wikipedia.org/wiki/Visual_S						l0pp0 tudio_Code#cite_note-TechCrunch-7)。该软件以扩展的方式支持[语法高亮](https://zh.wikipedia.org/wiki/語法高亮)、代码自动补全（又称 [IntelliSense](https://zh.wikipedia.org/w/index.php?title=IntelliSense&action=edit&redlink=1)）、[代码重构](https://zh.wikipedia.org/wiki/代码重构)功能，并且内置了[命令行](https://zh.wikipedia.org/wiki/命令行)工具和 [Git](https://zh.wikipedia.org/wiki/Git) 版本控制系统[[8\]](https://zh.wikipedia.org/wiki/Visual_Studio_Code#cite_note-8)。用户可以更改主题和键盘快捷方式实现个性化设置，也可以通过内置的[扩展程序](https://zh.wikipedia.org/wiki/插件)商店安装其他扩展以拓展软件功能。



#### 常用开发插件&设置

- 软件汉化插件：Chinese
- 打开网页插件：Open in browser
- 实时刷新插件：Live server
- 彩色缩进插件：Indent-rainbow
- 英语翻译插件：Code translate
- 格式化程序设置：Format on save
- 自动同步修改标签插件：Auto Rename Tag







# HTML

### 常用标签



#### 无语义布局标签

作用：布局网页，划分网页区域，摆放内容

- `div` :独占一行，大盒子
- `span` :不换行，小盒子

> 两个标签都是双标签，其中包裹的内容可以是任何内容



####  语义化标签

简单来说

头部用 **header**

页脚用 **footer**

导航用 **nav**

侧边栏用 **aside**

独立成段类似文章 帖子 评论用 **article**

文章中的各个次级段落用 **section**

解释一下 一个**article**中有多个**section**，甚至由**section**组成

**section**强调分段或分块或分成自然段

**article**比section**更加强调独立性**，一块内容是独立的、完整的，应当使用**article**

***大概article是文章 section是章节***



| **标签名称**   | **用途描述**                                         | **示例用法**                                                 | **优点/特点**                                        |
| -------------- | ---------------------------------------------------- | ------------------------------------------------------------ | ---------------------------------------------------- |
| `<header>`     | 定义文档或节的页眉，通常包含标题、导航等。           | ```html<br><header><h1>网站标题</h1><nav>导航链接</nav></header>``` | 提高页面结构清晰度，增强SEO和可访问性。              |
| `<footer>`     | 定义文档或节的页脚，通常包含版权信息、联系方式等。   | ```html<br><footer>© 2025 公司名称</footer>```               | 明确页面底部内容，便于屏幕阅读器解析。               |
| `<nav>`        | 定义导航链接部分，如主导航菜单。                     | ```html<br><nav><a href="#home">首页</a></nav>```            | 标识核心导航区域，提升用户体验和SEO。                |
| `<section>`    | 定义文档中的独立区域，通常带有标题。                 | ```html<br><section><h2>章节标题</h2><p>章节内容</p></section>``` | 结构化内容分段，便于组织和样式设计。                 |
| `<article>`    | 定义独立、完整的内容块（如博客文章、新闻）。         | ```html<br><article><h2>文章标题</h2><p>文章内容</p></article>``` | 独立内容模块化，利于内容重用和SEO优化。              |
| `<aside>`      | 定义与主内容相关但不直接关联的辅助内容（如侧边栏）。 | ```html<br><aside><h3>相关链接</h3><ul>链接列表</ul></aside>``` | 区分主次内容，提升页面可读性和可访问性。             |
| `<main>`       | 定义文档的主要内容区域（页面只能有一个）。           | ```html<br><main><article>核心内容</article></main>```       | 标识核心内容，便于屏幕阅读器和搜索引擎快速定位重点。 |
| `<figure>`     | 定义独立的流内容（如图片、图表、代码片段）。         | ```html<br><figure><img src="image.jpg"><figcaption>图片说明</figcaption></figure>``` | 将视觉元素与其描述绑定，提升内容的语义化。           |
| `<figcaption>` | 为`<figure>`元素提供标题或描述。                     | ```html<br><figcaption>图1: 示例图片</figcaption>```         | 增强`<figure>`内容的可访问性和上下文信息。           |
| `<mark>`       | 高亮显示文本内容（默认黄色背景）。                   | ```html<br><mark>关键词</mark>```                            | 突出显示重要信息，适用于搜索结果高亮。               |
| `<time>`       | 定义日期或时间（通过`datetime`属性机器可读）。       | ```html<br><time datetime="2025-05-09">2025年5月9日</time>``` | 提供结构化的日期时间数据，便于机器解析。             |
| `<details>`    | 定义可折叠的用户可切换内容块（如FAQ）。              | ```html<br><details><summary>点击展开</summary>详细内容</details>``` | 实现交互式内容折叠，减少页面冗余。                   |
| `<summary>`    | 为`<details>`元素提供标题或摘要。                    | ```html<br><summary>标题</summary>```                        | 与`<details>`配合使用，提升用户交互体验。            |
| `<dialog>`     | 定义对话框或模态窗口（如弹窗）。                     | ```html<br><dialog open>这是一个对话框</dialog>```           | 简化对话框实现，支持原生交互功能。                   |
| `<progress>`   | 表示任务的进度（如文件上传进度）。                   | ```html<br><progress value="70" max="100">70%</progress>```  | 可视化进度状态，提升用户反馈体验。                   |
| `<meter>`      | 表示标量值或分数（如磁盘使用率）。                   | ```html<br><meter value="0.6" min="0" max="1">60%</meter>``` | 直观展示数值范围，适用于数据可视化场景。             |



#### 图像标签

作用：在网页中插入图片

标签名：`<img src = "图片的URL">`

**`src 属性`**  用于指定图像的位置和名称，是  **`<img>`**  的必须属性

> 图片与代码文件放至同一文件夹即可使用 `./` 命令快捷添加，这种方法是 `相对路径`

**常见属性表**

| 属性   | 作用       | 说明                               |
| ------ | ---------- | ---------------------------------- |
| alt    | 替换文本   | 图片无法显示的时候显示的文字       |
| title  | 提示文本   | 鼠标悬停在图片上面的时候现实的文字 |
| width  | 图片的宽度 | 值为数字，没有单位                 |
| height | 图片的高度 | 值为数字，没有单位                 |

> img标签 中的 alt属性 适用于可能加载失败，进行解释并提示
>
> 分别使用 width属性 与 height属性 浏览器默认是***等比缩放***



#### 音频标签

标签名：`<audio src="音频的URL"></audio>`

**常见属性表**

| 属性                | 作用             | 特殊说明                 |
| ------------------- | ---------------- | ------------------------ |
| **src（必须属性）** | 音频URL          | 支持格式：MP3、Ogg、Wav  |
| controls            | 显示音频控制面板 |                          |
| loop                | 循环播放         |                          |
| autoplay            | 自动播放         | 浏览器一般会禁用自动播放 |

> 在HTML5中，如果属性名与属性值完全一样，则可简写为一个单词



#### 视频标签

标签名：`<video src="视频的URL"></video>`

**常见属性表**

| 属性                | 作用             | 特殊说明                         |
| ------------------- | ---------------- | -------------------------------- |
| **src（必须属性）** | 视频URL          | 支持格式：MP4、WebM、Ogg         |
| controls            | 显示视频控制面板 |                                  |
| loop                | 循环播放         |                                  |
| muted               | 静音播放         |                                  |
| autoplay            | 自动播放         | 浏览器支持在**静音状态**自动播放 |

> 在HTML5中，如果属性名与属性值完全一样，则可简写为一个单词



#### 超链接标签

作用：点击跳转到其他页面

标签名：**`<a href="链接">显示文字</a>`**

`target` 属性赋值 `"_blank"` 可实现新窗口跳转页面

`target` 属性赋值 `"_self"` 可实现当前窗口跳转页面，不用写，默认就是在当前窗口跳转页面

例如：`<a href="https://lufangqian.top" target="_blank">陆方七安的导航</a>`

本示例意为在新窗口打开指向`lufangqian.top`网站的名叫陆方七安的导航的超链接

> 开发初期，不知道超链接的跳转地址，href属性值写#，表示空链接，不会跳转,  可以回到顶部
>
> 如果 href 属性值是空的 ， 表示 刷新页面
>
> 如果 href 属性值是  javascript : js的内容 ;  ， 可以进行进行 js 的操作 
>
> 
>
> 在代码中，敲不管多少的空格，都只显示一个空格
>
> a 标签内，不准再写 a 标签



##### 锚点链接

a标签还可以跳转到特定位置，可以给要跳转到的位置的标签添加一个id，在a标签中给hef的值设置为#id名

```html
<a href="#top">返回顶部</a>

<!-- 在页面的顶部放置一个id为top的元素 -->
<div id="top"></div>
```

去除超链接默认样式

```css
a {
    color: inherit; /* 使用父元素的颜色 */
    text-decoration: none;
}
```

##### 跳转锚点

```html
<!-- 跳转到test1锚点 -->
<a href="#test1">去test1锚点</a>

<!-- 跳到本页面顶部 -->
<a href="#">回到顶部</a>

<!-- 跳转到其他页面锚点 -->
<a href="demo.html#test1">去demo.html页面的test1锚点</a>

<!-- 刷新本页面 -->
<a href="">刷新本页面</a>

<!-- 执行一段js, 如果还不知道执行什么，可以留空，javascript:; -->
<a href="javascript:alert(1);">点我弹窗</a>
```



##### 清楚默认样式

✅ 1. 去除下划线（最常见）

css

深色版本



```
a {
    text-decoration: none; /* 关键：去除下划线 */
}
```

------

✅ 2. 重置颜色

浏览器默认给链接设置颜色（如蓝色、访问后变紫色），可以统一设置：

css

深色版本



```
a {
    color: black;           /* 设置你想要的颜色 */
    color: inherit;         /* 或继承父元素颜色 */
}
```

------

✅ 3. 清除所有状态的默认样式（推荐）

链接有多种状态：未访问、已访问、悬停、点击中。建议统一控制：

css

深色版本



```
a {
    text-decoration: none;  /* 去掉下划线 */
    color: inherit;         /* 颜色继承父元素 */
    outline: none;          /* 去掉点击时的轮廓（谨慎使用） */
    /* outline: none 可能影响可访问性，建议保留或自定义 */
}

/* 可选：自定义悬停效果 */
a:hover {
    text-decoration: none;
    color: #007acc;
    /* 可加其他效果，如背景色 */
}
```

------

✅ 4. 完整“清除样式”示例

css

深色版本



```
a,
a:link,
a:visited,
a:hover,
a:active,
a:focus {
    text-decoration: none;
    color: inherit;
    outline: none;
    border: none;
    background: none;
}
```

> ⚠️ 注意：
>
> - `outline: none` 会移除键盘导航的焦点框，**影响无障碍访问**，不建议完全移除。
> - 更好的做法是自定义 `:focus` 样式：

css

深色版本



```
a:focus {
    outline: 2px solid #007acc;
    outline-offset: 2px;
}
```

------

✅ 5. 如果用于按钮或菜单中的链接

css

深色版本



```
.nav-link {
    text-decoration: none;
    color: white;
    padding: 10px 15px;
    display: inline-block;
}

.nav-link:hover {
    background-color: #007acc;
    border-radius: 4px;
}
```

------

✅ 总结：最常用写法

css

深色版本



```
a {
    text-decoration: none;
    color: inherit;
}

a:hover {
    text-decoration: none; /* 防止某些浏览器恢复下划线 */
}
```

------

🚫 不推荐的做法

- 使用 `underline` 或奇怪颜色不处理
- 完全移除 `outline` 而不提供替代焦点样式（对残障用户不友好）

------

✅ **最佳实践**：
 清除默认样式是为了美观，但要保留**可访问性**和**用户体验**。建议：

- 去掉下划线 ✅
- 统一颜色 ✅
- 自定义 `:hover` 和 `:focus` 效果 ✅





#### 全局标签属性

| 属性名 | 含义                                                         |
| ------ | ------------------------------------------------------------ |
| id     | 给标签指定唯一标识，注意：id 是不能重复的。<br>作用：可以让 label 标签与表单控件相关联；也可以与 CSS、JavaScript 配合使用。<br>注意：不能在以下 HTML 元素中使用：<br>`<head>`、`<html>`、`<meta>`、`<script>`、`<style>`、`<title>`。 |
| class  | 给标签指定类名，随后通过 CSS 就可以给标签设置样式。          |
| style  | 给标签设置 CSS 样式。                                        |
| dir    | 内容的方向，值: ltr、rtl。<br>注意：不能在以下 HTML 元素中使用：<br>`<head>`、`<html>`、`<meta>`、`<script>`、`<style>`、`<title>`。 |
| title  | 给标签设置一个文字提示，一般超链接和图片用得比较多。         |
| lang   | 给标签指定语言，具体规范和可选值请参考【10. HTML 设置语言】。<br>注意：不能在以下 HTML 元素中使用：<br>`<head>`、`<html>`、`<meta>`、`<script>`、`<style>`、`<title>`。 |

标签属性的作用是给标签提供一些附加信息

**注意！！！！！！！！！！重复写同一个属性，后写的属性将覆盖前面的同一属性**

每个标签都有属性 常见的为 class 与 id，经常被用在设置css样式与js行为中



还有三个较为常见且大部分标签皆可使用的属性

**title**(鼠标悬浮文字提示)    **lang**(给指定标签设置语言)   **dir**(内容显示方向，值为**ltr rtl**)



有一些标签有其特殊的属性

例如资源引用相关

- `src`

  （Source）：指定外部资源的路径，用于加载图片、脚本、视频等。

  - 用途：浏览器会直接加载该资源。
  - 示例：`<img src="image.jpg">`、`<script src="script.js"></script>`

- `href`

  （Hypertext Reference）：指定超链接的目标地址。

  - 用途：点击后跳转到其他页面或资源。
  - 示例：`<a href="https://example.com">点击访问</a>`

表单元素相关（如 `<input>`、`<textarea>`）常用属性：

- - **`name`**：提交表单时字段的名称（服务器端用于接收数据）。
  - **`value`**：输入框的默认值或用户输入的内容。
  - **`placeholder`**：输入框的提示文字（未输入时显示）。
  - **`required`**：表示该字段为必填项。



#### 标题标签

一般用于新闻标题、文章标题、网页区域名称、产品名称等等

标签名：`h1 ~ h6`

> 由大到小，h1标题为主标题，标题等级随着数字增大而减小

**注意事项**

- h1 标签在一个网页中建议只使用一次，用来放新闻标题或者网站的logo
- h2 ~ h6 没有使用次数的限制

> 以上两点为规范要求，并非语法要求，如要重复使用，也没啥事

注意，**标题标签之间不可嵌套**



#### 段落标签

一般用在新闻段落、文章段落、产品描述信息等等

标签名：**`p`**

段落标签内的文字会自动换行



#### 换行与水平线标签

换行： `<br>`

浏览器不识别代码中的Enter换行

水平线：`<hr>`

| 属性名 | 含义     | 属性值                               |
| ------ | -------- | ------------------------------------ |
| align  | 对齐方式 | 可选择 left right center ,默认center |
| size   | 粗细     | px，默认为2                          |
| color  | 颜色     | 颜色                                 |
| width  | 宽度     | 可以是确定的px，也可以是百分比数值   |

> 此标签为单标签



#### 文本标签

作用：为文本添加特殊格式，以突出重点

常见的格式有：加粗、倾斜、下划线、删除线

**标签名**

加粗：`<strong>`  or  `<b>`

倾斜：`<em>`  or  `<i>`

下划线： `<ins>`  or  `<u>`

删除线：`<del>`  or  `<s>`

高亮标记：`<mark>被标记内容</mark>`

文本标记：

> 为了代码的可读性，通常使用左侧语义明显的标签，并且本标签允许嵌套



##### 文本注音

标签名: `<ruby>` 与 `<rt>`

```html
<ruby>
  <span>彳亍</span>
  <rt>xing</rt>
</ruby>
```

**注意！一定是内容在上，rt注音标签在下**



#### 框架标签

**作用**  

在当前页面中嵌入另一个 HTML 文档（如网页、视频、地图等），实现内容复用或外部资源整合。

**标签名**  

**`<iframe src="链接" width="像素值" height="像素值"></iframe>`**  

**核心属性**  

| **属性**         | **作用**                                               |
| ---------------- | ------------------------------------------------------ |
| `src`            | 指定嵌入内容的 URL（如 `https://www.toutiao.com`）。   |
| `width`/`height` | 设置框架的尺寸（如 `width="900"` 和 `height="300"`）。 |
| `name`           | 为框架命名，可用于表单提交或链接目标。                 |
| `sandbox`        | 限制框架内容的功能（如禁用脚本、表单提交等）。         |
| `allow`          | 指定允许使用的功能（如摄像头、麦克风）。               |

---

##### 举个栗子

```html
<iframe src="https://www.toutiao.com" width="900" height="300"></iframe>
```

- **效果**：在网页中嵌入头条网站的内容，尺寸为 900x300 像素。

利用 iframe 嵌入一个普通网页

```html
<iframe src="https://www.toutiao.com" width="900" height="300" frameborder="0"></iframe>
```

 利用 iframe 嵌入一个广告

 利用 iframe 嵌入其他内容

与超链接的 target 属性配合使用

```html
<a href="https://www.toutiao.com" target="tt">点我看新闻</a>
<a href="https://www.taobao.com" target="tt">点我看淘宝</a><br>
<iframe name="tt" frameborder="0" width="900" height="300"></iframe>
```

 与表单的 target 属性配合使用

  ```html
<!-- 写表单的target属性配合使用 -->
<form action="https://so.toutiao.com/search" target="container">
    <input type="text" name="keyword">
    <input type="submit" value="搜索">
</form>
  ```



### 列表标签

* 不管什么列表，都要注意结构

作用：布局内容排列整齐的区域

分类：无序、有序、定义列表



#### 无序列表

用的比较多

作用：布局排列整齐的不需要规定顺序的区域

标签名：`<ul>父级 <li>子级`

> ul是无序列表，只能包裹li标签；li是列表条目，可以包裹任何标签

```html
<ul>
    <li>第一项</li>
    <li>第二项</li>
    <li>第三项</li>
    …………
</ul>
```

这是无序列表的一个嵌套 ul --> li --> span --> ul --> li

#### 有序列表

作用：布局排列整齐的需要规定**顺序**的区域

标签名：`<ol>父级 <li>子级`

> ol 是有序列表，只能包裹 li 标签；li 是列表条目，可以**包裹**任何标签
>
> 尽量不要让 li 单独出现 

```html
<ol>
    <li>第一项</li>
    <li>第二项</li>
    <li>第三项</li>
    …………
</ol>
```



#### 定义列表

* 术语名称，对术语的描述 

* 一个术语名称可以有还几个描述

标签名：`<dl>父级 <dt>子级-列表标题 <dd>子级-列表详情`

```html
<dl>
    <dt>列表标题</dt>    //术语名称
    <dd>列表详情</dd>    //对术语的描述
    …………
</dl>
```



### 表格

#### 表格标签

作用：网页中的表格与Excel表格类似，用来展示数据

标签名：`table 嵌套 tr  tr嵌套td/th`

| 标签名  | 说明       |
| ------- | ---------- |
| table   | 表格       |
| caption | 表格标题   |
| tr      | 行         |
| th      | 表头单元格 |
| td      | 内容单元格 |

> 在网页中，表格默认没有边框线，使用 **border** 属性可以添加边框线，若 border 里面的值大于 1 ， 他显示的就只是外边框
>
> 控制表格的宽度 **width**
>
> 控制表格高度 **height** ， 表头 和 脚注 高度不会变
>
> 表格和表格之间的间距 **cellspacing** （并不是没有边框，而是，边框之间的距离为0）
>
> 整个单元格的水平居中 **align**，左对齐 left , 右对齐 right , 居中 center ； align = "left";
>
> 垂直方向对齐 **valign** , 居中 middle ,  底部 bottom , 顶部 top  ; valign = "top";

```html
 <table border="1">
        <tr>
            <th>表头1</th>
            <th>表头2</th>
            <th>表头3</th>
        </tr>
        <tr>
            <td>第二行第一格</td>
            <td>第二行第二格</td>
            <td>第二行第三格</td>
        </tr>
```



#### 表格结构标签

作用：用表格结构标签把内容划分区域，让表格结构更清晰，语义更清晰

> 可以不写

| 标签名     | 含义     | 特殊说明                                                     |
| ---------- | -------- | ------------------------------------------------------------ |
| thead      | 表格头部 | 表格头部内容（只能写 height ，不能写 border,width,cellspacing这些属性） |
| tbody      | 表格主体 | 主要内容区域                                                 |
| tfoot (td) | 表格底部 | 汇总信息区域                                                 |



#### 合并单元格 

作用：将多个单元格合并成一个单元格，以合并同类信息

其中，跨行合并与跨列合并不同

合并时会保留**最左**、**最上**单元格中的内容

属性：

rowspan	跨行

colspan	跨列

- 跨**行**合并，保留最上单元格，添加属性 `rowspan `  rowspan = ''5''
- 跨**列**合并，保留最左单元格，添加属性 `colspan`  colspan = "2";

> 本属性应用于<td>、<th>等子级标签



### 表单

**表单是网页中用于与用户交互、收集信息并提交给服务器处理的结构化区域。**

作用：收集信息

例如：登录页面、注册页面、搜素页面

将多个标签放置在同一表单中，使用 `form` 标签

提交数据需要使用 `form` 标签中的 `action` 属性，属性值为**提交数据的地址** ，表单的网址后面的 s 是 search ，是必须要写的

```html
<form action = "https://www.baidu.com/s">
```



#### 禁用表单控件

```html
<input disabled>
```

最好不要既写 disabled 又写 checked ，又禁用又选用，容易出笑话





#### input标签

input 标签 比较特殊 Type属性值不同，则功能不同>

标签名：

```html
<input type="……" name = "" value= "" maxlenght = "">    //这些都很重要，基本上都要写
```

百度的 name 是 wd

京东的 name 是 keyword

| Type 属性值 | 说明                     |
| ----------- | ------------------------ |
| text        | 文本框，用于输入单行文本 |
| password    | 密码框                   |
| radio       | 单选框                   |
| checkbox    | 多选框 / 复选框          |
| file        | 上传文件                 |



占位文本：提示信息

> 当有多个文本输入框时，占位文本可以提示输入，此属性可用于文本框与密码框

在input标签中添加属性 `placeholder`

```html
<input type="……" placeholder="提示信息">
```

在input标签中添加属性 `onclik`

```html
<input type="……" oncli="提示信息">
```

清除选中时的边框

```css
input:focus {
    outline: none; /* 移除默认的聚焦边框 */
}
```

清除默认边框

```css
input{
    border: none;
    background-color: #F5F5F5;   /*文本框中的背景颜色*/ 
    border-radius: 3px;
}
```



##### 单选框 radio

常用属性：

| 属性名  | 作用     | 特殊说明                                 |
| ------- | -------- | ---------------------------------------- |
| name    | 控件名称 | 控件分组，同组只能选中一个(**单选功能**) |
| checked | 默认选中 | 属性名和属性值相同，简写为一个单词       |

> name属性相同将划分为一组，同组的单选框只能有一个被选中

```html
<input type="radio" name="gender" value="male">男
<input type="radio" name="gender" value="female">女
```





##### 上传文件 file

使用 `multiple` 属性可以实现文件多选



##### 多选框 checkbox

多选框也叫复选框

默认选中：checked

```html
<input type="checkbox" checked>
```



#### 隐藏域

可以简单的防止批量注册

```html
<input type="hidden">
```

再加上   name  value  





#### 下拉菜单

使用例子：用户注册时选择城市时可以使用下拉菜单选择城市

标签名：`select ` 嵌套  `option `,  `select `是下拉菜单的整体，`option`是下拉菜单的每一项

标签名：

```html
<select name="place">
    <option value="北京">北京</option>
    <option value="上海">上海</option>
    <option value="深圳">深圳</option>
    <option value="广州">广州</option>
    <option value="武汉">武汉</option>
    <option value="下北泽" selected>下北泽</option>
</select>
```

> **selected**属性为**默认选项**
>
> 最好在 option 里面写 value 值 , 这样 select 的place 就可以找到



#### 文本域

作用：多行输入文本的表单控件

标签名：`textarea` 双标签

> 提示文字在双标签里，或者使用 placeholder

```html
<texterea name="other" cols="25" rows="10"></texterea>
```

texterea 这个是不可以写 type 这个属性的



#### Label标签

作用：网页中，某个标签的说明文本

​			用于关联文本和表单控件

​			在 input 中，不仅点击 框框 能获取焦点，还要点击前面的文字也可以获取焦点 

tips：用 `Lable` 标签绑定文字和表单控件的关系，增大表单控件的点击范围

实现此功能有两个写法

实现方法：

- 写法一

label 标签只包裹内容，不包过表单控件

这只 label 标签的 for 属性值 和 表单控件的 id 属性值相同

```html
<input type="radio" id ="man">
<label for="man">男</label> 
```



- 写法二

label 标签中包含 input 标签，此时则不需要属性

```html
<label><input type="radio">男</label>
```

> 方法一中两个标签为并列的关系，方法二是label标签为父级，input为子级，属于包含关系



tips：支持 label 标签增大点击范围的表单控件有

- 文本框
- 密码框
- 上传文件
- 单选框
- 多选框
- 下拉菜单
- 文本域
- ……



#### 按钮标签

作用：与用户进行交互的重要对象，通常用于提交，选择等场景

标签名：

```html
<button type="">
    按钮
</button>
```

| Type属性值 | 说明                                                         |
| ---------- | ------------------------------------------------------------ |
| submit     | **提交**按钮，点击后可以提交数据到后台(默认选项)   //不可以写 name 的属性 |
| reset      | **重置**按钮，点击后将表单控件恢复默认值                     |
| button     | **普通**按钮，默认没有功能，一般配合 JavaScript 使用         |

可以在 input 去写，也可以直接用 button 去写



##### 清除按钮默认样式：

使用 CSS 重置属性

这是最直接的方法，通过设置关键的 CSS 属性来清除默认样式。

```css
button {
    /* 清除边框和背景 */
    border: none;
    background: none;
    
    /* 清除内边距和外边距 */
    padding: 0;
    margin: 0;
    
    /* 重置字体样式，使其继承父元素 */
    font: inherit;
    color: inherit;
    
    /* 去除点击时的轮廓（可选，注意可访问性） */
    outline: none;
    
    /* 去除默认的鼠标样式（可选） */
    cursor: pointer;
}
```



#### 逻辑分组控件



##### fieldset 分组

**功能**：将表单中的控件逻辑分组，通过视觉边框（默认样式）增强表单结构的清晰度。

核心属性：

- `disabled`：禁用 `<fieldset>` 内所有子控件。
- `form`：指定所属表单（用于不在 `<form>` 内部的 `<fieldset>`）。
- `name`：为分组命名，便于 JavaScript 操作。

- **适用场景**：适用于需要将相关表单元素（如输入框、单选按钮等）分组展示的场景。



##### legend 标题

- **功能**：为 `<fieldset>` 分组提供标题或描述，提升表单的可读性和可访问性。
- 使用规则：
  - **必须是 `<fieldset>` 的第一个子元素**。
  - 属于 `<fieldset>` 的一部分，不能单独使用。
- **作用**：帮助用户（包括屏幕阅读器用户）快速理解分组内容的用途。

食用方法：

```html
<form>
  <fieldset>
    <legend>个人信息</legend>
    <label for="name">姓名:</label>
    <input type="text" id="name" name="name"><br><br>
    <label for="email">邮箱:</label>
    <input type="email" id="email" name="email">
  </fieldset>
</form>
```



#### 表单总结

| 标签名 | 标签语义 | 常用属性                                                     |
| ------ | -------- | ------------------------------------------------------------ |
| form   | 表单     | action 属性：表单要提交的地址。<br>target 属性：跳转的新地址的打开方式；值：_self、_blank<br>method 属性：请求方式，可选值：get、post |

| input    | 多种形式的表单控件 | type 属性：指定表单控件的类型。<br>可选值：text、password、radio、checkbox、hidden、submit、reset、button 等。<br>name 属性：指定数据名称<br>value 属性：<br>对于输入框：指定默认输入的值；<br>对于单选和复选框：实际提交的数据；<br>对于按钮：显示按钮文字。<br>disabled 属性：设置表单控件不可用。<br>maxlength 属性：用于输入框，设置最大可输入长度。<br>checked 属性：用于单选按钮和复选框，默认选中 |
| -------- | ------------------ | ------------------------------------------------------------ |
| textarea | 文本域             | name 属性：指定数据名称<br>rows 属性：指定默认显示的行数，影响文本域的高度。<br>cols 属性：指定默认显示的列数，影响文本域的宽度。<br>disabled 属性：设置表单控件不可用。 |
| select   | 下拉框             | name 属性：指定数据名称<br>disabled 属性：设置整个下拉框不可用。 |
| option   | 下拉框的选项       | disabled 属性：设置拉下选项不可用。<br>value 属性：该选项事件提交的数据（不指定 value，会把标签中的内容作为提交数据）<br>selected 属性：默认选中。 |
| button   | 按钮               | disabled 属性：设置按钮不可用。<br>type 属性：设置按钮的类型，值：submit（默认）、reset、button |
| label    | 与表单控件做关联   | for 属性：值与要关联的表单控件的ID值相同。                   |
| fieldset | 表单控件分组       | -                                                            |
| legend   | 分组名称           | -                                                            |



### 字符实体

作用：在网页中显示预留字符



| **实体名称** | **实体编号** | **字符** | **说明**                       |
| ------------ | ------------ | -------- | ------------------------------ |
| `&amp;`      | `&#38;`      | `&`      | 和号（必须转义的字符）         |
| `&lt;`       | `&#60;`      | `<`      | 小于号（HTML 标签的开始符号）  |
| `&gt;`       | `&#62;`      | `>`      | 大于号（HTML 标签的结束符号）  |
| `&quot;`     | `&#34;`      | `"`      | 双引号（属性值分隔符）         |
| `&apos;`     | `&#39;`      | `'`      | 单引号（HTML5 支持）           |
| `&nbsp;`     | `&#160;`     | ` `      | 非间断空格（多个连续空格显示） |
| `&copy;`     | `&#169;`     | `©`      | 版权符号                       |
| `&reg;`      | `&#174;`     | `®`      | 注册商标符号                   |
| `&trade;`    | `&#8482;`    | `™`      | 商标符号                       |
| `&euro;`     | `&#8364;`    | `€`      | 欧元符号                       |
| `&yen;`      | `&#165;`     | `¥`      | 日元符号                       |
| `&pound;`    | `&#163;`     | `£`      | 英镑符号                       |
| `&deg;`      | `&#176;`     | `°`      | 度数符号（如 30°C）            |
| `&times;`    | `&#215;`     | `×`      | 乘号                           |
| `&divide;`   | `&#247;`     | `÷`      | 除号                           |
| `&ndash;`    | `&#8211;`    | `–`      | 短破折号（en dash）            |
| `&mdash;`    | `&#8212;`    | `—`      | 长破折号（em dash）            |
| `&hellip;`   | `&#8230;`    | `…`      | 省略号（三个点）               |
| `&laquo;`    | `&#171;`     | `«`      | 左引号（法语等语言）           |
| `&raquo;`    | `&#187;`     | `»`      | 右引号（法语等语言）           |
| `&lsquo;`    | `&#8216;`    | `‘`      | 左单引号                       |
| `&rsquo;`    | `&#8217;`    | `’`      | 右单引号                       |
| `&ldquo;`    | `&#8220;`    | `“`      | 左双引号                       |
| `&rdquo;`    | `&#8221;`    | `”`      | 右双引号                       |



### 注释

HTML的注释方式为  **`<!--内容-->`**

VS Code 中，添加/删除注释的快捷键是 **`Ctrl + /`**

注释的里面内容就不能再写注释了，注释不可以嵌套

也可以临时让某一行或某一段代码注释掉



### 路径

定义：路径指的是查找文件时，从起点到终点经历的路线

分类：

- 相对路径：从当前文件位置出发查找目标文件
- 绝对路径：从盘符出发查找目标文件

#### 相对路径

从当前文件位置出发查找目标文件

- **`/`** 表示进入某个文件夹里面 ，下一级
- **`.`** 表示当前文件所在文件夹
- **`./`** 为当前目录   **`../`**为上一级路径   **`../../`**为上上一级路径  以此类推

#### 绝对路径 

从 根目录 出发 ，C 盘 / D盘 / E盘

* 本地绝对路径
  * 从 盘符 出发 " C : / 打开的文件夹 / xxx.jpg "
  * 用的特别少

* 网络绝对路径

  * http / https 开头

  * 注意：网址不可以写错
  * 若服务器开启了防盗链，会造成如片引入失败



Windows电脑从 盘符 出发

Mac电脑从根 目录(/) 出发



### meta元信息

**配制字符编码**

```html
<meta charset="UTF-8">
```

**针对IE浏览器的一个兼容性设置**

```html
<meta http-equiv="X-UA-Compatible" content="IE=edge">
```

**针对移动端的一个配置**

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

**配置网页关键字**

```html
<meta name="keywords" content="8-12个以英文逗号隔开的单词/词语">
```

**配置网页描述信息**

```html
<meta name="description" content="80字以内的一段话，与网站内容相关">
```

**针对搜索引擎爬虫配置**：

```html
<meta name="robots" content="此处可选值见下表">
```

**配置选项表**

| 值        | 描述                               |
| --------- | ---------------------------------- |
| index     | 允许搜索爬虫索引此页面。           |
| noindex   | 要求搜索爬虫不索引此页面。         |
| follow    | 允许搜索爬虫跟随此页面上的链接。   |
| nofollow  | 要求搜索爬虫不跟随此页面上的链接。 |
| all       | 与 index, follow 等价              |
| none      | 与 noindex, nofollow 等价          |
| noarchive | 要求搜索引擎不缓存页面内容。       |
| nocache   | noarchive 的替代名称。             |

**自动刷新**

```html
<meta http-equiv="refresh" content="3">   //原地刷新
```

```html
<meta http-equiv="refresh" content="10;url=http://www.baidu.com">
```





# H5

### 简介

#### 1. 什么是HTML5？

- HTML5 是新一代的 HTML 标准，2014年10月由万维网联盟（W3C）完成标准制定。
- 官网地址：
  - W3C 提供：https://www.w3.org/TR/html/index.html
  - WHATWG 提供：https://whatwg-cn.github.io/html/multipage
- HTML5 在狭义上是指新一代的 HTML 标准，在广义上是指：整个前端。 

#### 2. HTML5 优势

1. 针对 JavaScript，新增了很多可操作的接口。
2. 新增了一些语义化标签、全局属性。
3. 新增了多媒体标签，可以很好地替代 flash。
4. 更加侧重语义化，对于 SEO 更友好。
5. 可移植性好，可以大量应用在移动设备上。

#### 3. HTML5兼容性

- 支持：Chrome、Safari、Opera、Firefox 等主流浏览器。
- IE 浏览器必须是 9 及以上版本才支持 HTML5，且 IE9 仅支持部分 HTML5 新特性。

这段内容说明了HTML5在不同浏览器中的兼容性情况，特别是对Internet Explorer（IE）浏览器的版本要求和限制。



### H5新增语义化标签

**优点**：  

- 提升 SEO（搜索引擎友好）  
- 提高可访问性（屏幕阅读器可识别）  
- 代码结构清晰，便于团队协作和维护

#### 新增布局标签 

| 标签名  | 语义                                                         | 单/双标签 |
| ------- | ------------------------------------------------------------ | --------- |
| header  | 整个页面，或部分区域的头部                                   | 双        |
| footer  | 整个页面，或部分区域的底部                                   | 双        |
| nav     | 导航                                                         | 双        |
| article | 文章、帖子、杂志、新闻、博客、评论等。                       | 双        |
| section | 页面中的某段文字，或文章中的某段文字（里面文字通常里面会包含标题）。 | 双        |
| aside   | 侧边栏                                                       | 双        |
| main    | 文档的主要内容 (WHATWG 没有语义，IE 不支持)，几乎不用。      | 双        |
| hgroup  | 包裹连续的标题，如文章主标题、副标题的组合（W3C 将其删除）   | 双        |

**关于 `article` 和 `section`：**

* `article` 里面可以有多个 `section`。
* `section` 强调的是分段或分块，如果你想将一块内容分成几段的时候，可使用 `section` 元素。
* article` 比 `section` 更强调独立性，一块内容如果比较独立、比较完整，应该使用 `article` 元素。



#### 新增状态标签

**手机电量**	**meter标签**

max 最大；min 最小；value 现在； low 最低； high 最高； optimum 最适（会出现颜色变化）

```html
<meter max="100" min="0" value="10" low="20" high="80" optimum="90"></meter>
```

![image-20250906172200538](./笔记/笔记/web-img/image-20250906172200538.png)

**当前进度**	**progress标签**

```html
<progress max="100" value="40"></progress>
```

![image-20250906172239618](./笔记/笔记/web-img/image-20250906172239618.png)



#### 新增列表标签

| 标签名   | 语义                                        | 单/双标签 |
| -------- | ------------------------------------------- | --------- |
| datalist | 用于搜索框的关键字提示                      | 双        |
| details  | 用于展示问题和答案，或对专有名词进行解释    | 双        |
| summary  | 写在 details 的里面，用于指定问题或专有名词 | 双        |

```html
<input type="text" list="mydata">
<datalist id="mydata">
    <option value="周冬雨">周冬雨</option>
    <option value="周杰伦">周杰伦</option>
    <option value="温兆伦">温兆伦</option>
    <option value="马冬梅">马冬梅</option>
</datalist>

<details>
    <summary>如何走上人生巅峰？</summary>
    <p>一步一步走呗</p>
</details>
```

#### 新增文本标签

##### 4.1 文本注音

| 标签名 | 语义                            | 单/双标签 |
| ------ | ------------------------------- | --------- |
| ruby   | 包裹需要注音的文字              | 双        |
| rt     | 写注音，rt 标签写在 ruby 的里面 | 双        |

```html
<ruby>
    <span>魑魅魍魉</span>
    <rt>chī mèi wǎng liǎng </rt>
</ruby>
```

##### 4.2 文本标记

| 标签名 | 语义 | 单/双标签 |
| ------ | ---- | --------- |
| mark   | 标记 | 双        |

注意：W3C 建议 mark 用于标记搜索结果中的关键字。

#### 新增的表单控件属性

| 属性名       | 功能                                                         |
| ------------ | ------------------------------------------------------------ |
| placeholder  | 提示文字（注意：不是默认值，value 是默认值），适用于文字输入类的表单控件。 |
| required     | 表示该输入项**必填**，适用于除按钮外其他表单控件。           |
| autofocus    | 自动获取焦点，适用于所有表单控件。                           |
| autocomplete | 自动完成，可以设置为 on 或 off，适用于文字输入类的表单控件。<br>注意：密码输入框、多行输入框不可用。 |
| pattern      | 填写正则表达式，适用于文本输入类表单控件。<br>注意：多行输入不可用，且空的输入框不会验证，往往与 required 配合。 |

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <form action="">
        账号：<input type="text" name="account" placeholder="请输入账号" required autofocus autocomplete="on" pattern="\w{6}">
        <br>
        密码：<input type="password" name="pwd" placeholder="请输入密码" required pattern="\w{6}">
        <br>
        性别：
        <input type="radio" value="male" name="gender" required>男
        <input type="radio" value="female" name="gender" required>女
        <br>
        <button>提交</button>
    </form>
</body>

</html>
```

#### input新增的type属性值

```html
    <form action="">
        邮箱：<input type="email">
        url: <input type="url" name="url">
        num: <input type="number" name="num" step="2" max="10" min="0">
        search: <input type="search" name="keyword">
        电话: <input type="tel" name="phone"> <!-- 在手机端可以-->
        光照强度： <input type="range" name="range" max="100" min="0" value="0">
        颜色： <input type="color" name="color">
        日期： <input type="date" name="date">
        月份：<input type="month" name="month">
        周：<input type="week" name="week">
        时间: <input type="time" name="time">
        日期+时间： <input type="datetime-local" name="time2">

        <br>
        <button>提交</button>
    </form>
```

#### 新增视频标签

标签名：`<video src="视频的URL"></video>`

###### 常见属性表

| 属性     | 值                     | 描述                                                         |
| -------- | ---------------------- | ------------------------------------------------------------ |
| src      | URL地址                | 视频地址                                                     |
| width    | 像素值                 | 设置视频播放器的宽度                                         |
| height   | 像素值                 | 设置视频播放器的高度                                         |
| controls | -                      | 向用户显示视频控件（比如播放/暂停按钮）                      |
| muted    | -                      | 视频静音                                                     |
| autoplay | -                      | 视频自动播放                                                 |
| loop     | -                      | 循环播放                                                     |
| poster   | URL地址                | 视频封面                                                     |
| preload  | auto / metadata / none | 视频预加载，如果使用 autoplay，则忽略该属性。<br>• none: 不预加载视频。<br>• metadata: 仅预先获取视频的元数据（例如长度）。<br>• auto: 下载整个视频文件，即使用户不希望使用它。 |

> 在HTML5中，如果属性名与属性值完全一样，则可简写为一个单词

#### 新增音频标签

标签名：`<audio src="音频的URL"></audio>`

###### 常见属性表

| 属性     | 值                     | 描述                                                         |
| -------- | ---------------------- | ------------------------------------------------------------ |
| src      | URL地址                | 音频地址                                                     |
| controls | -                      | 向用户显示音频控件（比如播放/暂停按钮）                      |
| autoplay | -                      | 音频自动播放                                                 |
| muted    | -                      | 音频静音                                                     |
| loop     | -                      | 循环播放                                                     |
| preload  | auto / metadata / none | 音频预加载，如果使用 autoplay，则忽略该属性。<br>• none: 不预加载音频。<br>• metadata: 仅预先获取音频的元数据（例如长度）。<br>• auto: 可以下载整个音频文件，即使用户不希望使用它。 |

> 在HTML5中，如果属性名与属性值完全一样，则可简写为一个单词

#### 新增全局属性

| 属性名          | 功能                                                         |
| --------------- | ------------------------------------------------------------ |
| contenteditable | 表示元素是否可被用户编辑，可选值如下：<br>• true : 可编辑<br>• false : 不可编辑 |
| draggable       | 表示元素可以被拖动，可选值如下：<br>• true : 可拖动<br>• false : 不可拖动 |
| hidden          | 隐藏元素                                                     |
| spellcheck      | 规定是否对元素进行拼写和语法检查，可选值如下：<br>• true : 检查<br>• false : 不检查 |
| contextmenu     | 规定元素的上下文菜单，在用户鼠标右键点击元素时显示。         |
| data-*          | 用于存储页面的私有定制数据。                                 |

```html
    <div class="contenteditable" contenteditable="true">nihao tianqizhenhao</div>
    <div class="draggable" draggable="true" hidden data-a="1" data-b="2">nihao tianqizhenhao</div>
```





### H5兼容性问题

让IE浏览器处于一个 最优的渲染模式

```html
<!--设置IE总是使用最新的文档模式进行渲染-->
<meta http-equiv="X-UA-Compatible" content="IE=Edge">

<!--优先使用 webkit ( Chromium ) 内核进行渲染, 针对360等壳浏览器-->
<meta name="renderer" content="webkit">
```

使用 html5shiv 让低版本浏览器认识 H5 的语义化标签。

```html
<!--[if lt IE 9]>
<script src="../sources/js/html5shiv.js"></script>
<![endif]-->
```

**扩展**

- `lt` 小于
- `lte` 小于等于
- `gt` 大于
- `gte` 大于等于
- `!` 逻辑非

```html
<!--[if IE 8]>仅IE8可见<![endif]-->
<!--[if gt IE 8]>仅IE8以上可见<![endif]-->
<!--[if lt IE 8]>仅IE8以下可见<![endif]-->
<!--[if gte IE 8]>IE8及以上可见<![endif]-->
<!--[if lte IE 8]>IE8及以下可见<![endif]-->
<!--[if !IE 8]>非IE8的IE可见<![endif]-->
```



#### 1. 添加元信息，确保浏览器最优渲染

##### **1.1 设置IE使用最新文档模式**

- **代码**：

  ```html
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
  ```

- **作用**：  
  强制IE浏览器（如IE8/9/10/11）使用最新版本的文档模式进行渲染，避免因旧版模式导致的兼容性问题（如HTML/CSS解析差异）。

##### **1.2 优先使用 WebKit 内核（针对双核浏览器）**

- **代码**：

  ```html
  <meta name="renderer" content="webkit">
  ```

- **作用**：  
  指示双核浏览器（如360、QQ浏览器）优先采用WebKit内核（Chromium）进行页面渲染，提升HTML5/CSS3支持度和渲染效果。

---

#### 2. 使用 `html5shiv` 兼容低版本浏览器

- **代码**：

  ```html
  <!--[if lt IE 9]>
  <script src="../sources/js/html5shiv.js"></script>
  <![endif]-->
  ```

- **作用**：  

  - **兼容HTML5语义标签**：让IE9及以下版本识别 `<header>`、`<footer>`、`<article>` 等HTML5标签。  
  - **样式支持**：通过JavaScript动态创建标签，使其可被CSS样式控制。  

- **适用场景**：  
  针对仍需支持IE8及以下版本的项目，确保HTML5结构在旧版浏览器中正常显示。

---

#### 3. 条件注释的运算符

- **常见运算符**：

  | 运算符 | 含义     | 示例                  |
  | ------ | -------- | --------------------- |
  | `lt`   | 小于     | `<!--[if lt IE 9]>`   |
  | `lte`  | 小于等于 | `<!--[if lte IE 8]>`  |
  | `gt`   | 大于     | `<!--[if gt IE 7]>`   |
  | `gte`  | 大于等于 | `<!--[if gte IE 10]>` |
  | `!`    | 逻辑非   | `<!--[if !IE]>`       |

- **作用**：  
  针对IE不同版本加载特定代码（如脚本、样式），实现精细化兼容性处理。

---

##### **总结**

1. **渲染优化**：通过 `meta` 标签强制浏览器使用最优内核（如IE最新模式、WebKit），提升HTML5/CSS3兼容性。  
2. **HTML5标签兼容**：`html5shiv` 解决IE9及以下版本不支持HTML5语义标签的问题。  
3. **条件注释**：利用IE特有语法，按版本加载特定资源，实现差异化兼容策略。  
4. **适用性**：适用于需兼容旧版浏览器（如IE8/9）的项目，确保现代网页在老旧环境中稳定运行。



# CSS

### CSS特性

CSS特性：化简代码/定位问题，并解决问题

- 继承性
- 层叠性
- 优先级

#### 继承性

特点：子级默认继承父级的文字控制属性

比如在body标签设置文字控制属性，body内的文字都将默认跟随body设置

如果标签有自己的样式则生效自己的样式，不继承

- **概念**：元素会自动拥有其父元素、或其祖先元素上所设置的某些样式。
- **规则**：优先继承离得近的。
- 常见的可继承属性
  - `text-??`, `font-??`, `line-??`, `color` .....
- **备注**：参照MDN网站，可查询属性是否可被继承。



#### 层叠性

如果发生了样式冲突，那就会根据一定的规则（选择器优先级），进行样式的层叠（覆盖）

特点：

- 相同的属性会覆盖：后面的CSS属性会覆盖前面的CSS属性
- 不同的属性会叠加：不同的CSS属性都能生效



#### 优先级

- **简单聊**：`!important > 内联样式 > ID > 类 = 属性选择器 = 伪类 > 标签 > 通配符/伪元素`

- 详细聊

  ：需要计算权重。

  - 计算权重时需要注意：并集选择器的每一个部分是分开算的！

特点：优先级也叫权重，当一个标签使用了多种选择器时，基于不同种类的选择器的匹配规则

规则：选择器指向性越强，其优先级越高优先生效

> 总的来说 选中标签的范围越大，优先级越低 !important最优先

举个栗子

```html
<style>
    div{
        color: red;
    }

    .box{
        color；green;
    }
</style>

<div class="box">
    此时 div标签 内容为绿色
</div>
```

##### **详细描述**

###### 1. 计算方式：每个选择器，都可计算出一组权重，格式为：(a, b, c)

- **a**：ID 选择器的个数。
- **b**：类、伪类、属性选择器的个数。
- **c**：元素、伪元素选择器的个数。

**例如：**

| 选择器                   | 权重      |
| ------------------------ | --------- |
| ul > li                  | (0, 0, 2) |
| div ul > li p a span     | (0, 0, 6) |
| #atguigu .slogan         | (1, 1, 0) |
| #atguigu .slogan a       | (1, 1, 1) |
| #atguigu .slogan a:hover | (1, 2, 1) |

###### 2. 比较规则：按照从左到右的顺序，依次比较大小，当前位胜出后，后面的不再对比。例如：

- (1, 0, 0) > (0, 2, 2)
- (1, 1, 0) > (1, 0, 3)
- (1, 1, 3) > (1, 1, 2)

###### 3. 特殊规则：

1. 行内样式权重大于所有选择器。
2. !important 的权重，大于行内样式，大于所有选择器，权重最高！



### CSS语法

##### CSS 语法由两部分构成：

- **选择器**：找到要添加样式的元素。
- **声明块**：设置具体的样式（声明块是由一个或多个声明组成的），声明的格式为：属性名: 属性值；

###### 备注：

1. 最后一个声明后的分号理论上能省略，但最好还是写上。
2. 选择器与声明块之间，属性名与属性值之间，均有一个空格，理论上能省略，但最好还是写上。



##### 叠加计算规则

特点：如果是复合选择器，则需要权重叠加计算

公式：行内样式 > id选择器个数 > 类选择器个数 > 标签选择器个数

规则：

- 从左向右 一次比较选择器个数，同一级个数多的优先级高；个数相同，则向后比较
- `!important` 权重最高
- 继承权重最低

###### 优先级规则：行内样式 > 内部样式 = 外部样 式

1. 内部样式、外部样式，这二者的优先级相同，且：后面的会覆盖前面的（简记：“后来者居上”）。
2. 同一个样式表中，优先级也和编写顺序有关，且：后面的会覆盖前面的（简记：“后来者居上”）。

| 分类     | 优点                                                         | 缺点                                                      | 使用频率 | 作用范围 |
| -------- | ------------------------------------------------------------ | --------------------------------------------------------- | -------- | -------- |
| 行内样式 | 优先级最高                                                   | 1. 结构与样式未分离<br>2. 代码结构混乱<br>3. 样式不能复用 | 很低     | 当前标签 |
| 内部样式 | 1. 样式可复用<br>2. 代码结构清晰                             | 1. 结构与样式未彻底分离<br>2. 样式不能多页面复用          | 一般     | 当前页面 |
| 外部样式 | 1. 样式可多页面复用<br>2. 代码结构清晰<br>3. 可触发浏览器的缓存机制<br>4. 结构与样式彻底分离 | 需要引入才能使用                                          | 最高     | 多个页面 |



### CSS引入方式

#### 内部 式表

CSS代码写在 style 标签里面

1. 写在 html 页面内部，将所有的 CSS 代码提取出来，单独放在 `<style>` 标签中。
2. 语法：

```css
<style>
  h1 {
    color: red;
    font-size: 40px;
  }
</style>
```

3. 注意点：
   * `<style>` 标签理论上可以放在 HTML 文档的任何地方，但一般都放在 `<head>` 标签中。
   * 此种写法：样式可以复用、代码结构清晰。

4. 存在的问题：
   * 并没有实现：结构与样式完全分离。
   * 多个 HTML 页面无法复用样式。

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS测试场</title>
    <style>
		/*此处书写CSS代码*/
        /*选择器*/
        p{
            /*CSS属性*/
            color:red;
            font-size:30px;
            
        }
    </style>
</head>
	<body>
	<p>Hello World</p>
	</body>
</html>
```



#### 外部样式表

首先，CSS 代码写在单独的 CSS 文件中（.css）

其次，在 HTML 使用 link 标签引入

```html
<link rel="stylesheet" href="CSS文件路径">
```

**写在单独的 .css 文件中，随后在 HTML 文件中引入使用。**

1. 语法：
   * 新建一个扩展名为 .css 的样式文件，把所有 CSS 代码都放入此文件中。

```css
h1 {
  color: red;
  font-size: 40px;
}
```

2. 在 HTML 文件中引入 .css 文件。

```
<link rel="stylesheet" href="./xxx.css">
```

3. 注意点：
   * `<link>` 标签要写在 `<head>` 标签中。

```
<link>
```

 

标签属性说明：

- `href`：引入的文档来自于哪里。
- `rel`：（relation：关系）说明引入的文档与当前文档之间的关系。

1. 外部样式的优势：样式可以复用、结构清晰、可触发浏览器的缓存机制，提高访问速度，实现了结构与样式的完全分离。
2. 实际开发中，几乎都使用外部样式，这是最推荐的使用方式！



#### 行内样式表(不推荐)

通常配合 JavaScript 使用

CSS 写在标签的 style 属性值里

```html
<div style="color:red;font-size:20px">这是 CSS 行内样式</div>
```

1. 写在标签的 `style` 属性中，（又称：内联样式）。
2. 语法：

```html
<h1 style="color:red;font-size:60px;">欢迎来到尚硅谷学习</h1>
```

3. 注意点：
   * `style` 属性的值不能随便写，写要符合 CSS 语法规范，是 名:值; 的形式。
   * 行内样式表，只能控制当前标签的样式，对其他标签无效。

4. 存在的问题： 书写繁琐、样式不能复用、并且没有体现：出结构与样式分离的思想，不推荐大量使用，只有对当前元素添加简单样式时，才偶尔使用。



### CSS3私有前缀

##### **什么是私有前缀**

如下代码中的 `-webkit-` 就是私有前缀。

```css
div {
    width: 400px;
    height: 400px;
    -webkit-border-radius: 20px;
}
```

#####  **为什么要有私有前缀**

- W3C 标准所提出的某个 CSS 特性，在被浏览器正式支持之前，浏览器厂商会根据浏览器的内核，使用私有前缀来测试该 CSS 特性，在浏览器正式支持该 CSS 特性后，就不需要私有前缀了。
- 举个例子：

```css
-webkit-border-radius: 20px;
-moz-border-radius: 20px;
-ms-border-radius: 20px;
-o-border-radius: 20px;
border-radius: 20px;
```

- 查询 CSS3 兼容性的网站：https://caniuse.com/

#####  **常见浏览器私有前缀**

- Chrome 浏览器: `-webkit-`
- Safari 浏览器: `-webkit-`
- Firefox 浏览器: `-moz-`
- Edge 浏览器: `-webkit-`
- ~~旧 Opera 浏览器: `-o-`~~
- ~~旧 IE 浏览器: `-ms-`~~

注意：

>我们在编码时，不用过于关注浏览器私有前缀，不用绞尽脑汁地去记忆，也不用每个都去查询，因为常用的 CSS3 新特性，主流浏览器都是支持的，即便是为了老浏览器而加前缀，我们也可以借助现代的构建工具，去帮我们添加私有前缀。







### 选择器

作用：查找标签，设置样式

#### 常用的选择器

- 标签选择器
- 类选择器
- id选择器
- 通配符选择器

| 基本选择器 | 特点                                                 | 用法                  |
| ---------- | ---------------------------------------------------- | --------------------- |
| 通配选择器 | 选中所有标签，一般用于清除样式。                     | `* {color:red}`       |
| 元素选择器 | 选中所有同种标签，但是不能差异化选择。               | `h1 {color:red}`      |
| 类选择器   | 选中所有特定类名（class 值）的元素 —— 使用频率很高。 | `.say {color:red}`    |
| ID 选择器  | 选中特定 id 值的那个元素（唯一的）。                 | `#earthy {color:red}` |

> 选择器优先级：

- `!important > 内联样式 > ID > 类 = 属性选择器 = 伪类 > 标签 > 通配符/伪元素`

#### 标签选择

标签选择器：使用标签名作为选择器，选中同名标签设置的相同样式

> 相同标签名的所有标签都会受到设置的相同样式

#### 元素选择器

###### 作用：为页面中某种元素统一设置样式。

- **语法**：

  ```css
  标签名 {
      属性名: 属性值;
  }
  ```

- **举例**：

  ```css
  /* 选中所有h1元素 */
  h1 {
      color: orange;
      font-size: 40px;
  }
  
  /* 选中所有p元素 */
  p {
      color: blue;
      font-size: 60px;
  }
  ```

- **备注**：元素选择器无法实现差异化设置，例如上面的代码中，所有的 p 元素效果都一样。



#### 类选择器

根据元素的 class 值，来选中某些元素

类选择器：查找标签，差异化设置标签的显示效果

实现步骤：

- 定义类选择器：`.类名`
- 使用类选择器：`标签添加 class="类名"`

```css
.red{
    color:red;
}
```



此时，要在目标标签中添加 `class` 属性

```html
<div class="red">
    此时，css中，类名为red的选择器将触发，同时内部的设置将被应用
</div>
```

**注意：**

- 类名自定义，不要用纯数字、数字开头或中文，尽量用英文命名
- 一个类选择器可以供多个标签使用
- 一个标签可以使用多个类名，类名之间用空格隔开
- 命名时如要使用多个单词，可以使用 `-` 连接



#### id选择器

根据元素的 id ，精准的选中某个元素

id选择器：查找标签，差异化设置标签的显示效果

场景：id选择器通常配合 JavaScript 使用，很少用来设置CSS样式

实现步骤：

- 定义 id选择器：`#id`
- 使用 id选择器：`标签添加属性 id="id名"`

 类似于类选择器，将 `.`换成`#` ， 将`class`属性 换成 `id`属性

**注意：**

* 一个标签不能使用多个id

* 不可以是数字开头，不要有空格



#### 通配符选择器

可以选中多有的 HTML 元素

但是，清楚样式的时候，会有很大的帮助

通配符选择器：查找页面所有标签，设置相同样式

使用方法：*，不需要调用，浏览器自动查找页面所有标签，设置相同的样式

```css
*{
    color:red;
}
```



#### 复合选择器

作用：由两个或多个基础选择器，通过不同的方式组合而成

复合选择器有多种，以下将逐步介绍



##### 交集选择器

**作用：选中同时符合多个条件的元素。**

- **交集有并且的含义**（通俗理解：即……又……的意思），例如：年轻且长得帅。

- **语法**：

  ```
  选择器1选择器2选择器3...选择器n {}
  ```

- **举例**：

  ```css
  /* 选中：类名为beauty的p元素，为此种写法用的非常多！！！！ */
  p.beauty {
      color: blue;
  }
  
  /* 选中：类名包含rich和beauty的元素 */
  .rich.beauty {
      color: green;
  }
  ```

- **注意**：

  1. 有标签名，标签名必须写在前面。
  2. id 选择器、理论上可以作为交集的条件，但实际应用中几乎不用 —— 因为没有意义。
  3. 交集选择器中不可能出现两个元素选择器，因为一个元素，不可能即是 p 元素又是 span 元素。
  4. 用的最多的交集选择器是：元素选择器配合类名选择器，例如：`p.beauty`。



##### 并集选择器

**作用：选中多个选择器对应的元素，又称：分组选择器。**

- **所谓并集就是或者的含义**（通俗理解：要么……要么……的意思），例如：给我转10万块钱或者我报警。

- **语法**：

  ```
  选择器1, 选择器2, 选择器3, ... 选择器n {}
  ```

  多个选择器通过逗号连接，此处逗号的含义就是：或。

- **举例**：

  ```css
  /* 选中id为peiqi，或类名为rich，或类名为beauty的元素 */
  #peiqi,
  .rich,
  .beauty {
      font-size: 40px;
      background-color: skyblue;
      width: 200px;
  }
  ```

- **注意**：

  1. 并集选择器，我们一般竖着写。
  2. 任何形式的选择器，都可以作为并集选择器的一部分。
  3. 并集选择器，通常用于集体声明，可以缩小样式表体积。



##### 后代选择器

* 选中指定元素中，符合要求的后代元素

* 语法：选择器1 选择器2 选择器3 ...... 选择器n {} （先写祖先，再写后代）
  * **选择器之间，用空格隔开，空格可以理解为："xxx 中的"，其实就是后代的意思。**
  * **选择器 1234 .... n，可以是我们之前学的任何一种选择器。**

举例：

```css
/* 选中ul中的所有li */
ul li {
    color: red;
}

/* 选中ul中所有li中的a */
ul li a {
    color: orange;
}

/* 选中类名为subject元素中的所有li */
.subject li {
    color: blue;
}

/* 选中类名为subject元素中的所有类名为front-end的li */
.subject li.front-end {
    color: blue;
}
```

注意：

1. 后代选择器，最终选择的是后代，不选中祖先。
2. 儿子、孙子、重孙子，都算是后代。
3. 结构一定要符合之前讲的 HTML 嵌套要求，例如：不能 p 中写 h1 ~ h6。



##### 子代选择器

- **作用**：选中指定元素中，符合要求的子元素（儿子元素）。（先写父，再写子）

  - 子代选择器又称：子元素选择器、子选择器。

- **语法**：

  ```
  选择器1 > 选择器2 > 选择器3 > ...... 选择器n {}
  ```

  - 选择器之间，用 `>` 隔开，`>` 可以理解为："xxx 的子代"，其实就是儿子的意思。
  - 选择器 1234 .... n，可以是我们之前学的任何一种选择器。

- **举例**：

  ```css
  /* div中的子代a元素 */
  div > a {
      color: red;
  }
  
  /* 类名为persons的元素中的子代a元素 */
  .persons > a {
      color: red;
  }
  ```

- **注意**：

  1. 子代选择器，最终选择的是子代，不是父级。
  2. 子、孙子、重孙子、重重孙子......统称后代！，子就是指儿子。



##### 相邻兄弟选择器

选中指定元素后，符合条件的相邻兄弟元素（紧挨着的下一个）

相邻兄弟选择器（Adjacent sibling selector）可选择紧接在另一元素后的元素，且二者有相同父元素。

如果需要选择紧接在另一个元素后的元素，而且二者有相同的父元素，可以使用相邻兄弟选择器（Adjacent sibling selector）。

```css
div+p {
    background-color:yellow; /*选择div之后紧邻的兄弟p元素*/
}
```

**案例**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    div+p{
      color: red;
    }
  </style>
</head>
<body>
  <div>d1</div>
  <p>2</p>
  <p>3</p>
</body>
</html>
```



##### 后续兄弟选择器

后续兄弟选择器选取所有指定元素之后的**所有兄弟元素**。

选择器1 ~ 选择器2

```css
div~p {
    background-color:yellow;
}
```

**案例**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    div~p{
      color: red;
    }
  </style>
</head>
<body>
  <div>d1</div>
  <p>2</p>
  <p>3</p>
</body>
</html>
```



#### 伪类选择器

很像类，但不是类，是元素特殊状态的一种描述

作用：伪类选择器表示元素状态，选中某个元素的某个状态设置样式

使用方法：`选择器` `:伪类` `{CSS属性}`

常用伪类有

- `:hover` - 当用户将鼠标指针悬停在元素上时应用的样式
- `:focus` - 当元素获得键盘焦点时应用的样式，例如通过Tab键导航到该元素

> 个人感觉，CSS伪类选择器的功能类似于面向对象编程中基于对象状态自动调用特定方法
>
> 其允许我们针对元素的不同状态定义和应用不同的样式规则，从而在不编写额外脚本的情况下实现元素外观的动态变化



##### 动态伪类



|  选择器  |             作用             |
| :------: | :--------------------------: |
|  :link   |         没有访问过的         |
| :visited |           访问过的           |
|  :hover  |           鼠标悬停           |
| :active  | 点击时(按下不动可以看到效果) |
|  :focus  |    元素被获取焦点时被选中    |

> 如果要给超链接同时设置上表中多个状态，需要按 LVHA 的顺序书写

去除超链接默认

```css
a {
    color: inherit; /* 使用父元素的颜色 */
    text-decoration: none;
}
```

**鼠标悬停，让隐藏的部分显示出来**

方法一：使用 `display` 属性（推荐用于完全隐藏/显示块级元素）

```
/* 默认隐藏 */
.hidden-content {
    display: none;
}

/* 父元素悬停时显示 */
.parent:hover .hidden-content {
    display: block; /* 或 inline-block, flex 等 */
}
```



```
<div class="parent">
    悬停我
    <div class="hidden-content">
        这是隐藏的内容
    </div>
</div>
```

> ⚠️ 注意：`display: none` 会完全从文档流中移除元素，不能直接用于过渡动画。

------

方法二：使用 `opacity` 和 `visibility`（支持过渡动画）

```
.hidden-content {
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.3s ease, visibility 0.3s ease;
}

.parent:hover .hidden-content {
    opacity: 1;
    visibility: visible;
}
```



```
<div class="parent">
    悬停我
    <div class="hidden-content">
        这是隐藏的内容
    </div>
</div>
```

> ✅ 优点：可以添加平滑的淡入淡出效果。

------

方法三：使用 `transform` 实现滑动/缩放效果



```css
.hidden-content {
    opacity: 0;
    transform: translateY(-10px); /* 初始位置偏移 */
    visibility: hidden;
    transition: all 0.3s ease;
}

.parent:hover .hidden-content {
    opacity: 1;
    transform: translateY(0);
    visibility: visible;
}
```

> ✅ 优点：可以实现滑入、缩放等动效，用户体验更好。

------

方法四：结合 `overflow: hidden` 实现区域裁剪



```
.parent {
    overflow: hidden; /* 隐藏溢出内容 */
    height: 50px;
    transition: height 0.3s ease;
}

.parent:hover {
    height: 150px; /* 悬停时展开 */
}
```

> 适用于手风琴、展开面板等效果。

------

实际应用示例：下拉菜单

```
.menu {
    position: relative;
}

.dropdown {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    background: #333;
    color: white;
    padding: 10px;
}

.menu:hover .dropdown {
    display: block;
}
```



##### 结构伪类

###### **常用的伪类选择器**

1. **:first-child**：所有兄弟元素中的第一个。
2. **:last-child**：所有兄弟元素中的最后一个。
3. **:nth-child(n)**：所有兄弟元素中的第 n 个。
4. **:first-of-type**：所有同类型兄弟元素中的第一个。
5. **:last-of-type**：所有同类型兄弟元素中的最后一个。
6. **:nth-of-type(n)**：所有同类型兄弟元素中的第 n 个。

**关于 n 的值：**

1. **0 或 不写**：什么都选不中——几乎不用。
2. **n**：选中所有子元素——几乎不用。
3. **1~正无穷的整数**：选中对应序号的子元素。
4. **2n 或 even**：选中序号为偶数的子元素。
5. **2n+1 或 odd**：选中序号为奇数的子元素。
6. **-n+3**：选中的是前 3 个。

**伪类选择器**

1. **:nth-last-child(n)**：所有兄弟元素中的倒数第 n 个。
2. **:nth-last-of-type(n)**：所有**同类型**兄弟元素中的倒数第 n 个。
3. **:only-child**：选择没有兄弟的元素（独生子女）。
4. **:only-of-type**：选择没有同类型兄弟的元素。
5. **:root**：根元素。
6. **:empty**：内容为空元素（空格也算内容）。



##### **否定伪类**

：not(选择器) 排除满足括号中条件的元素

```html
    <style>
        /* 选中的是div的儿子p元素，但是排除类名为fail的元素 */
        div>p:not([title^="加油"]) {
            color: #067234;
        }
    </style>
</head>

<body>
    <div>
        <span>ceshi</span>
        <p>测试2</p>
        <p>张三</p>
        <p>王五</p>
        <p>赵六</p>
        <p class="fail" title="加油">第一个</p>
        <p class="fail" title="加油">第二个</p>
        <p>第三个</p>
        <span>ceshi2</span>
    </div>
```



##### UI伪类

1. **:checked**：被选中的复选框或单选按钮。
2. **:enable**：可用的表单元素（没有 `disabled` 属性）。
3. **:disabled**：不可用的表单元素（有 `disabled` 属性）。

```html
    <style>
        input:checked {
            width: 100px;
            height: 100px;
        }

        input:enabled {
            background-color: green;
        }

        input:disabled {
            background-color: grey;
        }
    </style>
</head>

<body>
    <input type="checkbox">
    <input type="radio" name="gender">
    <input type="radio" name="gender">
    <input type="text">
    <input type="text" disabled>
</body>
```



##### 目标伪类

：target	选中锚点指向的元素

```html
    <style>
        div {
            background-color: #e55599;
            height: 300px;
        }

        div:target {
            background-color: #999999;
        }
    </style>
</head>

<body>
    <a href="#one">去看第一个</a>
    <a href="#two">去看第二个</a>
    <a href="#three">去看第三个</a>
    <a href="#four">去看第四个</a>
    <a href="#five">去看第五个</a>
    <br>
    <div id="one">第一个</div>
    <br>
    <div id="two">第二个</div>
    <br>
    <div id="three">第三个</div>
    <br>
    <div id="four">第四个</div>
    <br>
    <div id="five">第六个</div>
    <br>
</body>

```



##### 语言伪类

：lang（语言类型，例：en,zh-CN） 根据指定的语言选择元素（本质是看lang属性的本质）

```html
    <style>
        div:lang(en) {
            color: #889999;
        }

        div:lang(zh-CN) {
            color: blueviolet;
        }
    </style>
</head>

<body>
    <div>尚硅谷</div>
    <div lang="en">atguigu</div>
    <p>前端</p>
    <span>你好</span>
</body>
```



#### 属性选择器

| 选择器           | 示例            | 示例说明                                   |
| ---------------- | --------------- | ------------------------------------------ |
| attribute        | [target]        | 选择所有带有target属性元素                 |
| attribute=value  | [target=_blank] | 选择所有使用target="-blank"的元素          |
| attribute~=value | [title~=flower] | 选择标题属性**包含单词**"flower"的所有元素 |

**属性选择器**

1.  所有带target的元素
2.  选择具有特定target属性值的元素
3.  选中具有title属性，且属性值以字母 a 开头的元素
4.  选中具有title属性，且属性值以字母 u 结尾的元素
5.  选中具有title属性，且属性值包含字母 u 的元素

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    /* 所有带target的元素 */
    [target] {
      color: red;
    }

    /* 选择具有特定target属性值的元素 */
    [target="_blank"] {
      font-weight: bold;
    }

    /* 选择标题属性中包含特定单词的元素 */
    [title~=flower] {
      background-color: yellow;
    }
      
     /*险种具有title属性，且属性值以字母 a 开头的元素*/
     [title^="a"]{
          color:red;
     }
      
      /*选中具有title属性，且属性值以字母 u 结尾的元素*/
      [title$ = "u"]{
		color:red;
      }
      
      /*选中具有title属性，且属性值包含字母 u 的元素*/
      [title* = "u"]{
		color:red;
      }
  </style>
</head>

<body>
  <a href="https://www.example.com" target="_blank">Example 1</a>
  <a href="https://www.example2.com">Example 2</a>
  <a href="https://www.example3.com" target="_self">Example 3</a>

  <p title="flower garden">This is a flower garden.</p>
  <p title="flower pot">This is a flower pot.</p>
  <p title="garden">This is a garden.</p>
</body>

</html>
```



#### 伪元素选择器

很像元素，但不是元素，是元素中的一些特殊位置

- **作用**：选中元素中的一些特殊位置。
- **常用伪元素**：
  - `::first-letter` 选中元素中的**第一个**文字。
  - `::first-line` 选中元素中的**第一行**文字。
  - `::selection` 选中被**鼠标选中**的内容。
  - `::placeholder` 选中**输入框**的提示文字。
  - `::before` 在元素**最开始**的位置，创建一个子元素（必须用 `content` 属性指定内容）。
  - `::after` 在元素**最后**的位置，创建一个子元素（必须用 `content` 属性指定内容）。

**案例1：**

```html
    <style>
        /* 伪元素选择器 */
        /* 选中的是p元素最开始的位置，随后创建一个子元素 */
        p::before {
            content: "￥";
        }

        /* 选中的是p元素最最后的位置，随后创建一个子元素 */
        p::after {
            content: ".00";
        }
    </style>
</head>

<body>
    <!-- 伪元素选择器 -->
    <p>199</p>
    <p>446</p>
    <p>2345</p>
    <p>567</p>
    <p>245</p>
    <p>3568</p>

</body>
```

**案例2：**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>示例 2</title>
    <style>
      li:after {
          content: " ✔";
      }

      li:before {
          content: "👉 ";
      }
  </style>
</head>

<body>
    <ul>
        <li>苹果</li>
        <li>香蕉</li>
        <li>橙子</li>
    </ul>
</body>

</html>
```

**案例3：**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        a:after {
            content: " 🔗";
        }

        a:before {
            content: "🌐 ";
        }
    </style>
    <title>示例 3</title>
</head>

<body>
    <a href="https://www.example.com">示例网站</a>
    <a href="https://www.google.com">谷歌</a>
</body>

</html>
```

> 更多案例：https://juejin.cn/post/6854573204011221000?searchId=20250304161555AB9052027619DCBA5761

> E是指定的标签或选择器，本选择器相当于给父标签添加个子级元素，在标签内部添加装饰性的元素

注意点：

- 必须设置 content:"  " 属性，否则元素不生效，content用来设置 伪元素的内容，如果没有内容，引号留空即可
- 伪元素默认是行内显示模式（也就是说，无法手动设置宽高，除非使用display转换显示模式）
- 权重和标签选择器相同





### 属性

可以控制元素

#### 常用属性

键值对：通常，我们将属性名与属性值成对出现的属性叫键值对

| 属性名           | 说明     |
| ---------------- | -------- |
| color            | 文字颜色 |
| font-size        | 字体大小 |
| width            | 宽度     |
| height           | 高度     |
| background-color | 背景色   |
|                  |          |
|                  |          |
|                  |          |
|                  |          |







#### 字体属性

字体属性表

| 名称         | 属性名            | 说明               |
| ------------ | ----------------- | ------------------ |
| 字体大小     | font-size         | 修改文字大小       |
| 字体粗细     | font-weight       | 修改文字粗细       |
| 字体倾斜     | font-style        | 使文字倾斜         |
| 行高         | line-height       | 修改行高           |
| 字体族       | font-family       | 修改字体，如宋体   |
| 字体复合属性 | font              | 复合属性           |
| 文本缩进     | text-indent  (em) | 修改前后缩进       |
| 文本对齐     | text-align        | 修改文本对齐方式   |
| 修饰线       | text-decoration   | 上中下贯穿文本的线 |
| 颜色         | color             | 修改文字颜色       |

##### 引入自定义字体

属性名：`@font-face{ }`

引入字体后无需客户端安装，自动使用引入的字体

```css
@font-face {
    font-family:bbt;/*字体名叫bbt*/
    src: url(../btt.ttf);/*相对路径引入*/
}
```



##### 字体大小

属性名：font-size

属性值：文字尺寸，PC 端网页常用单位 `px`

> 通常来说，谷歌浏览器默认字体大小为16px



##### 字体粗细

属性名：font-weight

属性值：

- **数字**

正常为400，加粗为800

- **关键字**

正常：`normal` ，加粗：`bold`



##### 字体倾斜

属性名：font-style

属性值：不倾斜 `nomal`   倾斜 `italic`



##### 行高

作用：设置多行文本的间距

属性名：line-height

属性值：

- 数字 + px
- 数字（当前标签font-size属性值的倍数）



##### 字体族

属性名：font-family

属性值：字体名

font-family属性值可以书写多个字体名，各个字体名用 逗号 隔开，执行顺序从左到右依次查找

其最后一个属性可以设置一个字体族名，其作用为 当前面的字体皆未找到，将使用通用的字体族，比如 sans-seif 为无衬线字体

```css
font-family:楷体;

font-family:Microsoft YaHei,Heiti SC,tahoma,arial,Hiragino Sans GB,"\5B8B\4F53",sans-seif;
```



##### font复合属性

复合属性：属性的间歇方式，一个属性对应多个值的写法，各个属性之间用空格隔开

font： 是否倾斜 是否加粗 字号/行高 字体（必须按顺序书写）

注意：字号和字体值必须书写也必须按顺序书写，否则 font 属性不生效

就是把上面的属性合成一行，食用方法如下

```css
/*font：是否倾斜 是否加粗 字号/行高 字体;*/
font: italic 700 30px/2 楷体; 
```

```css
font-style         规定文本的字体样式。
font-weight        规定字体是否加粗
font-size          规定字体的大小，通常是以 px 为单位
font-family        规定文本的字体系列（字体族）
line-height        设置行高
 
 
font-style: italic;
font-weight: 400;
font-size: 20px;
line-height: 200px;
font-family: "宋体";
```



##### web字体

可以通过 `@font-face` 指定字体的具体地址，浏览器会自动下载该字体，这样就不依赖用户电脑上的字体了。

语法（简写方式）

```css
@font-face {
    font-family: "情书字体";
    src: url('./方正手迹.ttf');
}
```

语法（高兼容性写法）

```css
@font-face {
    font-family: "atguigu";
    font-display: swap;
    src: url('webfont.eot'); /* IE9 */
    src: url('webfont.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */
         url('webfont.woff2') format('woff2'),
         url('webfont.woff') format('woff'), /* chrome、firefox */
         url('webfont.ttf') format('truetype'), /* chrome、firefox、opera、Safari, Android*/
         url('webfont.svg#webfont') format('svg'); /* iOS 4.1- */
}
```

定制字体

- 中文的字体文件很大，使用完整的字体文件不现实，通常针对某几个文字进行单独定制。
- 可使用阿里 Web 字体定制工具： https://www.iconfont.cn/webfont



#### 文本属性

##### 文本缩进

属性名：text-indent

属性值：

- 数字 + px
- 数字 + em（1em = 当前标签的字号大小）

经常用来首行空两格，em就相当于一个字，会随字号更改，所以使用em更多



##### 文本对齐

作用：控制内容水平对齐方式

属性名：text-align

属性值：

| 属性值 | 效果           |
| ------ | -------------- |
| left   | 左对齐（默认） |
| center | 居中对齐       |
| right  | 右对齐         |

text-align本质使控制内容的对齐方式，属性要设置给内容的父级

举个栗子：让图片居中不能在 `<img>` 标签中使用属性，需要给其父标签添加属性



##### 文本间距

- **字母间距**：`letter-spacing`
- **单词间距**：`word-spacing`（通过**空格**识别词）
- **属性值为像素（px），正值让间距增大，负值让间距缩小。**



##### 文本阴影

在 CSS3 中，我们可以使用 `text-shadow` 属性给文本添加阴影。

语法：

```css
text-shadow: h-shadow v-shadow blur color;
```

| 值         | 描述                                   |
| ---------- | -------------------------------------- |
| `h-shadow` | 必需写，**水平**阴影的位置。允许负值。 |
| `v-shadow` | 必需写，**垂直**阴影的位置。允许负值。 |
| `blur`     | 可选，模糊的距离。                     |
| `color`    | 可选，阴影的颜色                       |

默认值：

- `text-shadow: none` 表示没有阴影。



##### 文本换行

在 CSS3 中，我们可以使用 `white-space` 属性设置文本换行方式。

常用值如下：

| 值         | 含义                                                         |
| ---------- | ------------------------------------------------------------ |
| `normal`   | 文本超出边界自动换行，文本中的换行被浏览器识别为一个空格。（默认值） |
| `pre`      | 原样输出，与 `<pre>` 标签的效果相同。                        |
| `pre-wrap` | 在 `pre` 效果的基础上，超出元素边界自动换行。                |
| `pre-line` | 在 `pre` 效果的基础上，超出元素边界自动换行，且只识别文本中的换行，空格会忽略。 |
| `nowrap`   | 强制不换行                                                   |



##### 文本溢出

在 CSS3 中，我们可以使用 `text-overflow` 属性设置文本内容溢出时的呈现模式。

常用值如下：

| 值         | 含义                                           |
| ---------- | ---------------------------------------------- |
| `clip`     | 当内联内容溢出时，将溢出部分裁切掉。（默认值） |
| `ellipsis` | 当内联内容溢出块容器时，将溢出部分替换为 ...   |

注意：

要使得 `text-overflow` 属性生效，块容器必须显式定义 `overflow` 为非 `visible` 值，`white-space` 为 `nowrap` 值。

```css
.text {
  width: 200px;
  white-space: nowrap;           /* 禁止换行 */
  overflow: hidden;              /* 隐藏溢出 */
  text-overflow: ellipsis;       /* 显示省略号 */
}
```



##### 文本修饰

CSS3 升级了 `text-decoration` 属性，让其变成了复合属性。

```css
text-decoration: text-decoration-line || text-decoration-style || text-decoration-color;
```

子属性及其含义：

- **`text-decoration-line`** 设置文本装饰线的位置
  - `none`：指定文字无装饰（默认值）
  - `underline`：指定文字的装饰是下划线
  - `overline`：指定文字的装饰是上划线
  - `line-through`：指定文字的装饰是贯穿线
- **`text-decoration-style`** 文本装饰线条的形状
  - `solid`：实线（默认）
  - `double`：双线
  - `dotted`：点状线条
  - `dashed`：虚线
  - `wavy`：波浪线
- **`text-decoration-color`** 文本装饰线条的颜色



##### 文本描边

注意：文字描边功能仅 **webkit** 内核浏览器支持。

- `-webkit-text-stroke-width`：设置文字描边的宽度，写长度值。
- `-webkit-text-stroke-color`：设置文字描边的颜色，写颜色值。
- `-webkit-text-stroke`：复合属性，设置文字描边宽度和颜色。





##### 行高

 属性名：`line-height`

- **可选值**：

  1. `normal`：由浏览器根据文字大小决定的一个默认值。
  2. 像素 (`px`)。
  3. 数字：参考自身 `font-size` 的倍数（很常用）。
  4. 百分比：参考自身 `font-size` 的百分比。

- **备注**：由于字体设计原因，文字在一行中，并不是绝对垂直居中，若一行中都是文字，不会太影响观感。

- **举例**：

  ```css
  div {
    line-height: 60px;
    line-height: 1.5;
    line-height: 150%;
  }
  ```

**注意事项**：

行高注意事项：

1. `line-height` 过小会怎样？—— 文字产生重叠，且最小值是 0，不能为负数。

2. `line-height` 是可以**继承的**，且为了能更好的呈现文字，最好写数值。

3. ```
   line-height
   ```

   和

   ```
   height
   ```

   是什么关系？

   - 设置了 `height`，那么高度就是 `height` 的值。
   - 不设置 `height` 的时候，会根据 `line-height` 计算高度。

应用场景：

1. 对于多行文字：控制行与行之间的距离。
2. 对于单行文字：让 `height` 等于 `line-height`，可以实现文字垂直居中。



**文本对齐_垂直**

1. **顶部**：无需任何属性，在垂直方向上，默认就是顶部对齐。

2. **居中**：对于单行文字，让 `height = line-height` 即可。

   - **问题**：多行文字垂直居中怎么办？——后面我们用定位去做。

3. **底部**：对于单行文字，目前一个临时的方式：

   - 让

     ```css
     line-height = (height × 2) - font-size - x
     ```

     - **备注**：`x` 是根据字体族，动态决定的一个值。

- **问题**：垂直方向上的底部对齐，更好的解决办法是什么？——后面我们用定位去做。



##### vertical-align	基线对齐

属性名：`vertical-align`

- **作用**：用于指定同一行元素之间，或表格单元格内文字的垂直对齐方式。
- **常用值**：
  1. `baseline`（默认值）：使元素的基线与父元素的基线对齐。
  2. `top`：使元素的顶部与其所在行的顶部对齐。
  3. `middle`：使元素的中部与父元素的基线加上父元素字母 x 的一半对齐。
  4. `bottom`：使元素的底部与其所在行的底部对齐。
- **特别注意**：`vertical-align` 不能控制块元素。



##### 文本修饰线

属性名：text-decoation
属性值：

| 属性值       | 效果   |
| ------------ | ------ |
| none         | 无     |
| underline    | 下划线 |
| line-through | 删除线 |
| overline     | 上划线 |



##### 文字颜色

属性名：color

属性值：

| 表示方法       | 属性值        | 说明                            |
| -------------- | ------------- | ------------------------------- |
| 颜色关键字     | 颜色英文单词  | red、green、blue                |
| rgb表示法      | rgb(r,g,b)    | r,g,b表示红绿蓝三原色           |
| rgba表示法     | rgba(r,g,b,a) | a表示透明度，取值0-1            |
| 十六进制表示法 | #RRGGBB       | #000000，#ffcc00 简写:#000,#fc0 |

###### 表示方式一：颜色名

- **编写方式**：直接使用颜色对应的英文单词，编写比较简单，例如：

  1. 红色: red
  2. 绿色: green
  3. 蓝色: blue
  4. 紫色: purple
  5. 橙色: orange
  6. 灰色: gray .......

- **说明**：

  1. 颜色名这种方式，表达的颜色比较单一，所以用的并不多。
  2. 具体颜色名参考 MDN 官方文档:
     - https://developer.mozilla.org/en-US/docs/Web/CSS/named-color

  

###### 表示方式二：rgb 或 rgba

- **编写方式**：使用红、黄、蓝这三种光的三原色进行组合。
  - r 表示红色
  - g 表示绿色
  - b 表示蓝色
  - a 表示透明度
- **举例**：

```css
/* 使用0~255之间的数字表示一种颜色 */
color: rgb(255, 0, 0); /* 红色 */
color: rgb(0, 255, 0); /* 绿色 */
color: rgb(0, 0, 255); /* 蓝色 */
color: rgb(0, 0, 0); /* 黑色 */
color: rgb(255, 255, 255); /* 白色 */

/* 混合出任意一种颜色 */
color: rgb(138, 43, 226); /* 紫罗兰色 */
color: rgba(255, 0, 0, 0.5); /* 半透明的红色 */

/* 也可以使用百分比表示一种颜色（用的少） */
color: rgb(100%, 0%, 0%); /* 红色 */
color: rgba(100%, 0%, 0%, 50%); /* 半透明的红色 */
```

- 小规律 
  1. 若三种颜色值相同，呈现的是灰色，值越大，灰色越浅。
  2. `rgb(0, 0, 0)` 是黑色，`rgb(255, 255, 255)` 是白色。
  3. 对于 `rgba` 来说，前三位的 `rgb` 形式要保持一致，要么都是 `0~255` 的数字，要么都是百分比。



###### 表示方式三：HEX 或 HEXA

**HEX 的原理同与 rgb 一样，依然是通过：红、绿、蓝色进行组合，只不过要用 6 个数字，分成 3 组来表达，格式为：#rrggbb**

- **每一位数字的取值范围是：0 ~ f ，即：（0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, f）**
- **所以每一种光的最小值是：00，最大值是：ff**

```css
color: #ff0000; /* 红色 */
color: #00ff00; /* 绿色 */
color: #0000ff; /* 蓝色 */
color: #000000; /* 黑色 */
color: #ffffff; /* 白色 */

/* 如果每种颜色的两位都是相同的，就可以简写 */
color: #ff9988; /* 可简写为：#f98 */

/* 但要注意前三位简写了，那么透明度就也要简写 */
color: #ff998866; /* 可简写为：#f986 */
```

**注意点：IE 浏览器不支持 HEXA，但支持 HEX。**



######  表示方式四：HSL 或 HSLA

- **HSL 是通过： 色相、饱和度、亮度，来表示一个颜色的，格式为：hsl(色相, 饱和度, 亮度)**

  - **色相**

    ：取值范围是 0~360 度，具体度数对应的颜色如下图：

    - Red: 0°
    - Yellow: 60°
    - Green: 120°
    - Cyan: 180°
    - Blue: 240°
    - Magenta: 300°

  - **饱和度**：取值范围是 0%~100%。（向色相中对应颜色中添加灰色，0% 全灰，100% 没有灰）

  - **亮度**：取值范围是 0%~100%。（0% 亮度没了，所以就是黑色。100% 亮度太强，所以就是白色了）

- **HSLA 其实就是在 HSL 的基础上，添加了透明度。**



##### 不透明度opacity

`opacity` 属性能为整个元素添加透明效果，值是 0 到 1 之间的小数，0 是完全透明，1 表示完全不透明。

**`opacity` 与 `rgba` 的区别？**

- **`opacity`** 是一个属性，设置的是整个元素（包括元素里的内容）的不透明度。
- **`rgba`** 是颜色的设置方式，用于设置颜色，它的透明度，仅仅是调整颜色的透明度



#### 背景属性

##### 背景图

属性名：background-image(bgi)

属性值：url(背景图的 URL)

在网页中，使用背景图实现 **装饰性** 的图片效果



举个栗子

```css
div{
    width: 400px;
    height: 400px;
    
    background-image: url(./images/1.png);
    
}
```

为以上例子做解释，设置 div标签 样式为宽高400px，并且将背景图设置为相对路径的1.png



> 提示：在浏览器中，背景图默认是平铺的效果，也就是容器的尺寸大就会复制几张填充满；同时，因为是背景图，div标签中有文字将显示在图片之上



##### 背景图平铺方式

属性名：background-repeat (bgr)

属性值：

| 属性值    | 效果             |
| --------- | ---------------- |
| no-repeat | 不平铺           |
| repeat    | 平铺（默认效果） |
| repeat-x  | 水平方向平铺     |
| repeat-y  | 垂直方向平铺     |

以下是对各个属性值效果的描述：

- no-repeat：只有一张图片，显示在容器的左上角不会扩展
- repeat：复制图片填满容器
- repeat-x：只有横向复制图片
- repeat-y：只有竖向复制图片



##### 背景图位置

属性名：background-position (bgp)

属性值：水平方向位置 垂直方向位置

关键字：

| 关键字 | 位置 |
| ------ | ---- |
| left   | 左侧 |
| right  | 右侧 |
| center | 居中 |
| top    | 顶部 |
| bottom | 底部 |

坐标： 数字 + px  /  关键字

注意事项：

- 数字可以与关键字混用

- 数字正负皆可

- 数字是从容器左上角计算

- 水平方向正数向右移动，负数像左侧移动；

- 垂直方向正数向下移动，负数向上移动；

  * top: 50%;     /* 向下移动 50% 的父元素高度 */

  * left: 50%;      /* 向右移动 50% 的父元素宽度 */

- 超出容器的部分会被裁切

**特殊提醒：**

- 关键字取值方式写法，可以颠倒取值顺序
- 可以只写一个关键字，另一个方向默认居中；数字只写一个值表示水平方向，垂直方向为居中



##### 背景图缩放

属性名：background-size (bgz)

作用：设置背景图大小

常用属性值：

- 关键字

​	cover：等比例缩放背景图片以**完全覆盖背景区**，可能背景图部分看不见

​	contain：等比例缩放背景图片以完全装入背景区，可能背景区部分空白

- 百分比：根据容器尺寸计算图片大小，注意：100%表示图片的宽度跟容器的宽度一样，图片的高度按照图片比例等比例缩放
- 数字 + 单位（例如：px）



##### 背景图固定

属性名：background-attachment (bga)

属性值：fixed

作用：背景不会随着元素的内容滚动



##### 背景图原点

background-origin

它用于**定义背景图像（`background-image`）的定位起点（即坐标原点 `(0,0)` 的位置）**。

- **作用**：设置背景图的原点。
- **语法**
  1. `padding-box`：从 padding 区域开始显示背景图像。--- 默认值
  2. `border-box`：从 border 区域开始显示背景图像。
  3. `content-box`：从 content 区域开始显示背景图像。



##### background-clip

它控制**背景（包括背景图和背景色）的绘制区域**，即“裁剪”到哪个盒子。

- `background-clip: border-box`(默认)
  - 背景绘制到边框区域下。
- `background-clip: padding-box`
  - 背景绘制到内边距区域，不绘制在边框下。
- `background-clip: content-box`
  - 背景只绘制在内容区域。

> ✅ **注意**：`background-clip` 是向“内”裁剪，即决定背景能画到哪个区域为止，而不是“向外裁剪”。

- **作用**：设置背景图的向外裁剪的区域。
- **语法**
  1. `border-box`：从 border 区域开始向外裁剪背景。--- 默认值
  2. `padding-box`：从 padding 区域开始向外裁剪背景。
  3. `content-box`：从 content 区域开始向外裁剪背景。
  4. `text`：背景图只呈现在文字上。
- **注意**：若值为 `text`，那么 `background-clip` 要加上 `-webkit-` 前缀。



#####  背景图尺寸

background-size

- **作用**：设置背景图的尺寸。

- **语法**

  1. **用长度值指定背景图片大小，不允许负值。**

     ```css
     background-size: 300px 200px;
     ```

  2. **用百分比指定背景图片大小，不允许负值。**

     ```css
     background-size: 100% 100%;
     ```

  3. **`auto`**：背景图片的真实大小。--- 默认值

  4. **`contain`**：将背景图片等比缩放，使背景图片的宽或高，与容器的宽或高相等，再将完整背景图片包含在容器内，但要注意：可能会造成容器里部分区域没有背景图片。

     ```css
     background-size: contain;
     ```

  5. **`cover`**：将背景图片等比缩放，直到**完全覆盖容器**，图片会尽可能全的显示在元素上，但要注意：背**景图片有可能显示不完整**。--- 相对比较好的选择

     ```css
     background-size: cover;
     ```





##### 背景复合属性

属性名：background (bg)

属性值：背景色 背景图 背景图平铺方式 背景图位置/背景图缩放 背景图固定（空格隔开各个属性值，不区分顺序）

> 类似于字体复合属性值，就是一条写出整个背景图的属性

```css
div()
{
    width: 400px;
    height: 400px;
    
    background: pink url(./images/1.png) no-repeat right center/cover;
}
```

> 翻一下就是背景粉色，图片为1.png，不平铺，水平靠右侧，垂直居中，等比例缩放完全覆盖容器，可能有截取

语法：

```css
background: color url repeat position / size origin clip
```

注意：

1. `origin` 和 `clip` 的值如果一样，如果只写一个值，则 `origin` 和 `clip` 都设置；如果设置了两个值，前面的是 `origin`，后面的 `clip`。
2. `size` 的值必须写在 `position` 值的后面，并且用 `/` 分开。



##### 多背景图

background-repeat

允许元素设置多个背景图片

语法如下：

```css
background-repeat: repeat-x | repeat-y | repeat | no-repeat | space | round | [ <repeat-style> ]#
```

- **`repeat`**：默认值。背景图像在水平和垂直方向上都重复。
- **`repeat-x`**：仅在水平方向上重复。
- **`repeat-y`**：仅在垂直方向上重复。
- **`no-repeat`**：背景图像不重复。
- **`space`**：尽可能多地重复背景图像，然后在剩余空间内**均匀分布**（不会裁剪图像）。
- **`round`**：尽可能多地重复背景图像，并根据需要缩放图像以**填满元素。**

对于多背景图的情况，你可以这样指定不同的重复方式：

```css
.element {
  background-image: url(image1.png), url(image2.png);
  background-repeat: repeat, no-repeat;
}
```

在这个例子中，`image1.png` 将会在两个方向上重复 (`repeat`)，而 `image2.png` 将不会重复 (`no-repeat`)。

**注意事项**

- 如果你为 `background-repeat` 提供的值少于背景图的数量，最后一个值会被应用到所有的剩余背景图上。
- 同样地，如果只提供了一个值，那么这个设置将应用于所有背景图。

**实例**

假设我们有如下CSS代码：

```css
div {
  background-image: url('img1.png'), url('img/XMLSchema.png');
  background-repeat: no-repeat, repeat-y;
}
```

这里，`img1.png` 不会重复 (`no-repeat`)，而 `img/XMLSchema.png` 只在垂直方向上重复 (`repeat-y`)。

这种方式使你可以非常灵活地控制不同背景图的行为，以实现所需的视觉效果。





#### 列表属性

| CSS 属性名          | 功能               | 属性值                                                       |
| ------------------- | ------------------ | ------------------------------------------------------------ |
| list-style-type     | 设置列表符号       | - `none`：不显示标识<br> - `square`：实心方块<br> - `disc`：圆形<br> - `decimal`：数字<br> - `lower-roman`：小写罗马字<br> - `upper-roman`：大写罗马字<br> - `lower-alpha`：小写字母<br> - `upper-alpha`：大写字母 |
| list-style-position | 设置列表符号的位置 | - `inside`：在 li 内部<br> - `outside`：在 li 外部           |
| list-style-image    | 自定义列表符号     | `url(图片地址)`                                              |
| list-style          | 复合属性（简写）   | 同时设置 `list-style-type`、`list-style-position`、`list-style-image`（无顺序要求） |

**解释**

1. **list-style-type**

   - 控制列表项符号类型（如 `disc`、`decimal` 等），`none` 可隐藏符号。

2. **list-style-position**

   - `inside`：符号嵌入文本行内；`outside`：符号独立于文本左侧。

3. **list-style-image**

   - 通过 URL 替换默认符号为自定义图片（需确保图片路径有效）。

4. **list-style**

   - 简写属性，支持同时设置三种属性，顺序无关，如：

     ```css
     list-style: square inside url(icon.png);
     ```



#### 边框属性（其他元素也能用）

| CSS 属性名    | 功能         | 属性值                                                       |
| :------------ | ------------ | ------------------------------------------------------------ |
| border-width  | 边框宽度     | CSS 中可用的长度值                                           |
| border-color  | 边框颜色     | CSS 中可用的颜色值                                           |
| border-style  | 边框风格     | - `none` 默认值<br> - `solid` 实线<br> - `dashed` 虚线<br> - `dotted` 点线<br> - `double` 双实线 |
| border        | 边框复合属性 | 没有数量、顺序的要求                                         |
| border-radius | 边框圆角     |                                                              |
| outline       | 边框外轮廓   |                                                              |

注意：

1. 以上 4 个边框相关的属性，其他元素也可以用，这是我们第一次遇见它们。
2. 在后面的盒子模型中，我们会详细讲解边框相关的知识。



#### 表格独有属性

| CSS 属性名      | 功能                            | 属性值                                                       |
| --------------- | ------------------------------- | ------------------------------------------------------------ |
| table-layout    | 设置列宽度                      | - `auto`：自动，列宽根据内容计算（默认值）。<br> - `fixed`：固定列宽，平均分配。 |
| border-spacing  | 单元格间距                      | - CSS 长度值（如 `10px`）。<br> - 生效前提：单元格边框不合并。 |
| border-collapse | 合并单元格边框                  | - `collapse`：合并。<br> - `separate`：不合并（默认值）。    |
| empty-cells     | 控制空单元格显示                | - `show`：显示（默认值）。<br> - `hide`：隐藏。<br> - 生效前提：单元格不合并。 |
| caption-side    | 设置表格标题 (`<caption>`) 位置 | - `top`：标题在表格上方（默认值）。<br> - `bottom`：标题在表格下方。 |





#### 布局属性

------

##### 容器大小最值

**最小 `min-height` 属性**

- **定义**：指定一个元素的最小高度。即使内容较少，元素的高度也不会低于这个值。

- **语法**：

  ```css
  min-height: <length> | <percentage>;
  ```

  - `<length>`：可以使用绝对单位如`px`、`cm`等；也可以使用相对单位如`em`、`rem`。
  - `<percentage>`：相对于包含块的高度百分比。

- **示例**：

  ```css
  .container {
      min-height: 200px;
  }
  ```

  这个例子确保了`.container`类至少有200px的高度，但如果内容更多，则会自动扩展。

**应用场景**

- 确保容器有足够的空间来容纳其内容。
- 在响应式设计中，为不同屏幕尺寸提供一致的最低高度。

---

**最大`max-height` 属性**

- **定义**：指定一个元素的最大高度。如果内容超出这个高度，通常会触发滚动条（需结合`overflow`属性使用），或者内容被隐藏（取决于其他样式设置）。

- **语法**：

  ```css
  max-height: <length> | <percentage>;
  ```

  类似于`min-height`，但这里是设置最大值。

- **示例**：

  ```css
  .content-box {
      max-height: 400px;
      overflow-y: auto; /* 超出部分显示垂直滚动条 */
  }
  ```

  此示例限制了`.content-box`的高度不超过400px，超出部分可通过滚动查看。

**应用场景**

- 控制图片或文本区域的最大尺寸，防止页面布局因内容过多而破坏。
- 结合`overflow`属性实现优雅的内容溢出处理方案。

---

**组合使用**

- 使用`min-height`和`max-height`组合可以创建更灵活的高度范围：

  ```css
  .flexible-container {
      min-height: 150px;
      max-height: 500px;
      overflow-y: auto;
  }
  ```

  这样，`.flexible-container`将至少有150px高，并且最多不会超过500px，超出部分可通过滚动查看。

**注意事项**

- 当使用百分比作为`min-height`或`max-height`的值时，需要确保父元素有一个明确的高度，否则百分比可能无法正确计算。
- 在某些情况下，特别是对于表格单元格（`td`或`th`），这些属性可能不起作用或行为有所不同，因为表格布局有自己的规则。

通过合理使用`min-height`和`max-height`，可以极大地增强网页布局的灵活性和适应性，特别是在响应式设计和动态内容加载场景下。







##### 垂直对齐方式

属性名：vertical-align (va)

属性值：

| 属性值      | 适用场景                 | 效果描述                                                     |
| ----------- | ------------------------ | ------------------------------------------------------------ |
| baseline    | 默认值                   | 元素的基线与父元素的基线对齐                                 |
| top         | 行内/表格元素            | 元素顶部与行/单元格的最高元素顶部对齐                        |
| middle      | 行内/表格元素            | 元素中线与父元素的基线+0.5ex高度对齐（表格中表现为垂直居中） |
| bottom      | 行内/表格元素            | 元素底部与行/单元格的最低元素底部对齐                        |
| text-top    | 行内元素                 | 元素顶部与父元素字体的顶端对齐                               |
| text-bottom | 行内元素                 | 元素底部与父元素字体的底端对齐                               |
| sub         | 特殊文本                 | 模拟`<sub>`标签效果，将基线降低到合适位置                    |
| super       | 特殊文本                 | 模拟`<sup>`标签效果，将基线提升到合适位置                    |
| 长度值      | 精确调整（如2px, 0.5em） | 相对于基线向上（正值）或向下（负值）移动                     |
| 百分比值    | 相对行高调整             | 根据元素的line-height值计算移动距离（如50%）                 |

以下是对核心属性值的补充说明：

- **baseline**：文本类元素（如`<span>`）默认对齐方式，图片底部会与基线对齐
- **middle**：在表格单元格中可实现真正垂直居中，但在行内元素中可能受字体影响
- **top/bottom**：对齐依据是当前行框(line box)的最高/最低元素，而非容器边界
- **text-top/text-bottom**：对齐标准是父元素的字体尺寸，而非实际内容高度

###### 注意事项

1. 仅对以下元素有效：

   - 行内元素（`display: inline`）
   - 行内块元素（`display: inline-block`）
   - 表格单元格（`display: table-cell`）

2. 常见无效场景：

   - 块级元素（需改用flex/grid布局）
   - 绝对定位元素
   - 浮动元素

3. 图片对齐建议：

   ```css
   img {
     vertical-align: middle; /* 消除图片底部间隙 */
   }
   ```

4. 表格特殊行为：

   ```css
   td {
     vertical-align: middle; /* 单元格内容垂直居中 */
   }
   ```

###### 总结图示

```
[父元素]
│
├── text-top ──────┐
├── baseline ──────┤ ← 基线与父元素文字对齐
├── text-bottom ──┤
│                  ↓
│  [子元素]        → 可用长度/百分比值微调
└── line-height区域
```





#### 修饰属性



##### 过渡动画属性

属性名：transition (trs)

属性值（简写语法）：

```css
transition: <property> <duration> <timing-function> <delay>;
/*常用就是这样的*/
transition: all 1s;
```

> 本属性写于标签本身的css，不要写在类似于hover的css中

###### 详细属性分解表

| 子属性                     | 属性值示例                          | 默认值 | 作用描述                                           |
| -------------------------- | ----------------------------------- | ------ | -------------------------------------------------- |
| transition-property        | all, width, opacity                 | all    | 指定应用过渡的CSS属性（多个属性用逗号分隔）        |
| transition-duration        | 0.3s, 500ms                         | 0s     | 定义动画持续时间（必须指定至少该属性才会触发动画） |
| transition-timing-function | ease, cubic-bezier(.17,.67,.83,.67) | ease   | 控制动画速度曲线                                   |
| transition-delay           | 0.2s, 100ms                         | 0s     | 设置动画开始前的延迟时间                           |

###### 缓动函数详解表

| 函数值                | 运动曲线特征         | 典型应用场景         |
| --------------------- | -------------------- | -------------------- |
| ease                  | 先加速后减速（默认） | 通用动画效果         |
| linear                | 匀速运动             | 进度条、机械运动     |
| ease-in               | 逐渐加速             | 物体下落效果         |
| ease-out              | 逐渐减速             | 弹窗关闭效果         |
| ease-in-out           | 对称加减速           | 页面切换过渡         |
| cubic-bezier(n,n,n,n) | 自定义贝塞尔曲线     | 需要特殊节奏的动画   |
| steps(n)              | 分步跳跃变化         | 帧动画、数字切换效果 |

###### 注意事项

1. **生效前提**：

   - 元素必须具有有效可过渡属性（如尺寸/位置/颜色等）
   - 需要明确的属性值变化触发（如:hover状态切换）

2. **性能优化**：

   ```css
   /* 优先使用以下高性能属性 */
   transform: translate/scale/rotate;
   opacity: 0-1;
   filter: 简单效果;
   ```

3. **多属性控制**：

   ```css
   /* 同时控制多个属性的过渡 */
   .box {
     transition: 
       transform 0.3s ease-out,
       opacity 0.2s linear 50ms;
   }
   ```

4. **隐式动画关闭**：

   ```css
   /* 强制禁用所有过渡 */
   .no-transition {
     transition: none !important;
   }
   ```

###### 最佳实践示例

```css
/* 基础悬停效果 */
.button {
  transition: all 0.3s ease;
  background: #3498db;
}
.button:hover {
  background: #2980b9;
  transform: translateY(-2px);
}

/* 级联动画控制 */
.card {
  transition: 
    opacity 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94),
    transform 0.4s 0.1s ease-out;
}
.card.hidden {
  opacity: 0;
  transform: scale(0.9);
}
```

###### 总结图示

```
[动画时间轴]
│         ↗↘
│       ↗    ↘       ease-in-out曲线示例
│     ↗        ↘
│   ↗            ↘
├───┐              ┌───►
0  delay         duration
```



##### 透明度控制

属性名：opacity (opa)

属性值：

| 属性值      | 效果描述                     |
| ----------- | ---------------------------- |
| 0           | 完全透明（元素不可见）       |
| 0~1之间数值 | 半透明（如0.5表示50%透明度） |
| 1           | 完全不透明（默认值）         |

###### 核心特性说明

- **继承性**：不继承，但子元素会受父元素透明度影响（实际表现为叠加计算）
- **作用范围**：影响元素**及其所有子元素**的可见度
- **布局特性**：透明元素仍占据文档流空间（与`visibility: hidden`不同）
- **性能表现**：支持GPU加速，适合用于动画过渡

###### `opacity` 与 `rgba` 的区别？

- **`opacity`** 是一个属性，设置的是整个元素（包括元素里的内容）的不透明度。
- **`rgba`** 是颜色的设置方式，用于设置颜色，它的透明度，仅仅是调整颜色的透明度

###### 属性值详解

- **0**：

  - 元素完全透明，但依然可交互（可点击/聚焦）
  - 常用于实现淡出效果或无障碍隐藏

  ```css
  .hidden { opacity: 0; }
  ```

- **0~1之间数值**：

  - 实现元素半透明效果
  - 叠加计算公式：`最终透明度 = 父元素opacity * 当前元素opacity`

  ```css
  .translucent { opacity: 0.7; }
  ```

- **1**：

  - 默认状态，元素完全不透明
  - 常用于重置继承的透明状态

  ```css
  .reset-opacity { opacity: 1 !important; }
  ```

###### 注意事项

1. **交互保留**：

   ```css
   /* 透明元素仍可交互 */
   .ghost-button {
     opacity: 0.5;
     pointer-events: none; /* 需额外添加该属性禁用交互 */
   }
   ```

2. **叠加特性**：

   ```html
   <!-- 父元素opacity:0.5，子元素opacity:0.6 → 实际显示0.3 -->
   <div class="parent">
     <div class="child"></div>
   </div>
   ```

3. **与RGBA的区别**：

   ```css
   /* 仅影响背景透明度（不影响子元素） */
   .bg-transparent { background: rgba(0,0,0,0.5); }
   
   /* 影响整个元素及子元素 */
   .element-transparent { opacity: 0.5; }
   ```

4. **动画优化**：

   ```css
   /* 优先使用opacity实现淡入淡出 */
   .fade-in {
     transition: opacity 0.3s ease;
     opacity: 1;
   }
   ```

###### 应用场景示例

1. 基础淡入效果：

   ```css
   .fade {
     opacity: 0;
     transition: opacity 0.4s ease-in;
   }
   .fade.active {
     opacity: 1;
   }
   ```

2. 模态框遮罩层：

   ```css
   .overlay {
     position: fixed;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     background: black;
     opacity: 0.6;
   }
   ```

3. 加载状态提示：

   ```css
   .loading {
     opacity: 0.8;
     transition: opacity 0.2s;
   }
   .loading:hover {
     opacity: 1;
   }
   ```

###### 总结图示

```
透明度层级
┌───────────────┐
│  父元素opa:0.6│
│  ┌───────────┐│
│  │ 子元素opa:0.5 → 实际显示0.3 │
│  └───────────┘│
└───────────────┘
```





##### 滤镜修饰

属性名：filter

属性值：常用 filter 函数

| 滤镜函数          | 描述                                            | 示例                                                         |
| ----------------- | ----------------------------------------------- | ------------------------------------------------------------ |
| `blur(px)`        | 高斯模糊，值越大越模糊                          | `filter: blur(3px);`                                         |
| `brightness(%)`   | 调整亮度                                        | `filter: brightness(50%);`（变暗）<br>`filter: brightness(1.5);`（更亮） |
| `contrast(%)`     | 调整对比度                                      | `filter: contrast(200%);`（增强对比）                        |
| `grayscale(%)`    | 变成灰度图                                      | `filter: grayscale(100%);`（完全黑白）                       |
| `hue-rotate(deg)` | 色相旋转                                        | `filter: hue-rotate(90deg);`                                 |
| `invert(%)`       | 反转颜色                                        | `filter: invert(100%);`（负片效果）                          |
| `opacity(%)`      | 设置透明度（类似透明但不影响布局）              | `filter: opacity(50%);`                                      |
| `saturate(%)`     | 饱和度                                          | `filter: saturate(200%);`（更鲜艳）                          |
| `sepia(%)`        | 棕褐色调（老照片效果）                          | `filter: sepia(100%);`                                       |
| `drop-shadow()`   | 添加阴影（类似 box-shadow，但支持透明度和形状） | `filter: drop-shadow(2px 2px 4px rgba(0,0,0,0.5));`          |

------

💡 实际示例

1. 图片悬停模糊变清晰

```css
img {
  filter: blur(5px);
  transition: filter 0.3s ease;
}

img:hover {
  filter: blur(0);
}
```

2. 黑白图片 + 鼠标移上去恢复彩色

```css
img {
  filter: grayscale(100%);
  transition: filter 0.4s;
}

img:hover {
  filter: grayscale(0);
}
```

3. 创建“毛玻璃”（磨砂玻璃）效果

```css
.glass {
  background: url('bg.jpg');
  backdrop-filter: blur(10px); /* 注意：这是 backdrop-filter */
  filter: brightness(0.9) contrast(1.2);
}
```

> ⚠️ 注意：`backdrop-filter` 是另一个属性，作用于元素背后的区域（如半透明菜单），需要单独启用（部分浏览器需前缀）。

------

🌐 浏览器兼容性

- `filter` 属性在现代浏览器中支持良好（Chrome、Firefox、Safari、Edge）。

- 对于旧版 IE 不支持。

- Safari 需要

  ```
  -webkit-
  ```

  前缀（某些版本）：

  ```
  -webkit-filter: blur(2px);
          filter: blur(2px);
  ```

------

❗ 注意事项

1. **性能影响**：过度使用 `filter`（尤其是 `blur`）可能影响页面渲染性能，特别是在动画中。

2. 与 opacity 区别

   ：

   - `opacity: 0.5` 会让整个元素（包括子元素）变透明。
   - `filter: opacity(50%)` 只影响当前元素的绘制层，有时更适合做局部透明处理。

3. **硬件加速**：使用 `filter` 会触发 GPU 加速，有助于提升动画流畅度。

------

✅ 小技巧：结合 transform 使用，

```css
.card:hover {
  filter: brightness(1.1) saturate(120%);
  transform: scale(1.02);
  transition: all 0.3s ease;
}
```





##### 光标/鼠标样式控制

属性名：cursor  

属性值：  

| 属性值                  | 适用场景       | 效果描述                                  |
| ----------------------- | -------------- | ----------------------------------------- |
| default                 | 默认状态       | 浏览器默认光标（通常为箭头）              |
| pointer                 | 可点击元素     | 手形光标（常用于链接、按钮）              |
| text                    | 文本输入区域   | I形文本选择光标                           |
| move                    | 可拖拽元素     | 十字箭头（表示可移动）                    |
| wait                    | 加载等待状态   | 旋转圆圈/沙漏（表示系统繁忙）             |
| not-allowed             | 禁止操作       | 带斜杠的圆圈（表示当前操作不可用）        |
| crosshair               | 精准定位       | 十字线光标（用于绘图、测量工具）          |
| grab                    | 可抓取元素     | 手掌张开（表示可抓取，如拖拽视图）        |
| grabbing                | 抓取中状态     | 手掌闭合（表示正在抓取）                  |
| zoom-in / zoom-out      | 缩放操作       | 放大镜+“+”/“-”号（用于图片缩放控制）      |
| col-resize / row-resize | 调整列/行宽高  | 双向水平/垂直箭头（用于表格或分割线调整） |
| cell                    | 表格单元格选择 | 单元格选择框（类似Excel的光标）           |
| help                    | 帮助信息       | 箭头+问号（表示有额外说明）               |
| progress                | 后台处理中     | 箭头+旋转圆圈（表示进程运行但可交互）     |
| url()                   | 自定义光标     | 加载外部光标文件（需提供备用值）          |

---

 

- **pointer**：  
  浏览器中点击反馈的通用标识，建议与 `:hover` 状态配合使用：  

  ```css
  button:hover {
    cursor: pointer;
  }
  ```

- **grab系列**：  
  用于拖拽交互场景，需注意旧版浏览器可能显示为 `move`：  

  ```css
  .draggable {
    cursor: grab;
  }
  .draggable:active {
    cursor: grabbing;
  }
  ```

- **not-allowed**：  
  需同步禁用元素交互性以达到最佳效果：  

  ```css
  button:disabled {
    cursor: not-allowed;
    opacity: 0.6;
  }
  ```

- **自定义光标**：  
  支持 `.cur`、`.png` 等格式，需定义备用值：  

  ```css
  .magic-cursor {
    cursor: url('wand.cur'), url('wand.png'), auto;
  }
  ```

---

###### 注意事项  

1. **浏览器兼容性**：  

   - `grab`、`zoom-in` 等新特性需在CSS中提供备用值：  

     ```css
     .modern-cursor {
       cursor: grab;
       cursor: -webkit-grab; /* 旧版Webkit内核浏览器 */
     }
     ```

2. **无障碍设计**：  

   - 避免滥用特殊光标干扰用户认知  
   - 禁用状态需同时设置 `aria-disabled="true"`  

3. **性能优化**：  

   - 自定义光标文件建议小于32x32像素  
   - 避免对大面积元素使用复杂光标  

---

###### 应用场景示例  

1. 拖拽列表项：  

   ```css
   .list-item {
     cursor: move;
     transition: transform 0.2s;
   }
   .list-item:dragging {
     cursor: grabbing;
     opacity: 0.8;
   }
   ```

2. 图片缩放控制：  

   ```css
   .zoom-control {
     cursor: zoom-in;
   }
   .zoom-control.active {
     cursor: zoom-out;
   }
   ```

3. 自定义游戏光标：  

   ```css
   .game-canvas {
     cursor: url('sword.cur'), url('sword.png'), crosshair;
   }
   ```

---

###### 总结图示  

```
[光标类型映射]
┌───────────┬───────────────┐
│  default  │      →        │ 常规操作
│  pointer  │      →        │ 点击反馈
│  text     │      →        │ 文本输入
│  move     │      →        │ 拖拽移动
└───────────┴───────────────┘
```



###### **综合案例**

```Html
css鼠标手型cursor中hand与pointer
Example：CSS鼠标手型效果 <a href="#" style="cursor:hand">CSS鼠标手型效果</a><br/>
Example：CSS鼠标手型效果 <a href="#" style="cursor:pointer">CSS鼠标手型效果</a><br/>
注：pointer也是小手鼠标，建议大家用pointer，因为它可以兼容多种浏览器。<br/>
Example：CSS鼠标由系统自动给出效果 <a href="#" style="cursor:auto">CSS鼠标由系统自动给出效果</a><br/>
Example：CSS鼠标十字型 效果 <a href="#" style="cursor:crosshair">CSS鼠标十字型 效果</a><br/>
Example：CSS鼠标I字型效果 <a href="#" style="cursor:text">CSS鼠标I字形效果</a><br/>
Example：CSS鼠标等待效果 <a href="#" style="cursor:wait">CSS鼠标等待效果</a><br/>
Example：CSS鼠标默认效果 <a href="#" style="cursor:default">CSS鼠标默认效果</a><br/>
Example：CSS鼠标向右的箭头效果 <a href="#" style="cursor:e-resize">CSS鼠标向右的箭头效果</a><br/>
Example：CSS鼠标向右上箭头效果 <a href="#" style="cursor:ne-resize">CSS鼠标向右上箭头效果</a><br/>
Example：CSS鼠标向上箭头效果 <a href="#" style="cursor:n-resize">CSS鼠标向上箭头效果</a><br/>
Example：CSS鼠标向左上箭头效果 <a href="#" style="cursor:nw-resize">CSS鼠标向左上箭头效果</a><br/>
Example：CSS鼠标向左箭头效果 <a href="#" style="cursor:w-resize">CSS鼠标向左箭头效果</a><br/>
Example：CSS鼠标向左下箭头效果 <a href="#" style="cursor:sw-resize">CSS鼠标向左下箭头效果</a><br/>
Example：CSS鼠标向下箭头效果 <a href="#" style="cursor:s-resize">CSS鼠标向下箭头效果</a><br/>
Example：CSS鼠标向右下箭头效果 <a href="#" style="cursor:se-resize">CSS鼠标向下箭头效果</a><br/>
```



##### 删除项目符号

使用 `list-style:none` 删除项目符号

```html
<style></style>
.no-bullets {
    list-style: none; /* 移除所有列表项的项目符号 */
    padding-left: 0;  /* 可选：移除默认的内边距 */
}

/* 如果你需要对ol（有序列表）也进行相同的操作 */
.no-bullets ol {
    list-style: none;
}
</style>
<ul class="no-bullets">
    <li>项目 1</li>
    <li>项目 2</li>
    <li>项目 3</li>
</ul>
```





##### 线性渐变

- **基本语法**：

  ```css
  background: linear-gradient(direction, color-stop1, color-stop2, ...);
  ```

- **参数说明**：

  - **`direction`**：渐变的方向。可以是角度值（如 `45deg`）或关键字（如 `to top`, `to bottom`, `to left`, `to right`）。
  - **`color-stop`**：定义渐变中的颜色及其位置。格式为 `color position`，其中 `position` 是可选的，默认从 0% 开始。

- **常见用法**：

  - **从上到下**：

    ```css
    background: linear-gradient(to bottom, red, blue);
    ```

  - **从左到右**：

    ```css
    background: linear-gradient(to right, red, blue);
    ```

  - **带有颜色停止点**：

    ```css
    background: linear-gradient(to right, red 0%, yellow 50%, blue 100%);
    ```

  - **使用角度**：

    ```css
    background: linear-gradient(45deg, red, blue);
    ```



**repeating-linear-gradient() 函数用于重复线性渐变：**

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>重复渐变</title>
<style>
#grad1 {
  height: 200px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: repeating-linear-gradient(red, yellow 10%, green 20%);
    /* 这样在同一个大小的父元素重复的会更多 */
  background-image: repeating-linear-gradient(red, yellow 1%, green 5%);
}

#grad2 {
  height: 200px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: repeating-linear-gradient(45deg,red,yellow 7%,green 10%);
}

#grad3 {
  height: 200px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: repeating-linear-gradient(190deg,red,yellow 7%,green 10%);
}

#grad4 {
  height: 200px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: repeating-linear-gradient(90deg,red,yellow 7%,green 10%);
}
</style>
</head>
<body>

<h1>重复的线性渐变</h1>

<div id="grad1"></div>

<p>45deg:</p>
<div id="grad2"></div>

<p>190deg:</p>
<div id="grad3"></div>

<p>90deg:</p>
<div id="grad4"></div>

<p><strong>注意:</strong> Internet Explorer 9 及更早版本的 IE 浏览器不支持线性渐变。</p>

</body>
</html>
```

**通过修改每个首颜色和尾颜色的百分比而修改重复单位的基本大小**



##### 径向渐变

径向渐变由它的中心定义。

为了创建一个径向渐变，你也必须至少定义两种颜色结点。颜色结点即你想要呈现平稳过渡的颜色。同时，你也可以指定渐变的中心、形状（圆形或椭圆形）、大小。默认情况下，渐变的中心是 center（表示在中心点），渐变的形状是 ellipse（表示椭圆形），渐变的大小是 farthest-corner（表示到最远的角落）。

* 多个颜色之间的渐变，默认从圆心四散（不一定是正圆，要看容器本身宽高比）

```css
background-image: radial-gradient(red, yellow, green);
```

* 使用关键词调整渐变圆的圆心位置

```css
background-image: radial-gradient(at right top, red, yellow, green);
```

* 使用像素调整渐变圆的圆心位置

```css
background-image: radial-gradient(at 100px 50px, red, yellow, green);
```

* 调整渐变形状为正圆

```css
background-image: radial-gradient(circle, red, yellow, green);
```

* 调整形状的半径

```css
background-image: radial-gradient(100px, red, yellow, green);
background-image: radial-gradient(50px 100px, red, yellow, green);
```



**语法:**

background-image: radial-gradient(shape size at position, start-color, ..., last-color);

形状:ellipse（椭圆）/circle（圆形）

大小(半径)：属性值可用像素或关键字表示(圆形演示)

​        **closest-side**:圆心到距离最近的边

​        **farthest-side**:圆心到距离最远的边

​        **closest-corner**：圆心到距离最 近的角

​        **farthest-corner**：圆心到距离最远的角

发散方向：属性值可以为(at)left、right、top、bottom、center(可组合使用),像素百分比

起始颜色......

终止颜色......

**颜色结点均匀分布（默认情况下）**

颜色结点均匀分布的径向渐变：

```css
#grad { background-image: radial-gradient(red, yellow, green); }
```

**颜色结点不均匀分布**

颜色结点不均匀分布的径向渐变：

```css
#grad { background-image: radial-gradient(red 5%, yellow 15%, green 60%); }
```

**设置形状**

shape 参数定义了形状。它可以是值 circle 或 ellipse。其中，circle 表示圆形，ellipse 表示椭圆形。默认值是 ellipse。

形状为圆形的径向渐变：

```css
#grad { background-image: radial-gradient(circle at 100%, red, yellow, green); }
```



**不同尺寸大小关键字的使用**

size 参数定义了渐变的大小。它可以是以下四个值：

closest-side:圆心到距离最近的边

​    farthest-side:圆心到距离最远的边

​    closest-corner：圆心到距离最近的角

​    farthest-corner：圆心到距离最远的角

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>径向渐变尺寸</title>
<style>
#grad1 {
  height: 150px;
  width: 150px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: radial-gradient(closest-side at 60% 55%, red, yellow, black);
}

#grad2 {
  height: 150px;
  width: 150px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: radial-gradient(farthest-side at 60% 55%, red, yellow, black);
}

#grad3 {
  height: 150px;
  width: 150px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: radial-gradient(closest-corner at 60% 55%, red, yellow, black);
}

#grad4 {
  height: 150px;
  width: 150px;
  background-color: red; /* 浏览器不支持的时候显示 */
  background-image: radial-gradient(farthest-corner at 60% 55%, red, yellow, black);
}
</style>
</head>
<body>
<h3>径向渐变 - 不同尺寸大小关键字的使用</h3>
<p><strong>closest-side：</strong></p>
<div id="grad1"></div>
<p><strong>farthest-side：</strong></p>
<div id="grad2"></div>
<p><strong>closest-corner：</strong></p>
<div id="grad3"></div>

<p><strong>farthest-corner（默认）：</strong></p>
<div id="grad4"></div>

<p><strong>注意：</strong> Internet Explorer 9 及之前的版本不支持渐变。</p>

</body>
</html>
```



##### 重复径向渐变

**repeating-radial-gradient()** 函数用于重复径向渐变：

```css
#grad1 {height: 200px;background-image: repeating-radial-gradient(red, yellow 10%, green 15%);}
```



##### 字体霓虹灯

```html
<!DOCTYPE html>
<html lang="zh">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>霓虹灯文本效果</title>
    <style>
        body {
            background-color: #000; /* 背景颜色设置为黑色 */
            height: 100vh; /* 高度设置为视口高度的100% */
            margin: 0; /* 消除默认的外边距 */
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .neon-text {
            font-size: 72px; /* 字体大小设置为72像素 */
            background: linear-gradient(45deg, #ff00cc, #3333ff); /* 使用线性渐变背景 */
            background-clip: text; /* 将背景剪裁应用于文本 */
            color: transparent; /* 文本颜色设置为透明 */
            text-shadow: 0 0 10px rgba(255, 0, 204, 0.7), 0 0 20px rgba(255, 0, 204, 0.7), 0 0 30px rgba(255, 0, 204, 0.7); /* 添加多重阴影以模拟霓虹效果 */
        }
    </style>
</head>

<body>
    <!-- 应用霓虹灯文本效果 -->
    <span class="neon-text">你好，世界！</span>
</body>

</html>
```









### HTML 和 CSS之间的关系

父元素：**直接**包裹某个元素的元素，就是该元素的父元素

子元素：被父元素**直接**包含的元素

祖先元素：一直往上找，都是祖先，父元素也算祖先元素的一种，但一般都是父元素

后代元素：一直往下找，都是后代



#### 细说font-size

1. 由于字体设计原因，文字最终呈现的大小，并不一定与 `font-size` 的值一致，可能大，也可能小。例如：`font-size` 设为 `40px`，最终呈现的文字，可能比 `40px` 大，也可能比 `40px` 小。
2. 通常情况下，文字相对字体设计框，并不是垂直居中的，通常都靠下一些。





### 盒子模型

作用：布局网页，摆放盒子和内容，大概就是个容器

#### CSS中的常用的长度单位

1. `px`：像素。
2. `em`：相对元素 **`font-size`** 的倍数。
3. `rem`：相对**根字体**大小，html标签就是根。
4. `%`：相对父元素计算。
5. `vw`：**视口宽度**百分之多少  10vw就是视口宽度的10%     是可以随着视口大小的变化而变化的
6. `vh`：**视口高度**的百分之多少   10vh就是视口高度的10%    是可以随着视口大小的变化而变化的
7. `vmax`：视口宽高中大的那个百分之多少
8. `vmin`：视口宽高中小的那个百分之多少

**注意：**

CSS 中设置长度，必须加单位，否则样式无效！



#### 元素的显示模式

##### 块元素（block）

- **又称**：块级元素

- 特点

  1. 在页面中独占一行，不会与任何元素共用一行，是从上到下排列的。
  2. 默认宽度：撑满父元素。
  3. 默认高度：由内容撑开。
  4. 可以通过 CSS 设置宽高。

##### 行内元素（inline）

- **又称**：内联元素

- 特点

  1. 在页面中不独占一行，一行中不能容纳下的行内元素，会在下一行继续从左到右排列。
  2. 默认宽度：由内容撑开。
  3. 默认高度：由内容撑开。
  4. 无法通过 CSS 设置宽高。

##### 行内块元素（inline-block）

- **又称**：内联块元素

- 特点

  1. 在页面中不独占一行，一行中不能容纳下的行内元素，会在下一行继续从左到右排列。
  2. 默认宽度：由内容撑开。
  3. 默认高度：由内容撑开。
  4. 可以通过 CSS 设置宽高。

**注意：**

元素早期只分为：行内元素、块级元素，区分条件也只有一条：“是否独占一行”，如果按照这种分类方式，行内块元素应该算作行内元素。

**区分：**

**对比总结表**：

| 特性         | 块级元素         | 行内元素         | 行内块元素                                  |
| ------------ | ---------------- | ---------------- | ------------------------------------------- |
| 是否独占一行 | ✅ 是             | ❌ 否             | ❌ 否                                        |
| 排列方向     | 垂直（从上到下） | 水平（从左到右） | 水平（从左到右）                            |
| 可设置宽度   | ✅                | ❌                | ✅                                           |
| 可设置高度   | ✅                | ❌                | ✅                                           |
| 默认宽度     | 撑满父容器       | 由内容决定       | 由内容决定                                  |
| 默认高度     | 由内容决定       | 由内容决定       | 由内容决定                                  |
| 典型代表     | `<div>`, `<p>`   | `<span>`, `<a>`  | `<img>`, `<input>`, `display: inline-block` |

------

**实际应用建议**：

- 使用 **块级元素** 构建页面的主要结构（如布局容器、段落、标题等）。
- 使用 **行内元素** 包裹文本中的部分内容（如加粗、链接等）。
- 使用**行内块元素**实现水平排列的可控制尺寸的元素，比如：
  - 导航菜单项
  - 图标按钮
  - 图文混排布局

> 💡 提示：可以通过 `display` 属性在三种模式之间转换，例如：
>
> ```
> display: block;
> display: inline;
> display: inline-block;
> ```

掌握这三种显示模式的区别，是理解和实现CSS布局的基础。



#### 组成

盒子模型的重要组成部分：

- 内容区域 -content  width & height
- 内边距 - padding （出现在内容与盒子边缘之间）
- 边框线 - border（盒子的边框）
- 外边距 - margin (出现在盒子外面，盒子与外界的距离）

> 本质上这些都是属性，在对应选择器中书写即可
>
> 盒子的大小 = content + 左右 padding + 左右 border
>
> 外边距margin不会影响盒子的大小，但会影响盒子的位置



##### content内容区

**CSS 尺寸设置属性表**

| CSS属性名  | 功能                   | 属性值 |
| :--------- | :--------------------- | :----- |
| width      | 设置内容区域宽度       | 长度   |
| max-width  | 设置内容区域的最大宽度 | 长度   |
| min-width  | 设置内容区域的最小宽度 | 长度   |
| height     | 设置内容区域的高度     | 长度   |
| max-height | 设置内容区域的最大高度 | 长度   |
| min-height | 设置内容区域的最小高度 | 长度   |

**注意：**

- `max-width`、`min-width`一般不与 `width`一起使用。
- `max-height`、`min-height`一般不与 `height`一起使用。



###### 关于默认宽度

**所谓的默认宽度**，就是不设置width属性时，元素所呈现出来的宽度。

**总宽度** = 父的content - 自身的左右margin。

**内容区的宽度** = 父的content - 自身的左右margin - 自身的左右border - 自身的左右padding。



 

##### Padding内边距

作用：设置 内容 与 盒子边缘 之间的距离

设置的背景颜色会填充内边距 

属性名： padding / padding-方向名词

以下是代码示例：

```css
div{
    /*四个方向内边距相同*/
    padding: 30px;
    
    /*单独设置一个方向内边距*/
    padding-top: 10px;
    padding-bottom: 20px;
    padding-right: 30px;
    padding-left: 40px;
    
    width: 200px;
    height: 200px;
    background-color: pink;
    
}
```



> Padding内边距属性 会撑大盒子，比如设置 padding: 20px; 盒子会向外扩展20px出来

应用：在文本框中，可以用于文字与前边框的距离

![image-20250906175133715](./笔记/笔记/web-img/image-20250906175133715.png)

```css
    padding-left: 16px;
```



###### 多值写法

取值写法：

| 取值个数 | 示例                         | 含义                   |
| -------- | ---------------------------- | ---------------------- |
| 一个值   | padding: 10px                | 四个方向内边距均为10px |
| 四个值   | padding: 10px 20px 40px 80px | 上右下左               |
| 三个值   | padding: 10px 40px 80px      | 上 左右 下             |
| 两个值   | padding: 10px 80px           | 上下 左右              |





##### Border边框线

###### 全方向

作用：全方向添加一个边框线

设置的背景颜色会填充边框线

属性名：border（bd）

属性值：边框线粗细 线条样式 颜色（不区分顺序）

常用的线条样式

| 属性值 | 线条样式 |
| ------ | -------- |
| solid  | 实线     |
| dashed | 虚线     |
| dotted | 点线     |

> 此处只说明常用的三个属性值，并非只有这三个

 

```css
div{
    border: 1px solid black;
    /*三个参数分别为 边框线粗细 线条样式 颜色*/
}
```

 这段CSS代码将为盒子添加一个1px宽度 黑色 实线的盒子边框线

同时还可以单独设置单方向的边框线



去除选中边框可以使用 `outline:none;`



###### 单方向

属性名：border-方向名词（bd+方向名词首字母，例如，bdl）

属性值：边框线粗细 线条样式 颜色（不区分顺序）

方向名词表

| 属性名 | 方向 |
| ------ | ---- |
| top    | 顶部 |
| bottom | 底部 |
| right  | 右侧 |
| left   | 左侧 |



##### Margin外边距

作用：拉开两个盒子之间的距离

属性名：margin

提示：与 padding 属性值写法、含义相同

复合模式请参考padding

| CSS属性名     | 功能                                           | 属性值        |
| :------------ | :--------------------------------------------- | :------------ |
| margin-left   | 左外边距                                       | CSS中的长度值 |
| margin-right  | 右外边距                                       | CSS中的长度值 |
| margin-top    | 上外边距                                       | CSS中的长度值 |
| margin-bottom | 下外边距                                       | CSS中的长度值 |
| margin        | 复合属性，可以写1~4个值，规律同padding(顺时针) | CSS中的长度值 |



**注意：**

* 子元素的margin是参考父元素的content计算的
* 上margin、左margin会影响自身的位置，下margin、右margin会影响兄弟元素的位置
* 对于行内元素来说，左右的margin 是可以完美设置的，上下margin设置后是无效的
* 对于块级元素来说，margin的值也可以是auto，可以实现该元素在其父元素内水平居中
* margin的值可以是负值



> Margin外边距属性 会在盒子外面扩展一片空白，不会改变盒子的大小，但是位置变了
>
> PS：简单的来说，内边距相当于快递包裹里的填充物，外边距相当于箱子外面的快递包裹袋子



###### 版心居中(重要)

如果想要盒子页面居中，即使在不同尺寸与分辨率的页面也能居中，就添加 `Margin外边距属性` 并将值设置为 `auto`

```css
margin:0 auto
```





**注意！！注意！！**

**使用此方法需要盒子设置宽度，否则会跟随父级宽度，但是在某种意义上，也算是版心居中了**



###### margin的塌陷问题

**什么是 margin 塌陷？**

当两个垂直方向（上下）的盒子（比如兄弟元素或父子元素）的 margin 相遇时，它们不会叠加，而是会**“合并”成一个 margin**，取两者中较大的那个值。这种现象就叫 margin 塌陷。

###### **如何解决 margin 塌陷？**

1. **加隔离层**：比如给父元素加 `padding`或 `border`（例如 `border: 1px solid transparent`）。
2. **触发 BFC**：给父元素设置 `overflow: hidden`或 `display: flow-root`。
3. **用 Flex/Grid 布局**：这些布局方式不会塌陷。



###### margin合并问题

**什么是 margin 合并？**

上面兄弟元素的下外边距和下面兄弟元素的上外边距会合并，取一个最大的值，而不是相加。

**如何解决 margin 合并（塌陷）？**

无需解决，布局的时候上下的兄弟元素，只给一个设置上下外边距就可以了。



###### 区别

`margin` 的**塌陷问题**（Margin Collapse）和**合并问题**其实指的是同一个现象，即 **“外边距合并”**（Margin Collapse），中文里有时会因翻译或理解不同而出现“塌陷”或“合并”的说法。但在标准的 CSS 术语中，正确的说法是 **“外边距合并”**（Margin Collapse）。

不过，为了澄清你的疑问，我们可以从两个角度来理解这个现象的不同表现形式：

------

✅ 正确认知：**“塌陷”和“合并”是同一现象的不同描述**

- **“合并”**：强调两个 margin **叠加在一起**，但不是相加，而是取**最大值**。
- **“塌陷”**：多用于描述父子元素之间 margin 表现“塌陷”到父元素外部，给人一种“塌下去”的视觉错觉。

所以，**它们不是两种不同的问题，而是同一问题在不同场景下的表现**。

------

📌 外边距合并（Margin Collapse）发生的三种典型场景

1. **相邻兄弟元素之间的 margin 合并**

两个**垂直排列的兄弟元素**，上下 margin 会合并。

```css
<div class="box1">Box 1</div>
<div class="box2">Box 2</div>
```

```css
.box1 { margin-bottom: 20px; }
.box2 { margin-top: 30px; }
```

👉 实际间距不是 `20 + 30 = 50px`，而是取最大值：**30px**。

------

2. **父子元素之间的 margin 塌陷（常被称作“塌陷”）**

当**子元素的 margin-top** 与**父元素的内容区域**接触时，margin 会“向上溢出”，导致父元素整体向下移动，看起来像是父元素的 margin 塌陷了。

```css
<div class="parent">
  <div class="child">Child</div>
</div>
```

```css
.parent {
  width: 200px;
  height: 200px;
  background: lightblue;
  /* 没有 padding 或 border */
}
.child {
  margin-top: 30px;
  height: 50px;
  background: coral;
}
```

👉 你期望子元素距离父元素顶部 30px，但结果是**整个父元素被往下推了 30px**。这就是所谓的“margin 塌陷”。

✅ **解决方法**：

- 给父元素添加 `padding-top: 1px;`
- 给父元素添加 `border: 1px solid transparent;`
- 使用 `overflow: hidden;`（推荐）
- 使用 `display: flex;` 或 `display: grid;`（Flexbox/Grid 不会发生 margin collapse）

------

3. **空元素自身的上下 margin 合并**

一个没有内容、没有 padding、没有 border 的块级元素，其自身的 `margin-top` 和 `margin-bottom` 会合并成一个 margin。

```css
.empty {
  margin-top: 20px;
  margin-bottom: 30px;
  /* height: 0; 且无内容 */
}
```

👉 最终 margin 高度为 30px（取最大值）。

------

✅ **总结**：区别？其实没有本质区别！

| 说法            | 含义说明                                                 |
| --------------- | -------------------------------------------------------- |
| **margin 合并** | 标准术语，指垂直方向相邻 margin 合并为一个，取最大值     |
| **margin 塌陷** | 特指**父子元素间**的 margin 合并现象，视觉上像“塌下去”了 |

👉 所以：

- **“合并”是通用术语**（适用于兄弟、空元素、父子）
- **“塌陷”是特例描述**（多用于父子关系）

------

✅ 如何避免 margin 合并/塌陷？

1. 使用 `padding` 或 `border` 隔开父子元素
2. 父元素设置 `overflow: hidden`
3. 使用 Flexbox / Grid 布局（默认不合并）
4. 使用 `display: inline-block`
5. 使用 CSS 逻辑间距（如 `gap`）



#### 尺寸计算

相邻元素外边距相同时会碾压，不同时采用大值

- 默认情况

盒子尺寸 = 内容尺寸 + border尺寸 + 内边距尺寸

现在有一案例，要求设计的盒子是200*200，因为border和padding会撑大，目前解决方法有两种

解决方法

- 手动减法：减掉 border 与 padding 的尺寸，自己算
- 内减模式：box-sizing: border-box 直接卸载属性中，浏览器自己会减去

#### box-sizing

`box-sizing: border-box`； `width`和`height`包含`border`和`padding`的值，不会再额外增加

就是说，所写的`width`和`height`是盒子的总宽高

让你设定的 `width` 和 `height` 成为元素在页面上**实际占据的空间大小**，内边距和边框会“吃掉”内容区域的空间，而不是增加总尺寸。

使用 `box-sizing` 属性可以设置盒模型的两种类型。

| 可选值      | 含义                                                         |
| ----------- | ------------------------------------------------------------ |
| content-box | `width` 和 `height` 设置的是盒子内容区的大小。（默认值）     |
| border-box  | `width` 和 `height` 设置的是盒子总大小。（怪异盒模型） 内容区+padding+border |



#### resize（了解）

要和 overflow 配合使用

使用 `resize` 属性可以控制是否允许用户**调节元素尺寸**。

| 值         | 含义                               |
| ---------- | ---------------------------------- |
| none       | 不允许用户调整元素大小。（默认值） |
| both       | 用户可以调节元素的宽度和高度。     |
| horizontal | 用户可以调节元素的宽度。           |
| vertical   | 用户可以调节元素的高度。           |





#### 元素溢出

谁是容器，就在谁身上加属性

作用：控制溢出元素的内容的显示方式

属性名：overflow

属性值

| 属性值    | 说明                             |
| :-------- | :------------------------------- |
| `visible` | 显示，默认值                     |
| `hidden`  | 隐藏                             |
| `scroll`  | 显示滚动条，不论内容是否溢出     |
| `auto`    | 自动显示滚动条，内容不溢出不显示 |

**注意**：

1. `overflow-x`、`overflow-y`不能一个是 `hidden`，一个是 `visible`，是实验性属性，不建议使用。

​    2.`overflow`常用的值是 `hidden`和 `auto`，除了能处理溢出的显示方式，还可以解决很多疑难杂症。

tag: 超出 裁切 隐藏 溢出



#### 隐藏元素的两种方式

可以少写点代码

###### **方式一：visibility 属性**

`visibility`属性默认值是 `show`（应为 `visible`），如果设置为 `hidden`，元素会隐藏。

元素看不见了，还占有原来的位置（元素的大小依然保持）。

###### **方式二：display 属性**

设置 `display: none`，就可以让元素隐藏。

彻底地隐藏，不但看不见，也不占用任何位置，没有大小宽高。



#### 样式的继承

**核心概念：**

有些样式会继承。元素如果本身设置了某个样式，就使用本身设置的样式；但如果本身没有设置某个样式，会从父元素开始一级一级继承（优先继承离得近的祖先元素）。

**方式一：visibility 属性**

`visibility`属性默认值是 `show`（应为 `visible`），如果设置为 `hidden`，元素会隐藏。

元素看不见了，还占有原来的位置（元素的大小依然保持）。

**方式二：display 属性**

设置 `display: none`，就可以让元素隐藏。

彻底地隐藏，不但看不见，也不占用任何位置，没有大小宽高。

##### **会继承的 CSS 属性**

- 字体属性 (如 `font-family`, `font-size`)
- 文本属性 (除了 `vertical-align`)
- 文字颜色 (如 `color`)

------

##### **不会继承的 CSS 属性**

- 边框 (如 `border`)
- 背景 (如 `background`)
- 内边距 (如 `padding`)
- 外边距 (如 `margin`)
- 宽高 (如 `width`, `height`)
- 溢出方式 (如 `overflow`)

##### **核心规律**

一个规律：能继承的属性，都是不影响布局的，简单说：都是和盒子模型没关系的。



#### 元素的默认样式

**元素一般都有些默认的样式，例如：**

1. **`<a>`元素：**
   - 下划线
   - 字体颜色
   - 鼠标小手（光标样式）
2. **`<h1>`～ `<h6>`元素：**
   - 文字加粗
   - 文字大小
   - 上下外边距
3. **`<p>`元素：**
   - 上下外边距
4. **`<ul>`、`<ol>`元素：**
   - 左内边距
5. **`body`元素：**
   - 8px外边距（4个方向）

------

**优先级说明：**

**元素的默认样式 > 继承的样式**

因此，如果要重置元素的默认样式，选择器**一定要直接选择到该元素**。



#### 清除默认样式

作用：清楚标签默认的样式，比如：默认的内边距

常用的方法是 通配符选择器

```css
*{
    margin: 0;
    pading: 0;
    box-sizing: border-box;
}
```



#### 布局的小技巧

**1. 行内元素、行内块元素的对齐特性**

行内元素、行内块元素，可以被父元素当做文本处理。

即：可以像处理文本对齐一样，去处理行内、行内块元素在父元素中的对齐。

例如：使用 `text-align`、`line-height`、`text-indent`等属性。

------

**2. 如何让子元素在父元素中水平居中**

- **若子元素为块元素：** 给**子元素**加上 `margin: 0 auto;`。
- **若子元素为行内元素、行内块元素：** 给**父元素**加上 `text-align: center;`。

------

**3. 如何让子元素在父元素中垂直居中**

- **若子元素为块元素：** 给**子元素**加上 `margin-top`，其值为：`(父元素content高度 - 子元素盒子总高度) / 2`。
- **若子元素为行内元素、行内块元素：**
  1. 让**父元素**的 `height`值等于 `line-height`值。
  2. 给**每个子元素**都加上 `vertical-align: middle;`。
     - **补充：** 若想实现绝对垂直居中，可以将父元素的 `font-size`设置为 `0`。



#### 元素之间的空白问题

原因：行内元素、行内块元素，彼此之间的换行会被浏览器解析为一个空白字符

解决方法：

1. 别换行（不咋地）
2. 给父元素设置 font-size：0；，在给需要显示文字的元素，单独设置字体大小（推荐）



#### 行内块之间的幽灵空白问题

![image-20250905141743070](./笔记/笔记/web-img/image-20250905141743070.png)

**行内块元素与文本对齐问题**

**1. 产生原因**

行内块元素与文本的基线对齐，而文本的基线与文本最底端之间是有一定距离的。

**2. 解决方案**

- **方案一：** 给行内块元素设置 `vertical-align`属性，值不为 `baseline`即可（例如设置为 `middle`、`bottom`、`top`均可）。
- **方案二：** 若父元素中只有一张图片，设置图片为 `display: block`。
- **方案三：** 给父元素设置 `font-size: 0`。如果该行内块内部还有文本，则需单独为文本设置 `font-size`。



#### :heavy_exclamation_mark: 圆角与阴影

##### 圆角

###### 基础用法

作用：设置元素的外边框为圆角

属性名：border-radius

属性值：数字+px / 百分比

多值写法：左上角 右上角 右下角 左下角

提示：属性值是圆角半径，数字越大越圆，越小越尖

> 单独写是四个角相同的圆角大小，可以通过给属性添加多个值以达到控制每个角弧度的效果
>
> 关于记忆的顺序的方法：从左上角顺时针赋值，没有取值的角与对角取值相同

在 CSS3 中，使用 `border-radius` 属性可以将盒子变为圆角。

- **同时设置四个角的圆角：**

  ```css
  border-radius: 10px;
  ```

- **分开设置每个角的圆角（几乎不用）：**

| 属性名                       | 作用                                                         |
| ---------------------------- | ------------------------------------------------------------ |
| `border-top-left-radius`     | 设置左上角圆角半径：<br>1. 一个值是正圆半径。<br>2. 两个值分别是椭圆的 x 半径、y 半径。 |
| `border-top-right-radius`    | 设置右上角圆角半径：<br>1. 一个值是正圆半径。<br>2. 两个值分别是椭圆的 x 半径、y 半径。 |
| `border-bottom-right-radius` | 设置右下角圆角半径：<br>1. 一个值是正圆半径。<br>2. 两个值分别是椭圆的 x 半径、y 半径。 |
| `border-bottom-left-radius`  | 设置左下角圆角半径：<br>1. 一个值是正圆半径。<br>2. 两个值分别是椭圆的 x 半径、y 半径。 |

- 分开设置每个角的圆角，综合写法（几乎不用）：

  ```css
  border-radius: 左上角x 右上角x 右下角x 左下角x / 左上角y 右上角y 右下角y 左下角y
  ```

- **一个值**：所有四个角都应用相同的圆角半径。

- **两个值**：第一个值应用于左上角和右下角，第二个值应用于右上角和左下角。

- **三个值**：第一个值应用于左上角，第二个值应用于右上角和左下角，第三个值应用于右下角。

- **四个值**：顺时针方向从左上角开始，依次是左上、右上、右下、左下。

###### 常见应用

正圆形状

前提是盒子本身就是正方形的，给盒子设置圆角属性值为 宽高的一半 / 50%

写法：有两种，一种是算出来设置，一种是直接设置为50%

```css
img{
    width: 200px;
    height: 200px;
    
    /*在本案例中，他俩的最终效果是一样的，百分比比的是盒子宽高*/
    border-radius: 100px;
    border-radius: 50%;
}
```

> 效果大概就是圆形头像的样子，在一个盒子中，最大值为50%，再大就没效果了





胶囊形状

前提是盒子本身是长方形，给盒子设置圆角属性值为 盒子高度的一半

写法：`Talk is cheap Show me the code`

```css
div{
    width: 200px;
    height: 80px;
    background-color: orange;
    
    border-radius: 40px;
}
```





##### 阴影效果

在 CSS 中，主要有两种阴影：

1. **盒子阴影（box-shadow）** → 给盒子元素加阴影（最常用）
2. **文字阴影（text-shadow）** → 给文字加阴影

作用：给元素设置阴影效果

###### 盒子阴影效果

属性名：box-shadow

属性值： X轴偏移量 Y轴偏移量 模糊半径 扩散半径 颜色 内外阴影

```css
 box-shadow: 5px 5px 12px #ffffff ,
                -5px -5px 12px #c8d0e7;

```

使用 `box-shadow` 属性为盒子添加阴影。

**内阴影**（阴影在元素内部）

加 `inset` 关键字：

```css
input {
    box-shadow: inset 0 2px 5px rgba(0,0,0,0.2);
}
```

✅ 常用于输入框、凹陷按钮等。

**多重阴影**（叠加多个阴影）

用逗号分隔多个阴影：

```css
.button {
    box-shadow: 
        0 2px 5px rgba(0,0,0,0.2),
        0 4px 10px rgba(0,0,0,0.1);
}
```

👉 层层叠加，更真实立体。



各个值的含义：

| 值       | 含义                                 |
| -------- | ------------------------------------ |
| h-shadow | 水平阴影的位置，必须填写，可以为负值 |
| v-shadow | 垂直阴影的位置，必须填写，可以为负值 |
| blur     | 可选，模糊距离                       |
| spread   | 可选，阴影的外延值                   |
| color    | 可选，阴影的颜色                     |
| inset    | 可选，将外部阴影改为内部阴影         |

默认值：

- `box-shadow: none` 表示没有阴影



注意：

- X轴偏移量 和 Y轴偏移量 是必须指
- 默认是外阴影，内阴影需要添加 inset 属性 直接在后面加上就行了

> 其实吧，他是个复合属性，义眼顶针了，对吧。



###### 文字阴影效果

**基础文字阴影**

```css
h1 {
    text-shadow: 2px 2px 5px rgba(0,0,0,0.5);
}
```

👉 文字有立体感，适合深色背景上的标题。

**发光文字效果**

```css
.glow {
    text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px #00f;
}
```

✅ 常用于科技感、霓虹灯风格

文字阴影不支持内阴影



#### 边框外轮廓

outline

- `outline-width`：外轮廓的宽度。

- `outline-color`：外轮廓的颜色。

- `outline-style`：外轮廓的风格。

  - `none`：无轮廓
  - `dotted`：点状轮廓
  - `dashed`：虚线轮廓
  - `solid`：实线轮廓
  - `double`：双线轮廓

- `outline-offset` 设置**外轮廓与边框的距离**，正负值都可以设置。

   

  **注意**：`outline-offset` 不是 `outline` 的子属性，是一个独立的属性。

- `outline` 复合属性

  ```css
  outline: 50px solid blue;
  ```



#### 盒子模型问题合集



##### 外边距合并现象

场景：垂直排列的兄弟元素，上下 margin 会合并

现象：取两个 margin 中的 **较大值** 生效

> 大概就是大的margin覆盖了小的，看不到了而已



##### 外边距塌陷问题

场景：父子级的标签，当父级没有内容时，子级的添加 **上外边距** 会产生塌陷问题

现象：导致父级一起向下移动

> 大概就是父级没有内容，子级的内容继承上去了，两个盒子合成一个盒子，使用外边距会导致两个盒子一起移动，看起来就像是给大盒子设置了上外边距

解决方法：

- 取消子级margin，父级设置padding，同时设置box-sizing: border-box 就能保证整个父级标签大小不变
- 父级设置 overflow: hidden
- 父级设置 border-top
- 给父级随便写点内容



##### 内外边距问题

场景：行内元素添加 margin 和 padding，无法改变元素垂直位置

解决方法：给行内元素添加 line-height(行高) 可以改变垂直位置

> 

```css
span{
    /*无法改变垂直位置*/
    margin: 50px;
    padding: 20px;
    
    /*无法改变垂直位置*/
    line-height: 100px;
}
```



### 浮动  

在最初，浮动是用来实现文字环绕图片效果的，现在浮动是主流的页面布局方式之一

作用：让块元素水平排列

属性值：float

属性值：

- left：左对齐，将出现在父级的最左边
- right：右对齐，将出现在父级的最右边

特点：顶对齐，具备行内块显示模式的特点，浮动后脱离标准流的控制，有可能出现重合



#### 浮动的特点

1. **脱离标准文档流**。（不好）
2. 无论浮动前是什么元素，浮动后都具有以下特性：
   - 默认的宽度和高度均由内容撑开（尽可能小）。
   - 可以显式地设置宽度(`width`)和高度(`height`)。
3. **不会独占一行**，可以与其他元素共用一行。
4. **不会发生 margin 合并，也不会发生 margin 塌陷**，能够完美地设置四个方向的 `margin`和 `padding`。
5. **不会像行内块元素一样被当做文本处理**（因此没有行内块元素的空白间隙问题）。



#### 浮动后会有哪些影响

对兄弟元素的影响：对后面的兄弟元素，会占据浮动元素之前的位置，在浮动元素下面，对前面的兄弟无影响

对父元素的影响：不能撑起父元素的高度，导致父元素高度塌陷，但父元素的宽度依然束缚浮动的元素



#### 清除浮动

场景：浮动元素会脱标，如果父级没有高度，子级无法撑开父级高度（可能导致布局错乱）

结局方法：清除浮动（清除浮动带来的影响）

方法一：

- 在父级元素内容的最后添加一个块级元素，设置 CSS 属性  `clear:both`

> 通常都将清除浮动的 CSS 的类名设置为 `clearfix` 

方法二：单伪元素法

```css
.clearfix::after{
    content:"";
    display: block;
    clear: both;
}
```

| 属性  | 说明                                                         |
| ----- | ------------------------------------------------------------ |
| clear | 指定不允许元素周围有浮动元素。left：在左侧不允许浮动元素。right：在右侧不允许浮动元素。both： 在左右两侧均不允许浮动元素。None  默认值。允许浮动元素出现在两侧。 |

“float是魔鬼，会影响其他相邻元素；但是clear是小白，其只会影响自身，不会对其他相邻元素造成影响！”

元素盒子的边不能和前面的浮动元素相邻，那么就是自己下移。



浮动的本质作用还是实现图文混排的效果





### 定位



父相子绝



#### 定位属性

position 属性用于指定一个元素在文档中的定位方式。

position 属性的五个值：

|    值    |   效果   |
| :------: | :------: |
|  static  | 静态定位 |
| relative | 相对定位 |
|  fixed   | 固定定位 |
| absolute | 绝对定位 |
|  sticky  | 粘性定位 |



#### 相对定位

 **1.如何设置相对定位？**

- 给元素设置 `position: relative;`即可实现相对定位。
- 可以使用 `left`、`right`、`top`、`bottom`四个属性调整位置。

**2. 相对定位的参考点在哪里？**

- 相对自己原来的位置。

**3。 相对定位的特点：**

1. **不会脱离文档流**，元素位置的变化只是视觉效果上的变化，**不会对其他元素产生任何影响**。

2. 定位元素的显示层级比普通元素高，无论什么定位，显示层级都是一样的。

   **默认规则是：**

   - 定位的元素会盖在普通元素之上。
   - 都发生定位的两个元素，后写的元素会盖在先写的元素之上。

3. `left`和 `right`不能一起设置，`top`和 `bottom`不能一起设置。

4. 相对定位的元素也能继续浮动，但**不推荐**这样做。

5. 相对定位的元素也能通过 `margin`调整位置，但**不推荐**这样做。

**注意：**

绝大多数情况下，相对定位会与绝对定位配合使用。



- **保留文档流**：元素仍占据原始空间，周围元素布局不受影响。

- **定位基准**：相对于**自身原始位置**进行偏移。

- **定位方式**：通过 `top`, `right` 等属性微调位置（如 `left: 20px` 向右移动20像素）。

- **应用场景**：微调元素位置、作为绝对定位子元素的定位基准，子级绝对定位，父级相对定位（子绝对父相对）

- **示例**：

  ```css
  .box {
    position: relative;
    top: 10px; /* 从原位置向下移动10px */
    left: 20px; /* 从原位置向右移动20px */
  }
  ```







#### 绝对定位

**1 如何设置绝对定位？**

- 给元素设置 `position: absolute;`即可实现绝对定位。
- 可以使用 `left`、`right`、`top`、`bottom`四个属性调整位置。

------

**2 绝对定位的参考点在哪里？**

- 参考它的**包含块**。

**什么是包含块？**

1. 1.

   对于**没有脱离文档流**的元素：包含块就是父元素。

2. 2.

   对于**脱离文档流**的元素：包含块是第一个拥有**定位属性**（`position`值非 `static`）的祖先元素（如果所有祖先都没定位，那包含块就是整个页面）。

------

**3 绝对定位元素的特点**

1. 1.

   **脱离文档流**，会对后面的兄弟元素、父元素有影响。

2. 2.

   `left`和 `right`不能一起设置，`top`和 `bottom`不能一起设置。

3. 3.

   绝对定位、浮动不能同时设置，如果同时设置，**浮动失效**，以定位为主。

4. 4.

   绝对定位的元素，也能通过 `margin`调整位置，但**不推荐**这样做。

5. 5.

   无论是什么元素（行内、行内块、块级）设置为绝对定位之后，都变成了**定位元素**。

**何为定位元素？**

- 默认宽、高都被内容所撑开，且能自由设置宽高。

 



**元素可以使用的顶部，底部，左侧和右侧属性定位。**然而，这些属性无法工作，除非是先设定position属性(static除外)。他们也有不同的工作方式，这取决于定位方法。

| 属性     | 说明                                                         |
| -------- | ------------------------------------------------------------ |
| position | 指定元素的定位类型。<br><br/>static HTML 元素的默认值，即没有定位，遵循正常的文档流对象。静态定位的元素不会受到 top, bottom, left, right影响。<br><br/>absolute  绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于```<html>```。absolute 定位使元素的位置与文档流无关，因此不占据空间。absolute 定位的元素和其他元素重叠。<br><br/>fixed  元素的位置相对于浏览器窗口是固定位置。即使窗口是滚动的它也不会移动：Fixed定位使元素的位置与文档流无关，因此不占据空间。Fixed定位的元素和其他元素重叠。     <br><br/>relative  相对定位元素的定位是相对其正常位置。移动相对定位元素，但它原本所占的空间不会改变。<br><br/>sticky  sticky 英文字面意思是粘，粘贴，所以可以把它称之为粘性定位。**position: sticky;** 基于用户的滚动位置来定位。粘性定位的元素是依赖于用户的滚动，在 position:relative 与 position:fixed 定位之间切换。它的行为就像 <br/><br/>position:relative; 而当页面滚动超出目标区域时，它的表现就像 position:fixed;，它会固定在目标位置。元素定位表现为在跨越特定阈值前为相对定位，之后为固定定位。这个特定阈值指的是 top, right, bottom 或 left 之一，换言之，指定 top, right, bottom 或 left 四个阈值其中之一，才可使粘性定位生效。否则其行为与相对定位相同。 |
| right    | 定义了定位元素右外边距边界与其包含块右边界之间的偏移。       |
| top      | 定义了一个定位元素的上外边距边界与其包含块上边界之间的偏移。 |
| bottom   | 定义了定位元素下外边距边界与其包含块下边界之间的偏移。       |
| left     | 定义了定位元素左外边距边界与其包含块左边界之间的偏移。       |





**案例：**

```html
    <style>
        /* 通用样式 */
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
        }

        .box {
            width: 100px;
            height: 100px;
            margin: 10px;
            color: white;
        }

        /* static 定位 */
        .static {
            position: static;
            background-color: #3498db;
        }

        /* relative 定位 */
        .relative {
            position: relative;
            left: 50px;
            top: 20px;
            background-color: #2ecc71;
        }

        /* absolute 定位 */
        .parent {
            position: relative;
            width: 300px;
            height: 200px;
            border: 1px solid #ccc;
            margin: 20px;
        }

        .absolute {
            position: absolute;
            right: 20px;
            bottom: 20px;
            background-color: #e74c3c;
        }

        /* fixed 定位 */
        .fixed {
            position: fixed;
            top: 20px;
            right: 20px;
            background-color: #f39c12;
        }

    </style>
</head>

<body>
    <!-- static 定位示例 -->
    <h2>static 定位</h2>
    <p>元素默认的定位方式，按照正常的文档流进行布局。</p>
    <div class="box static">Static</div>

    <!-- relative 定位示例 -->
    <h2>relative 定位</h2>
    <p>元素相对于其正常位置进行偏移，仍占据原文档流中的空间。</p>
    <div class="box relative">Relative</div>

    <!-- absolute 定位示例 -->
    <h2>absolute 定位</h2>
    <p>元素相对于最近的已定位祖先元素进行定位，如果没有已定位的祖先元素，则相对于文档的初始包含块。</p>
    <div class="parent">
        <div class="box absolute">Absolute</div>
    </div>

    <!-- fixed 定位示例 -->
    <h2>fixed 定位</h2>
    <p>元素相对于浏览器窗口进行定位，滚动页面时元素位置不变。</p>
    <div class="box fixed">Fixed</div>


    <!-- 用于产生滚动效果 -->
    <div style="height: 1000px;"></div>
</body>
```

**粘性定位实例:**

```html
<style>
div.sticky {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    padding: 5px;
    background-color: #cae8ca;
    border: 2px solid #4CAF50;
}
</style>
</head>

<body>
    <p>尝试滚动页面。</p>
    <p>注意: IE/Edge 15 及更早 IE 版本不支持 sticky 属性。</p>

    <div class="sticky">我是粘性定位!</div>

    <div style="padding-bottom:2000px">
        <p>滚动我</p>
        <p>来回滚动我</p>
        <p>滚动我</p>
        <p>来回滚动我</p>
        <p>滚动我</p>
        <p>来回滚动我</p>
    </div>

</body>
```



------





#### **固定定位**

**3.1 如何设置为固定定位？**

- 给元素设置 `position: fixed;`即可实现固定定位。
- 可以使用 `left`、`right`、`top`、`bottom`四个属性调整位置。

------

**3.2 固定定位的参考点在哪里？**

- 参考它的**视口**。

**什么是视口？**

- 对于PC浏览器来说，视口就是我们看网页的那扇“窗户”。

------

**3.3 固定定位元素的特点**

1. **脱离文档流**，会对后面的兄弟元素、父元素有影响。
2. `left`和 `right`不能一起设置，`top`和 `bottom`不能一起设置。
3. 固定定位和浮动不能同时设置，如果同时设置，**浮动失效**，以固定定位为主。
4. 固定定位的元素，也能通过 `margin`调整位置，但**不推荐**这样做。
5. 无论是什么元素（行内、行内块、块级）设置为固定定位之后，都变成了**定位元素**。

**何为定位元素？**

- 默认宽、高都被内容所撑开，且能自由设置宽高。



- **脱离文档流**：元素不再占据原始空间，后续元素会填补其位置。

- **定位基准**：相对于**浏览器窗口**，不随页面滚动而移动。

- **定位方式**：通过 `top`, `right`, `bottom`, `left` 指定偏移量来确定元素在视口中的具体位置。

- **应用场景**：创建固定的导航栏、返回顶部按钮、悬浮广告等需要在页面滚动时保持可见的界面元素。

- **示例**：

  ```css
  .fixed-element {
    position: fixed;
    bottom: 0; /* 固定在视窗底部 */
    right: 0; /* 固定在视窗右侧 */
    padding: 10px; /* 可选：为元素添加内边距 */
    background-color: white; /* 可选：设置背景颜色 */
    border: 1px solid #ccc; /* 可选：设置边框 */
  }
  ```

---

这种格式清晰地展示了固定定位的关键点和应用实例，有助于理解和记忆。固定定位是网页设计中非常实用的一种布局技术，特别适合用于实现那些需要持续对用户可见的UI组件。



```css
    position: fixed;
    top: 0px;
    z-index: 1000;    // 让固定定位的元素完全显示
```



---



**关键区别总结**

| 特性           | 绝对定位 (`absolute`)            | 相对定位 (`relative`)    |
| -------------- | -------------------------------- | ------------------------ |
| **文档流**     | 脱离文档流，不占空间             | 保留文档流，占据原空间   |
| **定位基准**   | 最近的已定位祖先元素或 `<body>`  | 自身原始位置             |
| **常见用途**   | 覆盖元素、模态框、精准定位       | 微调位置、创建定位上下文 |
| **父元素要求** | 需要父元素设置非 `static` 的定位 | 无特殊要求               |

---

**注意事项**

1. **层叠顺序**：定位元素可通过 `z-index` 控制堆叠层级，默认是0，其值越大越靠上。
2. **父容器限制**：绝对定位元素需父元素设置 `position: relative`（或其他非 `static` 值）以限制其定位范围。
3. **布局影响**：绝对定位可能导致内容重叠，需谨慎处理响应式布局中的尺寸问题。



#### 粘性定位

**4.1 如何设置为粘性定位？**

- 给元素设置 `position: sticky;`即可实现粘性定位。
- 可以使用 `left`、`right`、`top`、`bottom`四个属性调整位置，**不过最常用的是 `top`值**。

------

**4.2 粘性定位的参考点在哪里？**

- 离它最近的一个拥有 **“滚动机制”** 的祖先元素，即便这个祖先不是最近的真实可滚动祖先。

------

**4.3 粘性定位元素的特点**

1. 1.

   **不会脱离文档流**，它是一种专门用于窗口滚动时的新的定位方式。

2. 2.

   最常用的值是 `top`值。

3. 3.

   粘性定位和浮动可以同时设置，但**不推荐**这样做。

4. 4.

   粘性定位的元素，也能通过 `margin`调整位置，但**不推荐**这样做。

**核心特点总结：**

**粘性定位和相对定位的特点基本一致，不同的是：粘性定位可以在元素到达某个位置时将其固定。**



**定义**：

- **粘性定位** (`position: sticky;`) 是一种特殊的定位方式，它结合了相对定位和固定定位的优点。

**特性**：

- 元素默认按照文档流进行布局（相对定位）。
- 当页面滚动到某个预设的阈值时，元素会“固定”在指定位置（固定定位）。

**语法**：

```css
.sticky-element {
    position: sticky;
    top: 10px; /* 阈值，当元素距离视窗顶部10px时变为固定定位 */
}
```

**关键属性**：

- `position: sticky;`：声明元素使用粘性定位。
- `top`, `bottom`, `left`, `right`：定义元素变为固定定位的阈值。最常用的是`top`。

**示例**：

```html
<style>
    .sticky {
        position: sticky;
        top: 10px;
        background-color: #f1f1f1;
        padding: 10px;
        border: 2px solid #ddd;
    }
</style>

<div style="height: 1500px;">
    <div class="sticky">我是粘性定位的元素</div>
    <p>这里是一些页面内容。</p>
</div>
```

**应用场景**：

- **导航栏**：让导航栏在用户滚动页面时固定在屏幕顶部，方便用户操作。
- **侧边栏**：让侧边栏在用户滚动页面时固定在屏幕一侧，便于访问相关内容。
- **目录**：在长篇文章中，使目录部分固定在屏幕一侧，方便用户快速跳转。

**注意事项**：

- 粘性定位元素需要有一个具有滚动机制的父级容器，否则它的粘性效果不会生效。
- 在一些较老的浏览器版本中可能不支持`position: sticky;`，因此在实际项目中使用时需要注意兼容性问题。

---

通过合理利用粘性定位，你可以创建出既美观又实用的网页布局，提升用户的交互体验。希望这份笔记能帮助你更好地理解并应用粘性定位。



#### 定位的层级

1. 

   **定位元素的层级更高**：

   定位元素（无论何种定位）的显示层级比普通元素高，且所有定位类型的默认显示层级都一样。

2. 

   **默认的重叠规则**：

   如果发生位置重叠，默认后面的元素会显示在前面元素之上。

3. 

   **使用 `z-index`控制层级**：

   可以通过 CSS 属性 `z-index`来调整元素的显示层级。

4. 

   **`z-index`的属性值**：

   `z-index`的值是数字（没有单位），**数字越大，显示层级越高**。

5. 

   **`z-index`的生效条件**：

   **只有定位的元素**（即设置了 `position`且值非 `static`的元素）设置 `z-index`才会生效。

6. 

   **调试提示**：

   如果 `z-index`值大的元素没有覆盖值小的元素，请检查其**包含块**的层级。

##### **Z-index** 

是 CSS 中用于控制元素在堆叠上下文（stacking context）中的层级顺序的属性。它决定了当多个元素重叠时，哪个元素会显示在前面或后面。理解 `z-index` 的工作原理对于创建复杂的布局和确保界面元素按预期显示非常重要。

**基本概念**

- **堆叠顺序（Stacking Order）**：页面上的每个元素都有一个默认的堆叠顺序。默认情况下，后面的元素会在视觉上覆盖前面的元素。
- **Z-index 属性**：通过设置 `z-index` 属性，可以改变元素的堆叠顺序。值越大，元素越靠前；值越小，元素越靠后。默认值为 `auto`，即元素遵循其自然堆叠顺序。



```
.element {
    z-index: 1; /* 设置元素的堆叠层级 */
}
```



**使用方法**

- **数值范围**：`z-index` 可以接受正整数、负整数和 `auto`。较大的正值会使元素显示在前面，而较大的负值会使元素显示在后面。

  css

  深色版本

  

  ```
  .front {
      z-index: 10;
  }
  
  .back {
      z-index: -1;
  }
  ```

- **必须结合定位使用**：为了使 `z-index` 生效，元素必须具有以下任一定位属性：

  - `position: relative;`
  - `position: absolute;`
  - `position: fixed;`
  - `position: sticky;`

  css

  深色版本

  

  ```
  .element {
      position: relative;
      z-index: 1;
  }
  ```



**堆叠上下文（Stacking Context）**

- **堆叠上下文** 是指一组元素的堆叠顺序被独立管理的情况。一个新的堆叠上下文可以通过以下方式创建：
  - 根元素 (`<html>`)
  - `position` 值为 `absolute` 或 `relative` 且 `z-index` 不是 `auto`
  - `position` 值为 `fixed` 或 `sticky`
  - 元素具有 `opacity` 小于 1
  - 元素具有 `transform` 不是 `none`
  - 等等...
- 在同一个堆叠上下文中，`z-index` 的值决定元素的显示顺序。而在不同的堆叠上下文中，子元素的 `z-index` 只在其父级堆叠上下文中有效。



#### 定位的特殊应用

**注意：**

1. 1.

   发生**固定定位**、**绝对定位**后，元素都变成了**定位元素**，默认宽高被内容撑开，且依然可以设置宽高。

2. 2.

   发生**相对定位**后，元素依然是之前的显示模式。

3. 3.

   以下所说的特殊应用，只针对**绝对定位**和**固定定位**的元素，**不包括相对定位**的元素。

------

**让定位元素的宽/高充满包含块**

- **宽度与包含块一致**：给定位元素同时设置 `left: 0;`和 `right: 0;`。
- **高度与包含块一致**：给定位元素同时设置 `top: 0;`和 `bottom: 0;`。

------

**让定位元素在包含块中居中**

**方案一：**

```css
left: 0;
right: 0;
top: 0;
bottom: 0;
margin: auto;
```

**方案二：使用负外边距实现定位元素居中**

通过计算，先将元素左上角移动至包含块中心点，再通过负外边距将元素拉回，实现元素中心与包含块中心对齐。

**CSS代码方案：**

```css
left: 50%;
top: 50%;
margin-left: -宽度值的一半;
margin-top: -高度值的一半;
```

**重要注意事项：**

⚠️ **该定位的元素必须设置宽高！！！** ⚠️





### 布局

#### 版心

**1. 定义**

在PC端网页中，一般都会有一个**固定宽度**且**水平居中**的盒子，来显示网页的主要内容，这个盒子就是网页的**版心**。

**2. 版心宽度**

版心的宽度一般在 **960~1200像素** 之间（图中用红色圆圈特别强调了此范围，并单独标注了数字 **900** 作为示例）。

**3. 数量**

版心可以是一个，也可以是多个。



#### 常用类名

| 位置                   | 对应名词（CSS 类名常用）     |
| :--------------------- | :--------------------------- |
| **顶部导航条**         | `topbar`                     |
| **页头**               | `header`, `page-header`      |
| **导航**               | `nav`, `navigator`, `navbar` |
| **搜索框**             | `search`, `search-box`       |
| **横幅、广告、宣传图** | `banner`                     |
| **主要内容**           | `content`, `main`            |
| **侧边栏**             | `aside`, `sidebar`           |
| **页脚**               | `footer`, `page-footer`      |



### 重置默认样式

**HTML 元素的默认样式**

很多元素都有默认样式，例如：

1. **`<p>`元素**：有默认的上下 `margin`。
2. **`<h1>`~ `<h6>`元素**：有默认的上下 `margin`，并且字体加粗。
3. **`<body>`元素**：有默认的 `8px`外边距。
4. **超链接 (`<a>`)**：有默认的文字颜色和下划线。
5. **`<ul>`元素**：有默认的左 `padding`。
6. ……

------

**为何需要重置默认样式？**

在早期，这些默认样式为快速创建简单页面提供了便利。但在现代追求精细设计的复杂网页中，这些默认样式不仅会带来麻烦，而且在不同的浏览器中表现可能不一致。因此，我们需要将它们“重置”。

------

##### **方案一：使用全局选择器**

通过 CSS 全局选择器 (`*`) 来清除所有元素的默认外边距和内边距。

**CSS 代码：**

```css
* {
    margin: 0;
    padding: 0;
}
```

**评价：**

- 在简单案例中可以临时使用。
- **实际开发中不推荐使用**，原因：
  1. `*`会选择所有元素，但并非所有元素都有默认样式。
  2. 重置时通常需要做特定处理（例如：想让 `<a>`元素的文字是灰色，其他元素文字是蓝色）。

------

##### **方案二：reset.css**

**原理：**

选择具有默认样式的元素，清空其默认样式。

**效果：**

经过 reset 后的网页，好似“一张白纸”，开发人员可根据设计稿，精细地去添加具体的样式。

------

##### **方案三：Normalize.css**

**原理：**

一种最新方案，在清除默认样式的基础上，**保留了一些有价值的默认样式**。

**官方网站：**

http://necolas.github.io/normalize.css/

**相对于 reset.css 的优点：**

1. 保护了有价值的默认样式，而不是完全去掉它们。
2. 为大部分HTML元素提供一般化的样式
3. 新增对HTML5元素的设置
4. 对并集选择器的使用比较谨慎，有效避免调试工作杂乱

* 备注：

**Normalize.css 的重置，和 reset.css 相比，更加的温和，开发时可根据实际情况进行选择。**





### 字体图标

在网页设计中，字体图标是一种使用字体文件来显示图标的特殊技术。它们实际上是基于矢量的图形，可以无损地缩放到任意大小，并且可以通过CSS轻松调整其样式。以下是关于字体图标的一些关键点和应用示例。

---

#### **字体图标（Icon Fonts）**

- **矢量图形**：字体图标是基于矢量的，这意味着它们可以无损地缩放到任意大小，非常适合响应式设计。

- **易于修改**：由于字体图标本质上是文本字符，因此可以通过CSS轻松调整其颜色、大小、阴影等属性，就像操作普通文本一样简单。

- **轻量化**：相比图片图标，字体图标通常具有更小的文件大小，并且只需加载一次即可在整个网站中复用，有助于提高网页加载速度。

- **兼容性好**：字体图标支持所有现代浏览器，包括移动设备上的浏览器，同时在不同操作系统上也有一致的表现。

- **常见字体图标库**：
  - **Font Awesome**
  - **Material Icons**
  - **Ionicons**

---

#### **阿里巴巴 Iconfont 使用指南**

**注册并登录**

1. 访问 [Iconfont](https://www.iconfont.cn/) 并注册一个账号（如果还没有的话），然后登录。
2. 搜索和收藏图标，并将它们添加到您的项目中。

**创建项目并管理图标**

1. 在项目页面中，点击“下载至本地”，选择合适的格式（如 `Symbol` 或 `Font class`）进行下载。
2. 将下载的文件解压，并引入到您的项目中。

**下载为 Symbol（SVG Sprite）**

```html
<head>
  <script src="./path/to/iconfont.js"></script>
  <style>
    .icon {
      width: 1em;
      height: 1em;
      vertical-align: -0.15em;
      fill: currentColor;
      overflow: hidden;
    }

    .custom-icon {
      font-size: 200px;
      color: brown;
    }
  </style>
</head>
<body>
  <!-- 使用 Iconfont 图标 -->
  <svg class="icon custom-icon" aria-hidden="true">
    <use xlink:href="#icon-kuandai"></use>
  </svg>
</body>
```

**下载为 Font class**

```html
<head>
  <link rel="stylesheet" href="./path/to/iconfont.css">
  <style>
    .custom-icon {
      font-size: 200px;
      color: brown;
    }
  </style>
</head>
<body>
  <!-- 使用 Iconfont 图标 -->
  <i class="iconfont icon-kuandai custom-icon"></i>
</body>
```



##### 注意

建议根据随下载的指导文档或参考以下代码

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Icon Example</title>
    <style>
        @font-face {
            font-family: 'iconfont';
            src: url('./icon/iconfont.ttf'),
                url('./icon/iconfont.woff2'),
                url('./icon/iconfont.woff');
        }

        .iconfont {
            font-family: "iconfont" !important;
            font-size: 16px;
            font-style: normal;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        .webpaper {
            font-size: 200px;
            /* color:cyan; */
        }
    </style>
</head>

<body>
    <span class="iconfont webpaper">&#xe991;</span>
</body>

</html>
```



#### **总结**

字体图标极大地简化了网页设计中的图标管理，使得开发者能够更加高效地创建美观且功能强大的用户界面。无论是简单的导航栏图标还是复杂的交互元素，字体图标都是一个非常实用的选择。

- **Font Awesome** 提供了丰富的图标集和便捷的集成方式，适合快速开发和原型设计。
- **阿里巴巴 Iconfont** 提供了更多的自定义选项和灵活的集成方式，特别适合国内开发者使用。





### 动画属性

#### 2D变换

前提：二维坐标系如下图所示

------

##### 1. 2D位移

**traslate**

2D位移可以改变元素的位置，具体使用方式如下：

1. 先给元素添加转换属性 `transform`。
2. 编写 `transform` 的具体值，相关可选值如下：

| 值           | 含义                                                         |
| ------------ | ------------------------------------------------------------ |
| `translateX` | 设置水平方向位移，需指定长度值；若指定的是百分比，是参考自身宽度的百分比。 |
| `translateY` | 设置垂直方向位移，需指定长度值；若指定的是百分比，是参考自身高度的百分比。 |
| `translate`  | 一个值代表水平方向，两个值代表：水平和垂直方向。             |

1. 注意点：

   1. 位移与相对定位很相似，都不脱离文档流，不会影响到其它元素。

   2. 与相对定位的区别：相对定位的百分比值，参考的是其父元素；定位的百分比值，参考的是其自身。

   3. 浏览器针对位移有优化，与定位相比，浏览器处理位移的效率更高。

   4. `transform`可以链式编写，例如：

      ```css
      transform: translateX(30px) translateY(40px);
      ```

   5. 位移对行内元素无效。

   6. 位移配合定位，可实现元素水平垂直居中

      ```css
      .box {
          position: absolute;
          left: 50%;
          top: 50%;
          transform: translate(-50%, -50%);
      }
      ```

##### 2. 2D缩放

**scale**

缩放是指：让元素放大或缩小，具体使用方式如下：

1. 先给元素添加转换属性 `transform`。
2. 编写 `transform` 的具体值，相关可选值如下：

| 值       | 含义                                                         |
| -------- | ------------------------------------------------------------ |
| `scaleX` | 设置水平方向的缩放比例，值为一个数字，1 表示不缩放，大于 1 放大，小于 1 缩小。 |
| `scaleY` | 设置垂直方向的缩放比例，值为一个数字，1 表示不缩放，大于 1 放大，小于 1 缩小。 |
| `scale`  | 同时设置水平方向、垂直方向的缩放比例，一个值代表同时设置水平和垂直缩放；两个值分别代表：水平缩放、垂直缩放。 |

* 注意点：

1. `scale` 的值，是支持写负数的，但几乎不用，因为容易让人产生误解。
2. 借助缩放，可实现小于 12px 的文字。

##### 3. 2D旋转

**rotate**

旋转是指：让元素在二维平面内，顺时针旋转或逆时针旋转，具体使用方式如下：

1. 先给元素添加转换属性 `transform`。
2. 编写 `transform` 的具体值，相关可选值如下：

| 值       | 含义                                                         |
| -------- | ------------------------------------------------------------ |
| `rotate` | 设置旋转角度，需指定一个角度值 (deg)，正值顺时针，负值逆时针。 |

注意：`rotateZ(20deg)` 相当于 `rotate(20deg)`，当然到了 3D 变换的时候，还能写：`rotate(x, x, x)`

##### 4.  2D扭曲（了解）

**skew**

扭曲是指：让元素在二维平面内被“拉扯”，进而“走形”。实际开发几乎不用，了解即可，具体使用方式如下：

1. 先给元素添加转换属性 `transform`。
2. 编写 `transform` 的具体值，相关可选值如下：

| 值      | 含义                                                         |
| ------- | ------------------------------------------------------------ |
| `skewX` | 设置元素在水平方向扭曲，值为角度值，会将元素的左上角、右下角拉扯。 |
| `skewY` | 设置元素在垂直方向扭曲，值为角度值，会将元素的左上角、右下角拉扯。 |
| `skew`  | 一个值代表 `skewX`，两个值分别代表：`skewX`、`skewY`         |

##### 5.  2D多重变换

多个变换，可以同时使用一个 `transform` 来编写。

```css
transform: translate(-50%, -50%) rotate(45deg);
```

注意点：多重变换时，建议最后旋转。

##### 6.  变换原点

**transform-origin**

- 元素变换时，默认的原点是元素的中心，使用 `transform-origin` 可以设置变换的原点。
- 修改变换原点对位移没有影响，对旋转和缩放会产生影响。
- 如果提供两个值，第一个用于横坐标，第二个用于纵坐标。
- 如果只提供一个，若是像素值，表示横坐标，纵坐标取 50%；若是关键词，则另一个坐标取 50%。
  * `transform-origin: 50% 50%;` 变换原点在元素的中心位置，百分比是相对于自身。——默认值
  * `transform-origin: left top;` 变换原点在元素的左上角。
  * `transform-origin: 50px 50px;` 变换原点距离元素左上角 50px 50px 的位置。
  * `transform-origin: 0;` 只写一个值的时候，第二个值默认为 50%。



#### 3D变换

##### 1.   3D空间与景深

* 开启3D空间

  `transform-style` 

重要原则：元素进行 3D 变换的首要操作：**父元素**必须开启 3D 空间！

使用 `transform-style` 开启 3D 空间，可选值如下：

1. `flat`：让子元素位于此元素的二维平面内（2D 空间）——默认值
2. `preserve-3d`：让子元素位于此元素的三维空间内（3D 空间）

* 设置景深

  `perspective`

何为景深？——指定观察者与 z=0 平面的距离，能让发生 3D 变换的元素，产生透视效果，看来更加立体。

使用 `perspective` 设置景深，可选值如下：

1. `none`：不指定透视——（默认值）

2. 长度值：指定观察者距离 z=0 平面的距离，不允许负值。

注意：`perspective` 设置给发生 3D 变换元素的父元素！

##### 2.   透视点的位置

所谓透视点位置，就是观察者位置；默认的透视点在元素的中心。

使用 `perspective-origin` 设置观察者位置（透视点的位置），例如：

```css
/* 相对坐标轴向右偏移400px，往下偏移300px（相当于人蹲下300像素，然后向右移动400像素看元素）*/
perspective-origin: 400px 300px;
```

注意：通常情况下，我们不需要调整透视点位置。

##### 3.   3D位移

**translate**

3D 位移是在 2D 位移的基础上，可以让元素沿 z 轴位移，具体使用方式如下：

1. 先给元素添加转换属性 `transform`。
2. 编写 `transform` 的具体值，3D 相关可选值如下：

| 值            | 含义                                                         |
| ------------- | ------------------------------------------------------------ |
| `translateZ`  | 设置 z 轴位移，需指定长度值，正值向屏幕外，负值向屏幕里，且不能写百分比。 |
| `translate3d` | 第 1 个参数对应 x 轴，第 2 个参数对应 y 轴，第 3 个参数对应 z 轴，且均不能省略。 |

#####  4.   3D旋转

**rotate**

3D 旋转是在 2D 旋转的基础上，可以让元素沿 x 轴和 y 轴旋转，具体使用方式如下：

1. 先给元素添加转换属性 `transform`。
2. 编写 `transform` 的具体值，3D 相关可选值如下：

| 值         | 含义                                                         |
| ---------- | ------------------------------------------------------------ |
| `rotateX`  | 设置 x 轴旋转角度，需指定一个角度值 (deg)，面对 x 轴正方向：正值顺时针，负值逆时针。 |
| `rotateY`  | 设置 y 轴旋转角度，需指定一个角度值 (deg)，面对 y 轴正方向：正值顺时针，负值逆时针。 |
| `rotate3d` | 前 3 个参数分别表示坐标轴：x, y, z，第 4 个参数表示旋转的角度，参数不允许省略。<br>例如：`transform: rotate3d(1,1,1,30deg)`，意思是：x、y、z 分别旋转 30 度。 |

##### 5.  3D缩放

3D缩放是在2D缩放的基础上，可以让元素沿z轴缩放。

使用方式

1.先给元素添加转换属性`transform`。

2.编写`transform`的具体值，3D相关可选值如下：

* **`scaleZ`**：设置z轴方向的缩放比例，值为一个数字，1表示不缩放，大于1放大，小于1缩小。

- **`scale3d`**：第1个参数对应x轴，第2个参数对应y轴，第3个参数对应z轴，参数不允许省略。

##### 6.   3D的多重变换

多个变换,可以同时使用一个 transform 来编写。

```css
transform: translateZ(100px) scaleZ(3) rotateY(40deg);
```

> 注意点:多重变换时,建议最后旋转。

##### 7.  背部可见性

**backface-visibility**

在使用 CSS 3D 变换（比如 `transform: rotateY(180deg)`或 `rotateX()`等）时，一个元素实际上是有 **正面（front face）和背面（back face）** 的，就像一张卡片有正反两面。

默认情况下：

- **正面**：是你正常书写和看到的那一面（通常是元素初始状态）。
- **背面**：是当元素绕某个轴（如 Y 轴）翻转 180 度后你看到的那一面。

`backface-visibility`的作用

该属性决定了：**当元素的背面朝向用户时，是否显示这个背面。**

语法：

```css
backface-visibility: visible | hidden;
```

取值：

- **`visible`（默认值）**：即使元素的背面朝向用户，也依然可见。也就是说，你可以看到元素的“背面”。
- **`hidden`**：如果元素的背面朝向用户，则这个背面**不可见**（相当于隐藏了）。常用来实现“翻转卡片”只显示正面的效果。





#### 过渡

##### 使用

过渡可以在不使用 Flash 动画，不使用 JavaScript 的情况下，让元素从一种样式，平滑过渡为另一种样式。

1. **transition-property**

- **作用**：定义哪个属性需要过渡，只有在该属性中定义的属性（比如宽、高、颜色等）才会以有过渡效果。
- 常用值
  1. `none`：不过渡任何属性。
  2. `all`：过渡所有能过渡的属性。
  3. 具体某个属性名，例如：`width`、`height`，若有多个以逗号分隔。

不是所有的属性都能过渡，值为数字，或者值能转为数字的属性，都支持过渡，否则不支持过渡。常见的支持过渡的属性有：颜色、长度值、百分比、`z-index`、`opacity`、2D 变换属性、3D 变换属性、阴影。

2. **transition-duration**

- **作用**：设置过渡的持续时间，即：一个状态过渡到另外一个状态耗时多久。

- 常用值

  1. `0`：没有任何过渡时间——默认值。
  2. `s` 或 `ms`：秒或毫秒。
  3. 列表：
     - 如果想让所有属性都持续一个时间，那就写一个值。
     - 如果想让每个属性持续不同的时间那就写一个时间的列表。

  ```css
      <style>
  
          .box1 {
              width: 200px;
              height: 200px;
              background-color: #676767;
              /* 设置哪个属性需要过度 */
              /* transition-property: background-color, height, width; */
              /* 让能过渡的元素都过渡 */
              transition-property: all;
              /* 设置过渡时间 */
              transition-duration: 2s;
  
          }
  
          .box1:hover {
              background-color: aqua;
              height: 100px;
              width: 100px;
          }
      </style>
  </head>
  
  <body>
      <div class="box1"></div>
  </body>
  
  ```

  **淡入淡出效果（最常用）**

  ```css
  .hidden-content {
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.3s ease, visibility 0.3s ease;
  }
  
  .parent:hover .hidden-content {
      opacity: 1;
      visibility: visible;
  }
  ```

  > ✅ 效果：内容平滑淡入淡出
  > 💡 `visibility` 确保元素完全隐藏时不占用布局空间

3.  **transition-delay**

- **作用**：指定开始过渡的延迟时间，单位：s 或 ms。

4.  **transition-timing-function**

- **作用**：设置过渡的类型。
- 常用值
  1. `ease`：平滑过渡——默认值。
  2. `linear`：线性过渡。
  3. `ease-in`：慢 → 快。
  4. `ease-out`：快 → 慢。
  5. `ease-in-out`：慢 → 快 → 慢。
  6. `step-start`：等同于 `steps(1, start)`。
  7. `step-end`：等同于 `steps(1, end)`。
  8. `steps(integer, ?)`：接受两个参数的步进函数。第一个参数必须为正整数，指定函数的步数。第二个参数取值可以是 `start` 或 `end`，指定每一步的值发生变化的时间点。第二个参数默认值为 `end`。
  9. `cubic-bezier(number, number, number, number)`：特定的贝塞尔曲线类型。

在线制作贝塞尔曲线：https://cubic-bezier.com/



##### 复合属性

如果设置了一个时间，表示 `duration`；如果设置了两个时间，第一个是 `duration`，第二个是 `delay`；其他值没有顺序要求。

```css
transition: 1s 1s linear all;
```

transition: 属性 时长 速度曲线 延迟;



#### 动画

##### 基本使用 

1. 什么是帧

- 一段动画，就是一段时间内连续播放 n 个画面。每一张画面，我们管它叫做“帧”。一定时间内连续快速播放若干个帧，就成了人眼中所看到的动画。同样时间内，播放的帧数越多，画面看起来越流畅。

2. 什么是关键帧

- 关键帧指的是，在构成一段动画的若干帧中，起到决定性作用的 2-3 帧。



**第一步：定义关键帧（定义动画）**

1. 简单方式定义：

```css
/*写法一*/
@keyframes 动画名 {
    from {
        /*property1:value1*/
        /*property2:value2*/
    }
    to {
        /*property1:value1*/
    }
}
```

2. 完整方式定义：

```css
@keyframes 动画名 {
    0% {
        /*property1:value1*/
    }
    20% {
        /*property1:value1*/
    }
    40% {
        /*property1:value1*/
    }
    60% {
        /*property1:value1*/
    }
    80% {
        /*property1:value1*/
    }
    100% {
        /*property1:value1*/
    }
}
```

第二步：给元素应用动画，用到的属性如下：

1. `animation-name`：给元素指定具体的动画（具体的关键帧）
2. `animation-duration`：设置动画所需时间
3. `animation-delay`：设置动画延迟

```css
.box {
    /* 指定动画 */
    animation-name: testKey;
    /* 设置动画所需时间 */
    animation-duration: 5s;
    /* 设置动画延迟 */
    animation-delay: 0.5s;
}
```



##### 其他属性

动画属性详解

* `animation-timing-function`，设置动画的类型，常用值如下：

1. `ease`：平滑动画 —— 默认值
2. `linear`：线性过渡
3. `ease-in`：慢 → 快
4. `ease-out`：快 → 慢
5. `ease-in-out`：慢 → 快 → 慢
6. `step-start`：等同于 `steps(1, start)`
7. `step-end`：等同于 `steps(1, end)`
8. `steps(integer, ?)`：接受两个参数的步进函数。第一个参数必须为正整数，指定函数的步数。第二个参数取值可以是 `start` 或 `end`，指定每一步的值发生变化的时间点。第二个参数默认值为 `end`。
9. `cubic-bezier(number, number, number, number)`：特定的贝塞尔曲线类型。

* `animation-iteration-count`，指定动画的播放次数，常用值如下：

1. `number`：动画循环次数
2. `infinite`：无限循环

*  `animation-direction`，指定动画方向，常用值如下：

1. `normal`：正常方向（默认）
2. `reverse`：反方向运行
3. `alternate`：动画先正常运行再反方向运行，并持续交替运行
4. `alternate-reverse`：动画先反运行再正方向运行，并持续交替运行

* `animation-fill-mode`，设置动画之外的状态

1. `forwards`：设置对象状态为动画结束时的状态
2. `backwards`：设置对象状态为动画开始时的状态

* `animation-play-state`，设置动画的播放状态，常用值如下：

1. `running`：运动（默认）
2. `paused`：暂停



##### 复合属性

```css
animation-name
animation-duration
animation-delay

animation-timing-function
animation-iteration-count
animation-direction
animation-fill-mode
animation-play-state
```

* `animation-name  `      

​	**动画名称**
​	 作用：指定你要使用的**关键帧动画的名字**。这个名字必须和 `@keyframes 动画名` 中定义的	名	字一致。

 	示例：`animation-name: slideIn;` 表示使用名为 `slideIn` 的关键帧动画。

* `animation-duration`

  动画持续时间

 作用：设置动画从开始到结束需要多长时间。

 单位：秒（`s`）或毫秒（`ms`）。

 示例：`animation-duration: 2s;` 表示动画持续 2 秒。

* `animation-timing-function`
  **动画时间函数 / 缓动效果**
  作用：控制动画在**时间上的播放节奏**，比如是匀速、先快后慢，还是分步跳转。
  常见值：
  1. `ease`：慢开始，快中间，慢结束（默认）
  2. `linear`：匀速播放
  3. `ease-in`：慢开始，快结束
  4. `ease-out`：快开始，慢结束
  5. `ease-in-out`：慢快慢
  6. `steps(3, end)`：分 3 步跳着播放（适合帧动画）`cubic-bezier()`：自定义贝塞尔曲线

* `animation-iteration-count`
  **动画播放次数**
  作用：设置动画播放多少次。
  常见值：
  1. `1`：播放 1 次（默认）
  2. `3`：播放 3 次
  3. `infinite`：无限循环播放

* **`animation-direction`**
  **动画播放方向**
  作用：控制动画是否反向播放或来回播放。
  常见值：
  1. `normal`：正常方向播放（默认）
  2. `reverse`：反方向播放
  3. `alternate`：奇数次正向，偶数次反向（来回播放）
  4. `alternate-reverse`：奇数次反向，偶数次正向

* **`a0nimation-fill-mode`**
  **动画填充模式**
  作用：定义动画**在开始前和结束后**，元素保持什么状态。
  常见值：
  1. `none`：动画外不应用任何样式（默认）
  2. `forwards`：动画结束后，保持最后一帧的样式
  3. `backwards`：动画开始前，使用第一帧的样式（通常不明显）
  4. `both`：结合 `forwards` 和 `backwards`

* **`animation-play-state`**
  **动画播放状态**
  作用：控制动画是**正在播放还是暂停**。
  常见值：
  1. `running`：播放（默认）
  2. `paused`：暂停
     示例：可用于鼠标悬停时暂停动画：

```css
.box:hover {
  animation-play-state: paused;
}
```

✅ 总结表格

| 属性名                      | 中文含义 | 常见用途           |
| --------------------------- | -------- | ------------------ |
| `animation-name`            | 动画名称 | 指定关键帧动画     |
| `animation-duration`        | 持续时间 | 控制动画长短       |
| `animation-delay`           | 延迟时间 | 设置开始前等待多久 |
| `animation-timing-function` | 缓动效果 | 控制动画节奏       |
| `animation-iteration-count` | 播放次数 | 设定循环次数       |
| `animation-direction`       | 播放方向 | 正放、反放、来回   |
| `animation-fill-mode`       | 填充模式 | 动画前后保持状态   |
| `animation-play-state`      | 播放状态 | 暂停或继续         |

------

这些属性可以单独使用，也可以用简写属性 `animation` 一起写：

```css
.box {
  animation: slideIn 2s 0.5s ease-in infinite alternate forwards;
}
```



##### 过渡与动画的区别

- **过渡（Transition）**：描述**两个状态之间**如何平滑地变化，需要**触发条件**（如鼠标悬停）。
- **动画（Animation）**：定义**一系列关键帧**，可以自动播放、循环、更复杂地控制整个动画过程。

------

✅ 二、详细对比

| 特性                   | **过渡（Transition）**                               | **动画（Animation）**                               |
| ---------------------- | ---------------------------------------------------- | --------------------------------------------------- |
| **是否需要触发**       | ✅ 必须由用户行为触发（如 `:hover`, `:focus`）        | ❌ 可以自动播放，无需用户交互                        |
| **是否自动播放**       | ❌ 不会自动播放                                       | ✅ 可以设置 `animation-play-state: running` 自动播放 |
| **是否支持循环**       | ❌ 只能来回切换状态，不支持真正循环                   | ✅ 支持无限循环 `infinite`                           |
| **是否支持多个关键帧** | ❌ 只能从 A 状态到 B 状态（`from` → `to`）            | ✅ 支持多个关键帧（`0%`, `25%`, `50%`, `100%`）      |
| **是否支持反向播放**   | ✅ 可以通过 `transition` 反向生效                     | ✅ 支持 `animation-direction: alternate` 来回播放    |
| **是否可暂停**         | ❌ 不易控制暂停                                       | ✅ 可通过 `animation-play-state: paused` 暂停        |
| **是否依赖状态变化**   | ✅ 必须有 CSS 属性变化（如 `width` 从 100px → 200px） | ❌ 不依赖，可独立运行                                |
| **是否支持填充模式**   | ❌ 不支持                                             | ✅ 支持 `animation-fill-mode: forwards` 保持最终状态 |
| **控制精细度**         | ⭐ 一般，适合简单变化                                 | ⭐⭐⭐ 高，适合复杂动画                                |



#### transfrom	transition	animation 的区别

| 属性         | 作用                             | 类比                       | 说明                                                         |
| ------------ | -------------------------------- | -------------------------- | ------------------------------------------------------------ |
| `transform`  | **让元素变形或移动**（静态）     | “动作本身”：比如伸展、旋转 | 单独用时，**是瞬间完成的**，没有动画效果                     |
| `transition` | **让变化“慢慢来”**（需要触发）   | “慢动作播放”：让变形变柔和 | 让某个属性的变化**有过渡效果**（比如从红变蓝，慢慢渐变）,需要**触发** |
| `animation`  | **自动播放的复杂动画**（可循环） | “自动播放的动画片”         | 不需要用户触发（可以自动播放），能做更复杂的动画序列         |

### 多列布局

一般做新闻可以这么做

常用属性如下：

- `column-count`：指定列数，值是数字。
- `column-width`：指定列宽，值是长度。
- `columns`：同时指定列宽和列数，复合属性；值没有数量和顺序要求。
- `column-gap`：设置列边距，值是长度。
- `column-rule-style`：设置列与列之间边框的风格，值与 `border-style` 一致。
- `column-rule-width`：设置列与列之间边框的宽度，值是长度。
- `column-rule-color`：设置列与列之间边框的颜色。
- `column-rule`：设置列边框，复合属性。
- `column-span`：指定是否跨列；值: `none`、`all`。





### 伸缩盒模型

#### 伸缩盒模型简介

- **2009 年，W3C 提出了一种新的盒子模型——Flexible Box（伸缩盒模型，又称：弹性盒子）。**
- 它可以轻松地控制：元素分布方式、元素对齐方式、元素视觉顺序……
- 截止目前，除了在部分 IE 浏览器不支持，其他浏览器均已全部支持。
- 伸缩盒模型的出现，逐渐演变出了一套新的布局方案——**flex 布局。**

>😀小贴士：
>
>1. 传统布局是指：基于传统盒状模型，主要靠：`display` 属性 + `position` 属性 + `float` 属性。
>2. flex 布局目前在移动端应用比较广泛，因为传统布局不能很好地呈现在移动设备上。



#### 伸缩容器、伸缩项目

伸缩容器：

- **定义**：开启了 `flex` 的元素，就是伸缩容器。

1. 给元素设置 `display: flex` 或 `display: inline-flex`，该元素就变为了伸缩容器。
2. `display: inline-flex` 很少使用，因为可以给多个伸缩容器的父容器，也设置为伸缩容器。
3. 一个元素可以同时是：伸缩容器、伸缩项目。

伸缩项目：

- **定义**：伸缩容器所有子元素自动成为了伸缩项目。

1. 仅伸缩容器的子元素成为了伸缩项目，孙子元素、重孙子元素等后代，不是伸缩项目。
2. 无论原来是哪种元素（块、行内块、行内），一旦成为了伸缩项目，全都会“块状化”。



#### 主轴方向

##### 主轴与侧轴

- **主轴**：伸缩项目沿着主轴排列，主轴默认是水平的，默认方向是从左到右（左边是起点，右边是终点）。
- **侧轴**：与主轴垂直的就是侧轴，侧轴默认是垂直的，默认方向是从上到下（上边是起点，下边是终点）。

------

##### 主轴方向

- **属性名**：`flex-direction`
- 常用值如下
  1. `row`：主轴方向水平从左到右 —— 默认值
  2. `row-reverse`：主轴方向水平从右到左
  3. `column`：主轴方向垂直从上到下
  4. `column-reverse`：主轴方向垂直从下到上

注意：

改变了主轴的方向，侧轴方向也随之改变。



#### 主轴换行

属性名：`flex-wrap`

`nowrap`：默认值，不换行。

![image-20250909150111172](./笔记/web-img/image-20250909150111172.png)

`wrap`：自动换行，伸缩容器不够时自动换行。

![image-20250909150130947](./笔记/web-img/image-20250909150130947.png)

`wrap-reverse`：反向换行。

![image-20250909150145448](./笔记/web-img/image-20250909150145448.png)



#### flex-flow

- `flex-flow` 是一个复合属性，复合了 `flex-direction` 和 `flex-wrap` 两个属性。值没有顺序要求。

```css
flex-flow: row wrap;
```





#### 主轴对齐方式

属性名：`justify-content`

- 常用值如下
  1. `flex-start`：主轴起点对齐。—— 默认值
  2. `flex-end`：主轴终点对齐。
  3. `center`：居中对齐。
  4. `space-between`：均匀分布，两端对齐（最常用）。
  5. `space-around`：均匀分布，两端距离是中间距离的一半。
  6. `space-evenly`：均匀分布，两端距离与中间距离一致。

![image-20250909151014062](./笔记/web-img/image-20250909151014062.png)

#### 侧轴对齐

 1.只有一行的情况

- **所需属性**：`align-items`
- 常用值如下
  1. `flex-start`：侧轴的起点对齐。
  2. `flex-end`：侧轴的终点对齐。
  3. `center`：侧轴的中点对齐。
  4. `baseline`：伸缩项目的第一行文字的基线对齐。
  5. `stretch`：如果伸缩项目未设置高度，将占满整个容器的高度。——（默认值）

<img src="./笔记/web-img/image-20250909151835146.png" alt="image-20250909151835146" style="zoom: 67%;" />

<img src="./笔记/web-img/image-20250909151856490.png" alt="image-20250909151856490" style="zoom:67%;" />







2.多行的情况

所需属性：`align-content`

- 常用值如下
  1. `flex-start`：与侧轴的起点对齐。
  2. `flex-end`：与侧轴的终点对齐。
  3. `center`：与侧轴的中点对齐。
  4. `space-between`：与侧轴两端对齐，中间平均分布。
  5. `space-around`：伸缩项目间的距离相等，比距边缘大一倍。
  6. `space-evenly`：在侧轴上完全平分。
  7. `stretch`：占满整个侧轴。——默认值

![image-20250909152633503](./笔记/web-img/image-20250909152633503.png)

<img src="./笔记/web-img/image-20250909152701051.png" alt="image-20250909152701051" style="zoom: 67%;" />

<img src="./笔记/web-img/image-20250909152724476.png" alt="image-20250909152724476" style="zoom:67%;" />



#### 元素的水平垂直居中

方案一：

给父容器

```css
display:flex;
justify-content:center;
align-items:center;
```

方案二：

给父元素

```css
display:flex;
```

给子元素

```css
margin:auto;
```





#### 基准长度

flex-basis

- **概念**：`flex-basis` 设置的是主轴方向的基准长度，会让宽度或高度失效。
  - **备注**：主轴横向：宽度失效；主轴纵向：高度失效
- **作用**：浏览器根据这个属性设置的值，计算主轴上是否有多余空间，默认值 `auto`，即：伸缩项目的宽或高。





#### 拉伸

 **flex-grow（伸）**

- **概念**：`flex-grow` 定义伸缩项目的放大比例，默认为 `0`，即：纵使主轴存在剩余空间，也不拉伸（放大）。
- **规则**：
  1. 若所有伸缩项目的 `flex-grow` 值都为 `1`，则：它们将等分剩余空间（如果有空间的话）。
  2. 若三个伸缩项目的 `flex-grow` 值分别为 `1`、`2`、`3`，则：分别瓜分到 `1/6`、`2/6`、`3/6` 的空间



#### 压缩

**flex-shrink（缩）**

- **概念**：`flex-shrink` 定义了项目的压缩比例，默认为 `1`，即：如果空间不足，该项目将会缩小。
- **收缩项目的计算**，略微复杂一点，我们拿一个场景举例：

例如：

三个收缩项目，宽度分别为：200px、300px、200px，它们的 `flex-shrink` 值分别为：1、2、3。 若想刚好容纳下三个项目，需要总宽度为 700px，但目前容器只有 400px，还差 300px。 所以每个人都要收缩一下才可以放下，具体收缩的值，这样计算：

1. 计算分母：(200×1) + (300×2) + (200×3) = 1400
2. 计算比例：
   - 项目一：(200×1) / 1400 = 比例值1
   - 项目二：(300×2) / 1400 = 比例值2
   - 项目三：(200×3) / 1400 = 比例值3
3. 计算最终收缩大小：
   - 项目一需要收缩：比例值1 × 300
   - 项目二需要收缩：比例值2 × 300
   - 项目三需要收缩：比例值3 × 300



#### flex复合属性

复合了 flex-grow	flex-shrink	flex-basis 三个属性，默认值为 0	1 	auto

```css
/* 可以拉伸 可以压缩 不设置基准长度，可简写为: flex:auto */
/* flex:1 1 auto; */

/* 可以拉伸 可以压缩 设置基准长度为0，可简写为: flex:1 */
/* flex: 1 1 0; */

/* 不可以拉伸 不可以压缩 不设置基准长度，可简写为: flex:none */
/* flex: 0 0 auto; */

/* 不可以拉伸 可以压缩 不设置基准长度，可简写为: flex:0 auto */
/* flex: 0 1 auto; */
```



#### 排序和单独对齐

项目排序

- **order 属性** 定义项目的排列顺序。数值越小，排列越靠前，默认为 `0`。

单独对齐

- 通过 `align-self` 属性，可以单独调整某个伸缩项目的对齐方式。
- 默认值为 `auto`，表示继承父元素的 `align-items` 属性。





### 响应式布局

#### 媒体查询

**@media**

##### 媒体类型

* 只有在打印机或打印预览才应用的样式

```css
@media print {
    h1 {
        background: transparent;
    }
}
```

* 只有在屏幕上才应用的样式

```css
@media screen {
    h1 {
        font-family: "翩翩体-简";
    }
}
```

* 一直都应用的样式

```css
@media all {
    h1 {
        color: red;
    }
}
```

##### 媒体特性

| 值                 | 含义                               |
| ------------------ | ---------------------------------- |
| `width`            | 检测视口宽度。                     |
| `max-width`        | 检测视口最大宽度。                 |
| `min-width`        | 检测视口最小宽度。                 |
| `height`           | 检测视口高度。                     |
| `max-height`       | 检测视口最大高度。                 |
| `min-height`       | 检测视口最小高度。                 |
| `device-width`     | 检测设备屏幕的宽度。               |
| `max-device-width` | 检测设备屏幕的最大宽度。           |
| `min-device-width` | 检测设备屏幕的最小宽度。           |
| `orientation`      | 检测视口的旋转方向（是否横屏）。   |
| portrait           | 视口处于纵向，即高度大于等于宽度。 |
| landscape          | 视口处于横向，即宽度大于高度。     |

- **portrait**：视口处于纵向，即高度大于等于宽度。
- **landscape**：视口处于横向，即宽度大于高度。

------

完整列表请参考：

https://developer.mozilla.org/zh-CN/docs/Web/CSS/@media



##### 运算符

| 值        | 含义                                                         |
| --------- | ------------------------------------------------------------ |
| `and`     | 并且（用于组合多个媒体特性）                                 |
| `, 或 or` | 或（用逗号分隔不同的媒体查询，满足任一条件即应用样式）       |
| `not`     | 否定（取反整个媒体查询的结果）                               |
| `only`    | 肯定（限定仅当条件完全匹配时应用样式，主要用于防止旧版浏览器错误应用样式） |

```css
/* @media (min-width:700px) and (max-width:800px) { ... */

@media screen and (min-width: 700px) and (max-width: 800px) {
    h1 {
        background-color: orange;
    }
}
```



#### 常用阈值

在实际开发中，会将屏幕划分成几个区间，例如：

- **超小屏幕**：宽度小于 768px
- **中等屏幕**：宽度在 768px 到 992px 之间
- **大屏幕**：宽度在 992px 到 1200px 之间
- **超大屏幕**：宽度大于 1200px

------

结合外部样式的用法

用法一：

```html
<link rel="stylesheet" media="具体的媒体查询" href="mystylesheet.css">
```

用法二：

```css
@media screen and (max-width: 768px) {
    /* CSS-Code */
}

@media screen and (min-width: 768px) and (max-width: 1200px) {
    /* CSS-Code */
}
```







### BFC

* 什么是BFC？

1. BFC 是 Block Formatting Context（块级格式化上下文），可以理解成元素的一个“特异功能”。
2. 该“特异功能”，在默认的情况下处于关闭状态；当元素满足了某些条件后，该“特异功能”被激活。
3. 所谓激活“特异功能”，专业点说就是：该元素创建了 BFC（又称：开启了 BFC）。



* BFC有什么用？

1. 元素开启 BFC 后，其**子元素**不会再产生 margin 塌陷问题。
2. 元素开启 BFC 后，自己不会被其他浮动元素所覆盖。
3. 元素开启 BFC 后，就算其子元素浮动，元素自身高度也不会塌陷。



* 如何开启BFC？
  1. 根元素
  2. 浮动元素
  3. 绝对定位、固定定位的元素行内块元素
  4. 表格单元格：`table`、`thead`、`tbody`、`tfoot`、`th`、`td`、`tr`、`caption``
  5. ``overflow` 的值不为 `visible` 的块元素
  6. 伸缩项目
  7. 多列容器
  8. `column-span` 为 `all` 的元素（即使该元素没有包裹在多列容器中）
  9. `display` 的值，设置为 `flow-root`

