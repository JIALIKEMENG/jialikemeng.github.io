Telegraph-Image 图床，是一款开源的图床系统，旨在为博客或网站提供高质量的图片托管服务。通过 Telegraph-Image，您可以轻松地上传、管理和引用图片，同时保证图片的加载速度和稳定性。无需服务器，无限空间，免费使用。

**图床特性：**
1. 无限图片储存数量，你可以上传不限数量的图片。
2. 无需购买服务器，托管于Cloudflare的网络上，当使用量不超过Cloudflare的免费额度时，完全免费。
3. 无需购买域名，可以使用Cloudflare Pages提供的*.pages.dev的免费二级域名，同时也支持绑定自定义域名。
4. 支持图片审查API，可根据需要开启，开启后不良图片将自动屏蔽，不再加载。
5. 支持后台图片管理，可以对上传的图片进行在线预览，添加白名单，黑名单等操作。

**准备工作：**
1. 注册 [Github](https://github.com/) 和 [Cloudflare](https://www.cloudflare.com/) 账户并登录。
2. Fork [Telegraph-Image项目](https://github.com/cf-pages/Telegraph-Image)。

**搭建步骤：**
1. 进入Cloudflare的Workers和Pages页面，（点击创建应用程序），选择Pages，点击连接到git。
2. 选择自己账户下之前 Fork 好的项目，点击开始设置。
3. 部署，制作，选择默认配置部署就可以，等待部署完成，之后CF会自动分配免费域名（[示例](https://telegraph-image-yht.pages.dev/)） 。可以点击域名查看是否可以打开，也可以进行上传测试。
4. 若有自己的域名，你可以在自定义域里设置分配一个二级域名给这个项目。

**后台设置：**
1. 打开 Telegraph-Image 项目，进入设置里的函数选项。
2. 找到KV 命名空间绑定，创建新的命名空间，将空间名称命名为img_url。
3. 返回设置，在KV 命名空间绑定绑定我们刚创建好的空间，然后保存即可。
4. 找到设置→环境变量。新增变量，即后台账号密码。
5. 打开项目部署详细信息，在管理部署那里选择重新部署。
6. 访问项目域名，在域名后加/admin 回车，输入刚配置的账号密码即可进入后台，可以对图片进行管理，可以进行白名单，黑名单和删除操作。

**注意事项**
1. 设置了黑名单的图片无法进行访问。
2. 图片大小限制 5MB。
3. 上传图片之后后台却看不到图片，你需要在上传图片后复制图片URL进行一次访问，即可在后台看到图片信息。    
4. 由于是白嫖CF的资源，所以读取次数有限额，不过个人使用还是足够的。
5. 在Github的 Telegraph-Image项目Sync fork- >Update branch即可更新项目。

参看[项目页](https://github.com/cf-pages/Telegraph-Image)及[介绍页](https://mp.weixin.qq.com/s/gVl1yojC07B81_iQaxxZWw)。