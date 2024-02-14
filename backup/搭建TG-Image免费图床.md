Telegraph-Image 图床，是一款开源的图床系统，旨在为博客或网站提供高质量的图片托管服务。通过 Telegraph-Image，您可以轻松地上传、管理和引用图片，同时保证图片的加载速度和稳定性。无需服务器，无限空间，免费使用。

**图床特性：**
- 无限图片储存数量，你可以上传不限数量的图片。
- 无需购买服务器，托管于Cloudflare的网络上，当使用量不超过Cloudflare的免费额度时，完全免费。
- 无需购买域名，可以使用Cloudflare Pages提供的*.pages.dev的免费二级域名，同时也支持绑定自定义域名。
- 支持图片审查API，可根据需要开启，开启后不良图片将自动屏蔽，不再加载。
- 支持后台图片管理，可以对上传的图片进行在线预览，添加白名单，黑名单等操作。

**准备工作：**
- 注册 [Github](https://github.com/) 和 [Cloudflare](https://www.cloudflare.com/) 账户并登录。
- 最好拥有1个域名并托管在Cloudflare中。

**搭建步骤：**
1. Fork项目。
> 在 [Telegraph-Image项目](https://github.com/cf-pages/Telegraph-Image)主页点击Fork按钮，页面中什么都不要改，直接点击Create fork按钮，等待片刻就创建完成。
2. 连接到Github。
> 进入Cloudflare，点击左侧Workers和Pages->概述菜单，【点击创建应用程序】，切换到Pages界面，点击连接到git。
> 在弹出界面中选择Github，并点击连接Github按钮，之后，Cloudflare会自动引导你到Github授权页面（如果没有登录Github，则会先到登录界面）。
> 接着，选择Only Select repositories，并选择上面fork好的项目，然后点击Install & Authorize按钮，确认完成授权和开始安装。
> 最后，Github可能会要求你输入账号密码，以确认上面的授权。输入你的Github密码并Confirm。
3. 部署图床。
> 确认授权后，会从Github自动跳回到Cloudflare中，继续开始后续的部署设置。
> 首先，选中上面授权好的Github项目，点击开始设置。
> 项目名称可以自定义，生产分支建议保持默认的main，其他默认。
> 拉到页面下面，点击保存并部署，等待Pages自动部署项目完成。
> 当看到成功提示时，表示图床已经部署完成了。此时CF会自动分配一个默认的免费域名【[示例](https://telegraph-image-yht.pages.dev/)】 。
> 点击域名查看是否可以打开，也可以进行上传测试。
4. 自定义域名。
> 进入项目页面，切换到自定义域页面。
> 点击设置自定义域，输入你自己想用的二级域名，并点击继续按钮。
> Cloudflare将自动在域名DNS中添加一个CNAME解析记录，将自定义域名指向默认分配的域名。直接点击激活域按钮，然后等待验证即可。
> 自定义域验证完成后，系统自动配置好了SSL证书。此时就可以使用新的域名访问图床系统了。

**后台设置：**
1. 配置管理后台。
> 打开Workers和Pages->KV管理，点击右上角创建命名空间按钮，创建一个名为img_url的命名空间。
> 打开 Telegraph-Image 项目，进入设置里的函数选项。拉到页面的下面，找到KV命名空间绑定模块。点击添加绑定按钮，将变量名称和KV命名空间均设置为img_url，然后保存。
> 切换到环境变量页面，点击制作中的添加变量按钮，添加两个环境变量。变量名分别是BASIC_USER和BASIC_PASS，分别代表管理员的用户名和密码，然后保存。【当然，你也可以不设置这两个变量，这时候管理后台就是无需验证即可登录。但是你可以结合Cloudflare Access服务实现支持邮件验证码、Microsoft、Github等第三方帐号登录方式，更加灵活强大。如果使用Cloudflare Access，则需要对/admin和/api/manage/*两个路径进行保护。】
> 打开项目部署详细信息，在管理部署那里选择重新部署点击，等待重新部署完成即可。
> 访问项目域名，在域名后加/admin 回车，输入刚配置的账号密码即可进入后台，可以对图片进行管理，可以进行白名单，黑名单和删除操作。
> 后台图片状态信息字段含义：
- [ ] ListType表示图片当前是否在黑白名单当中。
- [ ] None则表示既不在黑名单中也不在白名单中。
- [ ] White表示在在白名单中。
- [ ] Block表示在黑名单中。
- [ ] TimeStamp图片首次加载的时间戳。
- [ ] Label图片审查的结果。
2. 开启内容审查。
> 打开[ModerateContent](moderatecontent)网站，点击SIGN UP，输入邮箱，点击SUBMIT，界面上就直接为你生成API Key，复制并保存下来。
> 在项目的设置->环境界面中，添加一个环境变量，名称为：ModerateContentApiKey，值就是上面获得的API Key。
> 重新部署系统。
3. 更新图床系统。
如果Telegraph-Image项目更新了，需要添加新的KV命名空间或环境变量，则先在Cloudflare的项目中配置好。
回到Github中，在Telegraph-Image项目页面上点击Sync fork->Update branch即可。

**注意事项**  
1. 每天最多100,000次免费读取操作，图片每加载一次都会占用该额度。建议在Cloudflare上开启域名缓存设置，这样仅当缓存未命中时才会占用该额度。如果额度用完了，则黑白名单等功能可能会失效。
2. 每天最多1,000次免费删除操作，每有一条图片记录都会占用该额度，超过了将无法删除图片记录。
3. 每天最多1,000次免费列出操作，每打开或刷新一次后台/admin都会占用该额度，超过了将无法进行后台图片管理。
4. 设置了黑名单的图片无法进行访问。
5. 启图片审查后，不良图片会被自动屏蔽，不支持加载。
6. 上传的单个文件最大支持5MB。
7. 上传图片之后后台却看不到图片，你需要在上传图片后复制图片URL进行一次访问，即可在后台看到图片信息。 
8.  每次修改部署项目的KV、环境变量等，记得要重新部署，否则不会生效。

参看[项目页](https://github.com/cf-pages/Telegraph-Image)及[介绍页1](https://mp.weixin.qq.com/s/gVl1yojC07B81_iQaxxZWw)和[介绍页2](https://[mp.weixin.qq.com/s/hbpCxE3dYZY1sgt2H3JffA](https://mp.weixin.qq.com/s/hbpCxE3dYZY1sgt2H3JffA))。