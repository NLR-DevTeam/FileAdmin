# FileAdmin
一款体验极佳的轻量级PHP文件管理器

项目的前身是[SimAdmin](https://github.com/YanJi314/SimAdmin)，但本身并不使用其任何代码

如果这个项目有帮助到你，点个 Star 再走呗

## 兼容性
- 服务端：完美兼容PHP 7.x - 8.x。
- 浏览器：仅兼容Google Chrome / Microsoft Edge的最新版本。

实测兼容多数宝塔分销虚拟主机及Kangle虚拟主机，部分没有真实文件系统的特殊环境可能无法运行。

## 安装
- 从[氢软API](https://api.simsoft.top/fileadmin/download/)直接下载FileAdmin安装版。**您也可以下载安装版之外的其他版本，详见本文“版本”章节**
- 到你的主机直接上传刚才下载的fileadmin.php。
- 如果认为原文件名不安全，您可以对此文件进行重命名。尽量将其安装在您的网站根目录。
- **[重要]打开此文件，在第一行修改$PASSWORD变量，输入您自己设定的密码。不更改此处设置会导致他人可以随意查看并修改您的文件，非常危险。**

## 使用
- FileAdmin为用户定义了多种方便使用的快捷键。

|快捷键|对应页面|功能|
|--|--|--|
|/|密码输入页面|聚焦密码输入框|
|/|文件管理页|编辑文件路径|
|Ctrl+A|文件管理页|选中所有文件|
|Ctrl+C|文件管理页|复制选中文件|
|Ctrl+X|文件管理页|剪切选中文件|
|Ctrl+V|文件管理页|当面板剪切板中存在文件（即菜单中显示“粘贴”按钮时）粘贴先前在面板中复制/剪切的文件；当面板剪切板中无项目时，自动从系统剪切板中获取文件（如有）并上传|
|Delete|文件管理页|删除选中的文件|
|F5|文件管理页|刷新文件列表|
|ESC|文件管理页|返回上级目录|
|Ctrl+S|文本编辑器|保存文件|
|Ctrl+Z|文本编辑器|撤销上一步操作|
|Ctrl+Y|文本编辑器|恢复被撤销的更改|
|Ctrl+F|文本编辑器|查找或替换内容|
|F5|文本编辑器|刷新文本编辑器|
|ESC|文本编辑器|退出文本编辑器|

- FileAdmin也自带了一些有助于提升效率的鼠标快捷操作

|鼠标操作|功能|
|--|--|
|单击文件|未进入选中模式时，打开此文件；进入选中模式时，选中/取消选中此文件|
|右键文件|未进入选中模式时，选中此文件并进入选中模式|
|在文件列表按下鼠标并滑动|多选或取消选中鼠标滑过的文件|
|在空白区域单击鼠标|取消选中所有文件|

- FileAdmin内置了从本仓库获取源码并自动更新本体程序的功能，在任意界面点击左上方的“FileAdmin”字样即可检查更新。部分大陆地区的主机/服务器可能不支持此功能。

## Js混淆
FileAdmin内置了强大的Js混淆器（Javascript Obfuscator），使开发者方便保护自己开发的源代码。开启此功能前请仔细阅读下方说明：
- Js混淆会使您的Js文件存储占用成倍上涨，且可能导致文件保存缓慢
- Js混淆可能会导致部分代码无法运行，请务必自行进行充分测试
- 您可能难以调试混淆后的Js代码
- FA并不具备解除混淆的能力，所以Js混淆开启后，会在当前目录生成一个.fajs文件用于存储Js源文件
- 请务必使用防火墙屏蔽他人对.fajs文件的访问
- 请勿直接修改、移动或删除.fajs文件，否则会导致您无法编辑Js源码

附常用防火墙配置方式：
- 宝塔免费防火墙URL过滤规则：`\.(fajs)`
- Cloudflare防火墙阻止规则：`(http.request.full_uri contains ".fajs")`

其余防火墙配置同理

## 官网
- 官网：https://fa.yanji.pro/
- 演示：http://demo.fa.yanji.pro/
- 介绍：https://www.bilibili.com/video/BV1XZ4y1m7WK
- 捐赠：https://yanji.pro/#donate

## 版本(即将上线)

FileAdmin 目前共有三个版本开放安装。
- 安装版：旨在使您获得最小化的代码体积。[ [https://api.simsoft.top/fileadmin/download/](点击下载) ]
- 维护版：从Github直接获取源码，包含完整的注释和缩进。[ [https://api.simsoft.top/fileadmin/download/maintain.php](点击下载) ]
- 安装版：氢软官方的实时开发版，可获知最新的开发进度。[ [https://api.simsoft.top/fileadmin/download/dev.php](点击下载) ]

Tip：无论选择哪个版本，内嵌的自动更新皆以安装版发版为准，且会使用安装版更新覆盖其他版本。如需长期使用非安装版的版本，请直接从上方渠道手动更新而非使用自动更新。

## 版权&免责
- 本程序使用AGPL-3.0协议开源，任何二开作品需以相同协议开源，不推荐用于商业用途。
- 本程序若因使用不当造成的任何损失，开发者不负任何责任。

## 感谢
- [星辰云](https://starxn.com)提供开发环境支持
- [XIAYM](https://github.com/XIAYM-gh)提供开发环境支持
- [AdminX](https://github.com/1689295608/AdminX)提供部分函数实现
- [Javascript Obfuscator](https://obfuscator.io)提供Js混淆技术支持
