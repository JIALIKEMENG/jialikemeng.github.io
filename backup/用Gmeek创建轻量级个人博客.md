[Gmeek](https://github.com/Meekdai/Gmeek)是Meekdai在github上开源的一个博客框架项目，完全基于 Github Pages、Github Issues 和 Github Actions。不需要本地部署，可以快速创建轻量级个人博客。

Gmeek 特性：
> - UI 界面和 Github 同源，只引入了 Github 原生 CSS：primer.style；
> - 博客写作在 Issues 中完成后，自动触发 Actions 执行部署任务；
> - 评论系统引入 utteranc.es；
> - 使用 jinja2 对 html 进行渲染，可通过模板自定义 UI 主题。

创建方法：
> - **注册**申请github账户并**登录**；
> - 点击[通过Gmeek模板创建仓库](https://github.com/new?template_name=Gmeek-template&template_owner=Meekdai)，仓库名称命名为“github用户名.github.io"（测试不可自定义），点击**新建仓库**；
> - 在你创建好的仓库页面，点击设置，**修改**pages—Build and deployment**来源**为Github Actions；
> - 点击代码，按需**修改**config.json**配置文件**，**保存**修改。config.json配置文件可参考[这里](https://github.com/Meekdai/meekdai.github.io/blob/main/config.json)；
> - 修改配置文件后，点击操作，选择build Gmeek，运行工作流程进行**全局生成**：
> - 如果全局生成成功，就可以点击议题，点击**创建议题**，来直接写博客了。写完后别忘了**加一个标签**（可自定义）。

至此，你的博客已经顺利创建并有了一篇博客文字。可以直接通过创建仓库时的仓库名”github用户名.github.io“来访问了。

示例：[https://jialikemeng.github.io/](https://jialikemeng.github.io/)

详细创建方法及存在问题处理参看：[Gmeek快速上手
](https://blog.meekdai.com/post/Gmeek-kuai-su-shang-shou.html)
