[PicGo](https://github.com/Molunerfinn/PicGo)是一个用于快速上传图片并获取图片 URL 链接的工具。支持七牛图床 /腾讯云/又拍云/GitHub/SM.MS/阿里云/Imgur图床的上传。

PicGo详细使用教程请看[使用文档](https://picgo.github.io/PicGo-Doc/)。

**使用GitHub图床的方法：**
1. 下载[PicGo](https://github.com/Molunerfinn/PicGo/releases)并安装。
2. 登录GitHub新建一个仓库，记住仓库名。
3. 生成一个token。
> 访问[这里](https://github.com/settings/tokens)；
> 点击Generate new token，note随便取名，选择有效期；
> 把repo的勾打上，翻到页面最底部，点击Generate token的绿色按钮生成token；
> 复制生成的token（只出现一次）。
4. 配置PicGo：仓库名的格式是用户名/仓库名（仓库名为步骤2的仓库名）, 一般选择main分支，然后粘贴token。最后点击确定以生效。

[测试图片【国区应该不显示】](https://raw.githubusercontent.com/JIALIKEMENG/picgo/master/Gallery-Simplicity-05.jpg)

[PicList](https://github.com/Kuingsmile/PicList) 可以看作是PicGo的增强版，保留了 PicGo 的所有功能，添加了许多新功能：相册现在支持同步删除云中的文件。内置映像托管选项已扩展为包括 WebDav、本地映像托管和 SFTP。此外，PicList 还引入了全面的云存储管理功能，包括云目录查看、文件搜索、批量上传、下载和文件删除、复制各种格式的链接以及图像、Markdown、文本和视频的预览。此外，它还拥有更强大的相册功能以及许多其他改进和增强功能。

使用方法基本和PicGo相同。