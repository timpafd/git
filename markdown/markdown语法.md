# markdown语法
1. 字体、字号、颜色

<font face="黑体"color=#A52A2A  size=7>我是黑体</font>  
<table><tr><td bgcolor= BlueViolet > 背景色2 BlueViolet </td></tr></table>  
`<font face="黑体"color=#A52A2A  size=7>我是黑体</font>`  
`<table><tr><td bgcolor= BlueViolet > 背景色2 BlueViolet </td></tr></table>`  

 > Size：规定文本的尺寸大小。可能的值：从 1 到 7 的数字。浏览器默认值是 3。

2. 列表

    > 在文字前加上*、+或- 即可变为无序列表，有序列表则直接在文字前加1. 2. 3. 符号要和文字之间加上一个字符的空格。

3. 标题

    > 在这段文字前加 # 号即可,'''# 一级标题 ## 二级标题 ### 三级标题 '''总共六级标题，建议在井号后加一个空格

4. 引用

    > 只需要在文本前加入 > 这种尖括号（大于号）即可,尖括号与文字中间需有空格

5. 图片与链接表示

    > 图片为：`![]()`

    > 链接为：`[]()`

    > 链接：[baidu](https://www.baidu.com)

    > 图片：![描述文字](https://img03.sogoucdn.com/app/a/100520093/b692ca88cf40622d-c4c351c548f54192-bb3dcf0e0a9e96d7137a472afa9b9192.jpg)

6. 粗体与斜体

    > 用两个 *或_ 包含一段文本就是粗体的语法，用一个 *或_ 包含一段文本就是斜体的语法

7. 表格

|   tables      |   tables      |   tables      |
|----------    |   :-------:    |   --------:   |
|   col 3        | right-alig   |   $160         |  

```

|   tables      |   tables      |   tables      |
|----------    |   :-------:    |   --------:   |
|   col 3        | right-alig   |   $160         |
```

<font color=#A52A2A  >上下文之间要留空行</font>  
语法说明：  

* `|`、`-`、`:`之间的多余空格会被忽略，不影响布局。  
* 默认标题栏居中对齐，内容居左对齐。  
* `-:`表示内容和标题栏居右对齐，`:-`表示内容和标题栏居左对齐，`:-:`表示内容和标题栏居中对齐。  
* 内容和`|`之间的多余空格会被忽略，每行第一个|和最后一个|可以省略，`-`的数量至少有一个


8.代码框
> 只需要用两个 ` 把中间的代码包裹起来,使用 tab 键即可缩进。  
> 将\```放于代码段的首行和末行

\```  
|   tables      |   tables      |   tables      |  
|----------    |   :-------:    |   --------:   |  
|   col 3        | right-alig   |   $160         |  
\```

9. 分割线
***

> 分割线的语法只需要三个 * 号

> <u>下划线</u>使用`<u></u>`标签实现 <font color=#A52A2A  >如果文本不是超链接，就不要对其使用下划线</font>