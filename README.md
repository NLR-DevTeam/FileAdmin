# FileAdmin
由盐鸡开发的一款轻量级文件管理器

## 兼容性
- 服务端：完美兼容PHP 7.x，理论上8.x也可以运行。
- 浏览器：仅兼容Google Chrome / Microsoft Edge的最新版本。

## 安装
- 从Github存储库直接下载fileadmin.php。
- 到你的主机直接上传刚才下载的fileadmin.php。
- 如果认为原文件名不安全，您可以对此文件进行重命名。尽量将其安装在您的网站根目录。
- **[重要]打开此文件，在第一行修改$PASSWORD变量，输入您自己设定的密码。不更改此处设置会导致他人可以随意查看并修改您的文件，非常危险。**

## 使用
FileAdmin为用户定义了多种方便使用的快捷键。

|快捷键|对应页面|功能|
|--|--|--|
|/|密码输入页面|聚焦密码输入框|
|/|文件管理页|编辑文件路径|
|Ctrl+A|文件管理页|选中所有文件|
|Ctrl+C|文件管理页|复制选中文件|
|Ctrl+X|文件管理页|剪切选中文件|
|Ctrl+V|文件管理页|粘贴先前复制/剪切的文件|
|Delete|文件管理页|删除选中的文件|
|ESC|文件管理页|返回上级目录|
|Ctrl+S|文本编辑器|保存文件|
|Ctrl+Z|文本编辑器|撤销上一步操作|
|Ctrl+Y|文本编辑器|恢复被撤销的更改|
|Ctrl+F|文本编辑器|查找或替换内容|
|ESC|文本编辑器|退出文本编辑器|

FileAdmin内置了从本仓库获取源码并自动更新本体程序的功能，在任意界面点击左上方的“FileAdmin”字样即可检查更新。部分大陆地区的主机/服务器可能不支持此功能。

## Demo
地址：https://fileadmin-demo.simsoft.top/fileadmin.php

密码：SimSoft

Demo已禁用保存文件等功能，非程序Bug

## 感谢
- [星辰云](https://starxn.com)提供开发环境支持
- [XIAYM](https://github.com/XIAYM-gh)提供开发环境支持
- [AdminX](https://github.com/1689295608/AdminX)提供部分函数实现
