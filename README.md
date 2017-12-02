# 简介

**Mac 世界之窗**：三步搭建一个自己的 **🔴私人代理服务器🔴**：

> 1. 购买一个指定类型的服务器（**提供一个自己的私人邮箱**）
> 2. 下载 “世界之窗”：🔴**[世界之窗下载地址](https://github.com/WindowOfTheWorld/TheWorld/releases/tag/世界之窗最新版)**🔴
> 3. 用该邮箱 在世界之窗上登录，登录成功后，后台会自动到用户指定的 vps 上部署代理服务，部署完成后用户就可以正常使用了。

**注**：“世界之窗”只是一个工具，本身不能提供代理服务，需要用户先自行购买 服务器，按照上述步骤进行配置安装，过程简单易懂。



相比其他手段，**世界之窗**搭建 私人代理服务器的 特点：

> - **Google 秒开**
> - **私人服务器**：属于自己的，私密安全。
> - **自动分流**：客户端会自动区分：需要翻墙的走代理服务器，不需要的直接走国内。这样访问一些正常的网站，和平时没什么差别。*想以前不能访问的站点，现在也能正常浏览，而且超快的*。
> - **稳定**：自己的服务器自己用。不用几万人挤在一起。一个人占了网速，自己就没办法用了。
> - **动态 IP**：一旦服务器ip 地址被屏蔽，可以立马切换服务器地址，零差价。



*有问题请联系*：worldwindow9@gmail.com



# 背景

作者是程序猿一枚，十几年一如既往、不忘初心，作者爱 Coding。

作者翻墙80%的时间都是在浏览 Google、stackoverflow 等技术网站，可以说是 Google 或者类 Google 这样科技网站的重度依赖者。回顾一下自己的翻墙历史：

2010年 Google 宣布退出中国后，国内用户只能从gooogle.cn 切换到 google.com.hk。但是从10年开始，GFW 逐渐加大对google.com.hk请求的干扰，到11年丢包率达到50%以上，那时候同事之间经常开玩笑说：Google 能不能打开，得看 RP，一看你的人品就不行。接着到11年底的时候，google.com.hk 基本上完全打不开，Google就这样宣布被完全拦在国门之外了。

为了能正常学习最新技术，从11年开始，自己陆续尝试了各种 VPN、代理，免费的、付费的，像[GoAgent](https://zh.wikipedia.org/wiki/GoAgent)、 GreenVPN、红杏、自由之门、蓝灯等。从一个月大几十的到一年几百的，有一些能正常用一段时间，也有一些就是为了骗钱，收了钱没过段时间就跑路了...感觉那段时间为了能上网查点有用的资料，没少折腾。现在想想那会自己的忍耐度也是很强的，但凡能用的方法，自己都会毫不犹豫地去尝试、根本不敢奢望能够有个稳定、快速、体验好的工具了。

**春天来了**：13年的时候，在 GitHub 上无意中发现了大神Clowwindy的开源项目。一番学习和体验后，终于知道怎样才算真正的翻墙体验，稳定、低延时（Google 低于50ms 延时）。



后来身边的朋友强烈要求在国外搭建一些相关服务，免费提供给身边的朋友使用。自己利用业余时间把这些功能整理成一个批处理包括（自动部署服务器、更换切换服务器等），如果有朋友需求，可以使用该脚本在特定服务器上部署使用（自己一直在用，速度比其他商用 vpn，代理好很多）当然前提得先自己购买一个服务器，价格也能接受，性价比要比外面的一些商用的高很多。

**注**：该工具只提供给和作者一样的技术研发、产品设计、科技工作者用于查阅国际资料使用，这里面没有政治、只有技术。所以该工具只提供访问一些科技、设计网站的访问权限，禁止政治、种族等相关网站以及相关人员的使用。



# 特点

使用该工具前提得先自己购买 vps。具体操作很简单，有兴趣请 Email：worldwindow9@gmail.com，一键部署属于自己的**个人代理**。

简单讲讲**个人代理**的具体特点：

#### 1. 比 VPN 更优秀、更安全

十九大后VPN 将逐渐退出中国市场，现在各个地方已经在逐步清理 vpn 软件及厂商。因为 vpn 协议更容易呗 GFW 识别，不得已很多 vpn 厂商只能卷款跑路了，坑了哪些年付费的用户了。相比，我们的个人代理是基于[Socks5](https://zh.wikipedia.org/wiki/SOCKS#SOCK5)代理方式的网络数据加密传输包，加密算法包括[AES](https://zh.wikipedia.org/wiki/%E9%AB%98%E7%BA%A7%E5%8A%A0%E5%AF%86%E6%A0%87%E5%87%86)、[Blowfish](https://zh.wikipedia.org/wiki/Blowfish_(%E5%AF%86%E7%A0%81%E5%AD%A6))、[IDEA](https://zh.wikipedia.org/wiki/IDEA%E7%AE%97%E6%B3%95)、[RC4](https://zh.wikipedia.org/wiki/RC4)等，同时采用多种方式对数据进行混淆。所以相比 传统vpn 个人代理更难被识别。

#### 2. 动态 IP

为了防止服务器 IP 被屏蔽，我们的服务采用动态 IP，一旦发现被屏蔽，就立马更换 IP。

#### 3. 性价比更高

#### 4. 专属个人代理

#### 5. 小众工具

首先想说明的是：

“没有攻不破的技术，只要有足够的人力物力；

就像没有破不了的密码，只要有足够的人力物力”。

作者不会希望这个工具有太多的人使用。还是前面说明的那句话：它只服务于那些真正有需要的群体。比起蓝灯或者其他的公开商用工具，它可能属于那种更加“**私密**”、**小众**的群体。这里的“私密“代表不希望它成为公众的焦点、茶余饭后的话题，成为对抗 ZF权威及技术能力 的代表。

- 作者是一个和大多数人一样的**中国人**、**爱国者**
- 作者的标签是：热爱**科技**、**Coding**、**爱国**，要强调的是这里没有**政治**，只有**科技**
- **世界之窗**的标签是：**科技**、**互联网**、**Coding**

以上是作者的立场。

------



# 产品内容

如果你觉得自己和作者一样是一个重度依赖者，觉得自己需要一个这样的工具，欢迎邮件联系：worldwindow9@gmail.com。作者会带你一起愉快的遨游于互联网的海洋中。

# 下载地址

**🔴**[世界之窗下载地址](https://github.com/WindowOfTheWorld/TheWorld/releases/tag/世界之窗最新版)**🔴**

联系：worldwindow9@gmail.com


