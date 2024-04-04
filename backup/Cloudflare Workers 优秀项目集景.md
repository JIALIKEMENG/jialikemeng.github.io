### 节点：
 [3K 大佬改写的项目](https://github.com/3Kmfi6HP/EDtunnel)
 [Zizifn 大佬原创项目](https://github.com/zizifn/edgetunnel/blob/main/src/worker-vless.js)
 [部署自定义订阅服务](https://github.com/mjjonone/sub-worker/blob/main/_worker.js)

### 建站：
**通过 Workers 搭建博客**
方案一：利用 worker 的 KV 作为数据库搭建博客：[源码](https://github.com/gdtool/cloudflare-workers-blog)，[安装教程](https://cfblog.661212.xyz/article/000003/cfblog-plus.html)
方案二：利用 workers+github 搭建博客系统:[源码](https://github.com/kasuganosoras/cloudflare-worker-blog)

**通过 Workers 搭建导航站：**
利用 worker 搭建导航站：[源码](https://github.com/sleepwood/CF-Worker-Dir)

**利用 Workers 搭建图床：**
[源码](https://github.com/iiop123/workers-image-hosting)
[示例](https://img.231516.xyz/ ) 

**通过 Workers 搭建短网址服务：**
[源码 1 ](https://github.com/igengdu/short/)（推荐，[示例](https://d.igdu.xyz/ )免费短网址服务即是基于此开源项目）
[源码 2](https://github.com/crazypeace/Url-Shorten-Worker)，[教程](https://zelikk.blogspot.com/2022/07/url-shorten-worker-hide-tutorial.html)
[源码 3](https://github.com/xyTom/Url-Shorten-Worker/)
[源码 4](https://github.com/Closty/duanwangzhi)
[源码 5](https://github.com/Likenttt/eastlake-cloudflare-worker-short-url)，[教程](https://blog.661212.xyz/index.php/archives/4/)

**通过 workers 等监控网站状态：**
[源码](https://github.com/eidam/cf-workers-status-page)（也可以通过 Uptimerobot 实现网站健康状态监控，[源码](https://github.com/yb/uptime-status)）
[教程](https://linux.do/t/topic/10601)

**通过 workers 等搭建临时邮箱：**
[源码](https://github.com/dreamhunter2333/cloudflare_temp_email)

**通过 workers 等搭建 RSS 订阅生成器：**
[源码](https://github.com/yllhwa/RSSWorker)内含教程

**通过 workers 等部署 Copilot 服务：**
Copilot（原 New Bing）可以试用 ChatGPT４，目前通过 Workers 就可以部署本地可用的 Copilot 服务。
[源码](https://github.com/Harry-zklcdc/go-proxy-bingai)　内含教程
[试用示例](https://bingai-cfwk.zklcdc.xyz/web/#/)
[其他方式部署 Copilot 的试用网址](https://github.com/Harry-zklcdc/go-proxy-bingai/wiki/%E6%BC%94%E7%A4%BA%E7%AB%99)

**通过 workers 等部署 Telegram Bot 服务：**
[源码](https://github.com/Tsuk1ko/cfworker-telegraf-template) 
[教程](https://moe.best/tutorial/cfworker-telegraf-tgbot.html)

### 中转
[Gh-proxy: Github 项目加速](https://github.com/hunshcn/gh-proxy)
[Jsproxy](https://github.com/EtherDream/jsproxy/tree/master/cf-worker)
[Workers-Proxy](https://github.com/klightso/Workers-Proxy-1)，[参考教程](https://www.locmjj.com/274.html)

### 网盘文件列表
**利用 Workers 搭建 Google Drive 列表服务：**
[源码 1](https://github.com/xunyixiangchao/goindex%EF%BC%9B)
[源码 2](https://github.com/yanzai/goindex%EF%BC%9B)
[源码 3](https://github.com/Aicirou/goindex-theme-acrou)
[源码 4](https://github.com/maple3142/GDIndex)

**OneDrive-index:**
 **利用 Workers 搭建 OneDrive 列表服务：**
[源码 1](https://github.com/spencerwooo/onedrive-cf-index)
[源码 2](https://github.com/Eggsmemory/OneDrive-Index-Cloudflare-Worker-Cht)

转自[Cloudflare Workers优秀项目收集（持续更新）](https://igdux.com/workers)