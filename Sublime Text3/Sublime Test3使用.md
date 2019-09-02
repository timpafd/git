[TOC]

---  
**[Sublime Text3下载地址](https://www.sublimetext.com/3)**  

---  
# 注册码  
```
 —– BEGIN LICENSE —–
eldon
Single User License
EA7E-1122628
C0360740 20724B8A 30420C09 6D7E046F
3F5D5FBB 17EF95DA 2BA7BB27 CCB14947
27A316BE 8BCF4BC0 252FB8FF FD97DF71
B11A1DA9 F7119CA0 31984BB9 7D71700C
2C728BF8 B952E5F5 B941FF64 6D7979DA
B8EB32F8 8D415F8E F16FE657 A35381CC
290E2905 96E81236 63D2B06D E5F01A69
84174B79 7C467714 641A9013 94CA7162
```  
# 安装package control  
[Sublime Text3官网](https://packagecontrol.io/installation)  
[Sublime Text3中文官网](http://packagecontrol.cn/installation)  
## 方法一  
从**菜单 View - Show Console** 或者 `ctrl + ~ `快捷键，调出 console。将以下 Python 代码粘贴进去并 enter 执行，不出意外即完成安装。  
```
import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```  
## 方法二  
下载`Package Control.sublime-package`(https://packagecontrol.io/Package%20Control.sublime-package).  
将下载好的文件放入到`Installed Packages`目录下(详见手动安装)  
重启软件  
# 安装包  
## 自动安装
按`Ctrl+Shift+P`或点击Preferences/Package Control，然后输入`Install Package`(或是`Package Control：Install Package`),（第一次运行可以要几秒钟，因为要下载Package Control里面存在的包"花名册"），然后在弹出的命令界面，可在此界面输入插件名，进行选择，完成选择后按`Enter`开始安装  
## 手动安装  
由于某种原因导致自动安装失败可使用手动安装  
1. 点击sublime Text3菜单`Preferences > Browse Packages…`(或首选项>浏览插件目录)，会打开路径为`C:\Users\Administrator\AppData\Roaming\Sublime Text 3\Packages`的目录。  
2. 返回上一级目录，进入`Installed Packages`,即当前路径为`C:\Users\Administrator\AppData\Roaming\Sublime Text 3\Installed Packages`。  
3. 将下载好的文件放到`Installed Packages`目录下。  
4. 重启软件。  

## 汉化包  
1. 按`Ctrl+Shift+P`或点击Preferences/Package Control，然后输入`Install Package`(或是`Package Control：Install Package`),（第一次运行可以要几秒钟，因为要下载Package Control里面存在的包"花名册"），然后在弹出的命令界面，输入`Chinese`，选择`ChineseLocalizatio`(回车或者鼠标单击击)。  
2. 切换语言，帮助(H)/Language/简体中文，繁体中文，日本语，English。  

# 快捷键  
| Win快捷键 |作用 | 备注 |
|:-------------|:-------------|:-----|
|html:5+tab|html结构代码||
|tab|补全标签代码|比如，在html文件中输入`div`，然后	按住tab键后，会自动生成`<div></div>`。|
|  **Ctrl + Shift + D** |复制当前行到下一行  |   |
|  Ctrl+Shift+K |  快速删除整行 |   |
|Ctrl+鼠标左键单击|集体输入||
|Ctrl+H|查找替换|||
| Ctrl+/  |  注释单行 |   |
| Ctrl+Shift+/  | 注释多行  |   |
|Ctrl+L|  快速选中整行，继续操作则继续选择下一行，效果和 `Shift + ↓` 效果一样| |
|**Ctrl+Shift+L**|  先选中多行，再按下快捷键，<br/>会在每行行尾插入光标，即可同时编辑这些行| 经常与上一个快捷键结合起来使用 |
|**Ctrl + Shift +【↑/↓**| 移动当前行 | |
|F11|全屏||


[更多快捷键](SublimeText快捷键.html)
# 相关插件推荐  
## Markdown插件  
### 1. 需安装的插件
* Markdown Editting  
主要用来做 Markdown 编辑时的语法高亮，视觉效果更好  
* Markdown Preview  
用来在浏览器中预览效果  
* LiveReload  
热加载  
---  
使用 Package Control安装  

### 2. 部分插件配置  
1. 将 `Markdown Preview` 的 `enable_autoreload `设置为 `true`  
打开 `Preferences – Package Settings – Markdown Preview – Setting`，在 `user` 设置中添加：  
```
{
    "enable_autoreload": true,
}
```
2. 启用 LiveReload  
打开 `ctrl + shift + p`，输入 `LiveReload: Enable/disable plug-ins`，选择 `Enable: Simple Reload`。  
3. 设置预览快捷键  
选择 `Preferences — Key Bindings-User`，将下面的内容添加进去：  
```
{ "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"} }
```  

## 前端插件  
其他插件查看[一个前端程序猿的Sublime Text3的自我修养](https://blog.guowenfh.com/2015/12/26/SublimeText/)  
### FileHeader  
自动创建文件开头模板，并且会根据最后的保存时间修改更新时间。
### CSS Format  
css格式化。
### Emmet  
它能够让你在编辑器中书写CSS和HTML的缩写并且动态地拓展它，是一个能大幅度提高前端开发效率的一个工具。  
这个软件的安装过程比较久,可能会出现[PyV8](https://raw.githubusercontent.com/emmetio/pyv8-binaries/master/pyv8-win64-p3.zip)安装出错,使用手动安装方式安装  

---  
[Emmet语法](https://docs.emmet.io/cheat-sheet/)  

---  
使用：  
新建文件，输入html:5，按[Ctrl + E] 或者 Tab 键  
### JsFormat  
JS代码格式化  
快捷键是：选中JS代码，然后按`ctrl+alt+f`。  
或者，先用快捷键打开命令面板 `ctrl + shift + p`, 再输入 `Format: Javascript` 就可以使用格式化命令  
### HTML-CSS-JS Prettify  
编辑HTML, CSS, JS时，经常会出现缩进不对，代码行不对其的情况。装了这个插件之后，只要按下 Ctrl+Shift+h (Windows), Command+Shift+h (Mac), 你的文档就会被整理干净。  
注: 需要配置node文件路径 HTML-CSS-JS Prettify > plugin Options  
### javascript complet：JavaScript代码自动提示  
### Sublime Server  
我们如果右键在浏览器中打开html网页，其实是以文件路径的方式打开的，导致很多api无法操作。最好的办法是：将html在服务器上打开。  
  
我们如果安装 Sublime Server，就可以让网页在本地的服务器上打开。  
  
安装成功之后，使用步骤如下：  
  
（1）选择菜单栏"Tools --> SublimeServer --> Start SublimeServer"启动服务器。  
  
（2）在html文档里，右键选择 "View in SublimeServer"。  
  
如果想关闭服务器，直接把Sublime Text 整个软件关掉就好。其他的关闭方式容易导致软件卡死。  
