[骤雨重山图床](https://github.com/uxiaohan/ZYCS-IMG)是利用Cloudflare Pages部署的稳定的无限Telegraph图床【[示例]】(https://37img.pages.dev/)，实现图片上传和访问，并进一步通过WordPress的WP.COM全球图片缓存进行加速，提高图片加载速度。可用于免费图片托管解决方案，是Flickr/imgur 等替代品。

**简介**
- [Cloudflare Pages](https://pages.cloudflare.com/) 是一个强大的静态网站托管服务，结合了 Cloudflare 的全球 CDN（内容分发网络）优势。
- [Telegraph](https://telegra.ph/) 是一个简单而有效的匿名发布平台，可以用于快速上传和管理内容，特别是图片。
- [WordPress 的全球图片缓存](https://01.wp.com/) 是一个高效的 CDN 服务，专门用于加速 WordPress 托管的图片内容。它利用全球分布的节点，将图片缓存并提供快速访问。
- [Cloudflare CDN（内容分发网络）](https://www.cloudflare.com/zh-cn/application-services/products/cdn/)是由Cloudflare提供的服务，旨在加速和保护和加速全球网络应用程序。

**部署**
- 准备一个 Cloudflare 账户
- Fork 本仓库，自由修改App.vue和index.html文件中的文案
- 登录Cloudflare Dashboard打开Workers 和 Pages创建Pages
- 连接到Git选择Github或Gitlab中你刚刚Fork的项目，点击开始设置
- 只需要修改框架预设为Vue即可，点击保存并部署，即可部署成功并投入使用

特点
- 无限图片储存数量，你可以上传不限数量的图片到Telegraph
- 无需购买服务器，托管于Cloudflare Pages上，每天10万次的请求
- 无需购买域名，可以使用Cloudflare Pages 提供的*.pages.dev的免费二级域名，同时也支持绑定自定义域名
- 目前似乎无后台管理功能

具体参看[中文说明](https://github.com/uxiaohan/ZYCS-IMG/blob/main/README_CN.md)。