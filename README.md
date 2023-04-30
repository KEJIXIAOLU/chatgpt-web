# 一键免费部署你的私人 ChatGPT 网页应用
之前尝试过在Telegram、微信等调用ChatGPT，由于使用体验不太好，且微信里容易封号。这两天无意看到一个Docker项目，可以快速搭建私人ChatGPT网页应用，让您可以随时随地无需翻墙，就可以方便地访问ChatGPT。
## 什么是ChatGPT Next Web？
简单地说，ChatGPT Next Web就是可以一键免费部署你的私人 ChatGPT 网页应用。其主要特点是：

- 在 3 分钟内使用 Vercel 免费一键部署；
- 精心设计的 UI，响应式设计，支持深色模式；
- 极快的首屏加载速度（~100kb）；
- 海量的内置 prompt 列表，来自中文和英文；
- 自动压缩上下文聊天记录，在节省 Token 的同时支持超长对话；
- 一键导出聊天记录，完整的 Markdown 支持；
- 拥有自己的域名？好上加好，绑定后即可在任何地方无需翻墙无障碍快速访问。

在此，感谢作者Yifei Zhang，其项目地址[在这里](https://github.com/Yidadaa/ChatGPT-Next-Web/blob/main/README_CN.md#%E5%BC%80%E5%A7%8B%E4%BD%BF%E7%94%A8)。


## 准备工作
1、准备好你的 [OpenAI API Key](https://platform.openai.com/account/api-keys);

2、域名一个：没有域名请到[Namesilo购买域名](www.namesilo.com )，虽然不是必须的，但有自己的域名好处多多，具体如下：

- 使用下面用到的Vercel部署时，其自带的域名在中国大陆地区有可能是被封禁的，使用自己的域名即可无障碍直连访问；

- 在Namesilo上（无需翻墙地址：https://makemedollar.com/Namesilo）  购买.xyz的域名每年也就7元，只要您购买的域名长度在6位数，那么续费是一律都是0.99美元；
如果您想长期使用，建议购买.com的域名；

- Whois隐私（不会公布域名拥有者的真实信息）在NameSilo是免费的，而NameCheap需要2.88美金/年。

- NameSilo要比NameCheap拥有的顶级域名（TLD）要多。

## 开始部署
### 步骤1：部署在Vercel上

点击右侧按钮开始部署： [Deploy with Vercel](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FYidadaa%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web)，直接使用 Github 账号登录即可。

### 步骤2：设置API Key和CODE

记得在环境变量页填入 API Key 和页面访问密码 CODE（访问密码，最好是7位数以上的复杂密码）。然后按“Deploy”开始部署。

部署完毕后，即可开始使用；

### 步骤3：绑定自定义的域名

绑定自定义域名：Vercel 分配的域名 DNS 在某些区域被污染了，绑定自定义域名即可直连。

绑定域名的[官方教程](https://vercel.com/docs/concepts/projects/domains/add-a-domain)。

不懂托管域名到CloudFlare的小伙伴，可以[参阅这里](https://youtu.be/1GtDTWybJNM)。
完成域名绑定服务器后，即可正常访问您的域名，开始使用独享的网页版ChatGPT！

