 PicX 是XPoet开发的一款基于 GitHub API 开发的图床工具，可提供图片上传托管、生成图片链接和常用图片工具箱服务。

**PicX 图床特点：**
- 在线使用、无需下载、无需安装。
- 操作简单、文档完善、持续维护。
- 代码开源、数据安全、完全免费。

**PicX 图床创建方法：**

- 注册申请[github](https://github.com/)账户并登录；
- 打开[图床神器](https://picx.xpoet.cn/)，进行登录（先查看登陆教程再操作）；
> 有两种登陆方式：
> GitHub OAuth 授权登录：
> （1）安装 PicX GitHub APP
> 使用 GitHub OAuth 授权登录必须先安装 PicX GitHub APP，否则没有操作权限。点击界面中间的安装 PicX GitHub APP 立即跳转到 安装页面，安装成功后，会自动跳转回 PicX 登录页，并进行是否授权登录的询问。
> （2）进行 GitHub OAuth 授权登录
> PicX GitHub APP 安装成功之后，在消息提示框点击确定或者手动点击 GitHub OAuth 授权登录按钮，进行授权登录。授权登录成功之后，PicX 会自动完成该账号下的图床配置。
> 填写 GitHub Token 登录：
> （1）创建一个带有 repo 权限的 GitHub Token. 点击 [新建GitHub Token](https://github.com/settings/tokens/new) 快速新建 GitHub Token：输入令牌名字，选择无有效期，勾选repo，最后点击 Generate token 按钮，即可生成 GitHub Token。新生成的 Token 只会显示一次，请妥善保存，如有遗失，重新生成即可。
> （2）绑定 GitHub Token. 点击填写 GitHub Token 登录，通过填写 GitHub Token 登录获取到你的 GitHub 账号信息、Public 仓库信息等数据，完成 Token 绑定。
>

- 进行图床配置；
> 有两种配置方法：
> （1）自动配置
> 在登录成功之后，点击界面一键自动配置，自动创建 GitHub 仓库，并完成仓库、分支和目录之间的绑定。首次使用 PicX，强烈推荐使用一键自动配置，极其便捷。
> （2）手动配置
> 需要逐步操作来完成仓库、分支和目录之间的绑定。详细操作参看[使用文档](https://picx-docs.xpoet.cn)中图文说明。
> 
图床配置完成，创建成功之后就可以上传图片了。上传成功，会自动复制图片链接地址，或者手动在左侧窗口图片下方复制。图片保存在github仓库里，可以进行筛选、删除的工作。

**PicX 图床功能：**
- 支持 [拖拽](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E6%8B%96%E6%8B%BD%E5%9B%BE%E7%89%87)、[复制粘贴](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E5%A4%8D%E5%88%B6%E7%B2%98%E8%B4%B4)、[选择文件](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E9%80%89%E6%8B%A9%E6%96%87%E4%BB%B6) 等方式进行选择图片
-  支持上传时对图片 [重命名](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E9%87%8D%E5%91%BD%E5%90%8D)、[哈希化](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E5%93%88%E5%B8%8C%E5%8C%96)（确保图片名唯一）和 [设置命名前缀](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E5%89%8D%E7%BC%80%E5%91%BD%E5%90%8D)
-  支持 批量上传图片、[批量删除图片](https://picx-docs.xpoet.cn/usage-guide/management.html#%E5%88%A0%E9%99%A4-%E6%89%B9%E9%87%8F%E5%88%A0%E9%99%A4) 和 [批量复制图片链接](https://picx-docs.xpoet.cn/docs/usage-guide/management.html#%E6%89%B9%E9%87%8F%E5%A4%8D%E5%88%B6%E5%A4%9A%E5%BC%A0%E5%9B%BE%E7%89%87%E9%93%BE%E6%8E%A5)
-  支持图床 多级目录 管理 （创建多级目录 / 查看多级目录下图片）
-  支持 [一键复制](https://picx-docs.xpoet.cn/docs/usage-guide/upload.html#%E5%A4%8D%E5%88%B6%E5%9B%BE%E7%89%87%E9%93%BE%E6%8E%A5) 图片链接和 [自由转换 Markdown / HTML / BBCode 格式](https://picx-docs.xpoet.cn/docs/usage-guide/settings.html#%E5%9B%BE%E7%89%87%E9%93%BE%E6%8E%A5%E6%A0%BC%E5%BC%8F%E8%AE%BE%E7%BD%AE)
-  内置 [多种图片链接规则](https://picx-docs.xpoet.cn/docs/usage-guide/settings.html#%E5%9B%BE%E7%89%87%E9%93%BE%E6%8E%A5%E8%A7%84%E5%88%99%E9%85%8D%E7%BD%AE)（GitHub、GitHub Pages、jsDelivr、Statically 等）
-  支持 [自定义配置图片链接规则](https://picx-docs.xpoet.cn/docs/usage-guide/settings.html#%E9%85%8D%E7%BD%AE%E8%87%AA%E5%AE%9A%E4%B9%89%E5%9B%BE%E7%89%87%E9%93%BE%E6%8E%A5%E8%A7%84%E5%88%99)
-  支持 [图片压缩](https://picx-docs.xpoet.cn/docs/usage-guide/settings.html#%E5%9B%BE%E7%89%87%E5%8E%8B%E7%BC%A9%E8%AE%BE%E7%BD%AE) (内置高效压缩算法，可配置在上传前自动压缩)
-  支持配置 [图片水印](https://picx-docs.xpoet.cn/docs/usage-guide/settings.html#%E5%9B%BE%E7%89%87%E6%B0%B4%E5%8D%B0%E8%AE%BE%E7%BD%AE)
-  支持 PWA
-  支持 [暗夜模式](https://picx-docs.xpoet.cn/docs/usage-guide/settings.html#%E4%B8%BB%E9%A2%98%E8%AE%BE%E7%BD%AE) (自动切换 / 自由切换)
-  i18n（中文简体、中文繁体、英文）
-  工具箱（[图片压缩](https://picx-docs.xpoet.cn/docs/usage-guide/toolbox.html#%E5%9B%BE%E7%89%87%E5%8E%8B%E7%BC%A9)、[图片转 Base64](https://picx-docs.xpoet.cn/docs/usage-guide/toolbox.html#%E5%9B%BE%E7%89%87%E8%BD%AC-base64)、[图片水印](https://picx-docs.xpoet.cn/docs/usage-guide/toolbox.html#%E5%9B%BE%E7%89%87%E6%B0%B4%E5%8D%B0)）

关于PicX 图床的详细部署及使用说明请查看[仓库](https://github.com/XPoet/picx)和[使用文档](https://picx-docs.xpoet.cn)。