**（一）图床项目**
1. [Cloudflare Image Hosting](https://github.com/ifyour/cf-image-hosting)，官方演示站点[示例](https://images.mingming.dev/)。
一个利用CF实现的免费图床。 免费无限制上传、支持拖放上传、支持复制粘贴上传、支持图片&视频&GIF上传，最大支持的上传文件大小为5MB。  
2. [Telegraph-Image](https://github.com/cf-pages/Telegraph-Image)，官方演示站点[示例](https://im.gurl.eu.org/)。免费图片托管解决方案，Flickr/imgur 替代品。使用 Cloudflare Pages 和 Telegraph。大家使用最多的一个，可以设置图片审查及后台管理。已搭建，参看[搭建TG-Image免费图床](https://jialikemeng.github.io/post/da-jian-TG-Image-mian-fei-tu-chuang.html)。
3. [骤雨重山图床](https://github.com/uxiaohan/ZYCS-IMG)，官方演示站点[示例](https://wp-cdn.4ce.cn/)。用Cloudflare Pages部署稳定的无限量图片托管平台Telegraph，实现图片上传和访问，并通过WordPress的WP.COM全局图片缓存进一步加速，提高图片加载速度。可用于免费图片托管解决方案，替代方案如Flickr/imgur。已搭建，参看[骤雨重山图床的Fock和部署](https://jialikemeng.github.io/post/zou-yu-zhong-shan-tu-chuang-de-Fock-he-bu-shu.html)。
4. [img-mom](https://github.com/beilunyang/img-mom)，基于Cloudflare Workers构建的Telegram机器人的服务端，未测试。
5. [workers-image-hosting](https://github.com/iiop123/workers-image-hosting)，基于cloudflare workers数据存储于KV的简易图床项目。
**（二）图片处理**
1. [Cloudflare Worker Image](https://github.com/ccbikai/cloudflare-worker-image)，支持PNG,JPG,BMP,TIFF等格式图片处理，支持管道操作，可以执行多个操作。且默认输出WEBP格式的图片。
**（三）邮箱项目**
1. [vmail](https://github.com/oiov/vmail) 只需一个域名就可以部署的临时邮箱系统，特点是支持多域名后缀，找回密码。官方演示[示例](https://vmail.dev/)。
2. [cloudflare_temp_email](https://github.com/dreamhunter2333/cloudflare_temp_email) ，官方演示[示例](https://mail.awsl.uk/)。支持的功能有：多语言、自定义名字邮箱、支持增加访问密码、支持自动回复。支持发送邮件，支持SMTP发送邮件和IMAP查看邮件。支持完整的用户注册和登录功能。
3. [mail2telegram](https://github.com/TBXark/mail2telegram/blob/master/doc/README_CN.md)，这是一个基于 Cloudflare Email Routing Worker的 Telegram Bot，能够将邮件转换成telegram消息。你可以将任意前缀的收件人的邮件转发到Bot，然后一个无限地址的临时邮箱Bot就诞生了。也是用worker部署的。