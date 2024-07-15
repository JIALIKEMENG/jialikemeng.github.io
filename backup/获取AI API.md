###  获取Google Gemini API
2023年12月6日，谷歌发布新一代大模型Gemini的demo, 同时，Bard已将模型更新为Gemini Pro。Gemini 是谷歌目前最新最强的大语言模型，支持多模态（文字，图片，音频，视频等等）处理。美国时间12月13日，Gemini API对公众开放。。
根据谷歌提供的价格信息，将会有两个收费方式，现阶段的免费版本可以每分钟60次请求，足够满足个人用户的需求了。至于收费版本，目前还不能用，但是收费标准已经公布了。Gemini Pro 付费版的定价是每千个字符0.00025美元，每张图片0.0025美元，输出每千个字符0.0005美元。另外谷歌会使用免费版Google Pro API的输入和输出来提高模型能力，但是承诺付费版不会用于训练和改进产品（保护隐私）。
- 准备一个谷歌账号，已经有了请跳过。
- 建议使用美国等非国区/港区节点访问。参看[Google AI Studio 和 Gemini API 支持的语言和地区](https://ai.google.dev/available_regions?hl=zh-cn)。
- 打开Google AI Studio [申请api的网址](https://makersuite.google.com/app/apikey)，当然你也可以打开[Gemini的首页](http://ai.google.dev) ，并点击 Get API key in Google AI Studio 按钮。你需要先同意使用条款才能继续使用。
- 点击左边菜单里的 Get API key，然后在右边点击 API keys 下方的 Create API key in new project。出现 API key generated ，Google Gemini API 生成成功，即可 copy 使用。
参看[Google Gemini API快速上手(附申请步骤)](https://blog.csdn.net/zwqjoy/article/details/135058668)

###  获取ChatGPT API Key（官方）
- 打开 [openAI 官网](https://platform.openai.com/)并登录。
- 点击右上角的个人中心，之后在弹出的框中点击 View API keys 。
- 在跳转的页面中，点选 Create new secret key ，新建一个key 。
- 在弹出的创建框中填写一个名字，方便备注，然后点击 Create secret key 创建。
- 之后出现的一串字符就是API key了，点选旁边的绿色按钮即可复制调用。
参看[如何申请调用ChatGPT API 以及key秘钥获取方法](https://zhuanlan.zhihu.com/p/651877443)。

[Open ChatGPT API Key 有效性检测](http://tools.lbbit.top/check_key_valid/)

参看[ChatGPT 使用教程以及免费接口(支持OpenAI所有模型)](https://t66y.com/htm_data/2403/7/6229592.html)。