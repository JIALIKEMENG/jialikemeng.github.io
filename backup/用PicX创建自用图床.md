 PicX 是XPoet开发的一款基于 GitHub API 开发的图床工具，可提供图片上传托管、生成图片链接和常用图片工具箱服务。

**PicX 图床特点：**
- 在线使用、无需下载、无需安装。
- 操作简单、文档完善、持续维护。
- 代码开源、数据安全、完全免费。

**PicX 图床创建方法：**

- 注册申请[github](https://github.com/)账户并登录；
- 打开[图床神器](https://picx.xpoet.cn/)，进行登录（先查看登陆教程再操作）；
> 有两种登陆方式：
> 1. GitHub OAuth 授权登录：
> （1）安装 PicX GitHub APP
> 使用 GitHub OAuth 授权登录必须先安装 PicX GitHub APP，否则没有操作权限。点击界面中间的安装 PicX GitHub APP 立即跳转到 安装页面，安装成功后，会自动跳转回 PicX 登录页，并进行是否授权登录的询问。
> （2）进行 GitHub OAuth 授权登录
> PicX GitHub APP 安装成功之后，在消息提示框点击确定或者手动点击 GitHub OAuth 授权登录按钮，进行授权登录。授权登录成功之后，PicX 会自动完成该账号下的图床配置。
>2.  填写 GitHub Token 登录：
> （1）创建一个带有 repo 权限的 GitHub Token. 点击 [新建GitHub Token](https://github.com/settings/tokens/new) 快速新建 GitHub Token：输入令牌名字，选择无有效期，勾选repo，最后点击 Generate token 按钮，即可生成 GitHub Token。新生成的 Token 只会显示一次，请妥善保存，如有遗失，重新生成即可。
> （2）绑定 GitHub Token. 点击填写 GitHub Token 登录，通过填写 GitHub Token 登录获取到你的 GitHub 账号信息、Public 仓库信息等数据，完成 Token 绑定。
>

- 进行图床配置；
> 有两种配置方法：
> 1. 自动配置
> 在登录成功之后，点击界面一键自动配置，自动创建 GitHub 仓库，并完成仓库、分支和目录之间的绑定。首次使用 PicX，强烈推荐使用一键自动配置，极其便捷。
> 2. 手动配置
> 需要逐步操作来完成仓库、分支和目录之间的绑定。详细操作参看[使用文档](https://picx-docs.xpoet.cn)中图文说明。
> 
图床配置完成，创建成功之后就可以上传图片了。上传成功，会自动复制图片链接地址，或者手动在左侧窗口图片下方复制。图片保存在github仓库里，可以进行筛选、删除的工作。

示例图片（JsDelivn）：![605](https://cdn.jsdelivr.net/gh/JIALIKEMENG/picx-images-hosting@master/605.6giqjek9afo0.webp)

关于PicX 图床的详细部署及使用说明请查看[仓库](https://github.com/XPoet/picx)和[使用文档](https://picx-docs.xpoet.cn)。