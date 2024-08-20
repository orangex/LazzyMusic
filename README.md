# Lazzy Music

---

正如其名，我折腾是想大家不用折腾，Lazzy Music 是一个自带客户端的多平台的本地音乐流媒体服务，希望能给你一个涵盖音乐获取、管理、播放的无缝优质体验。

## 快速开始:

在你的 PC 上安装 Lazzy Music 服务端，在手机上安装客户端，登录同一个账号，添加音乐，等待片刻就可以在客户端上尽情享用了。

### 服务端

前往这里下载最新版本 [https://github.com/orangex/LazzyMusic-Server/releases](https://github.com/orangex/LazzyMusic-Server/releases) ，安装运行后托盘中（Mac 为屏幕右上角状态栏，Windows 为右下角托盘）会出现 LazzyMusic 的图标，右键登录即可。

更新方式：Windows 下载新的版本后直接将旧版本的程序删除然后安装新版本运行即可，Mac 常规安装新版即会覆盖更新。均需先退出程序。

### 客户端

iOS 已上架 TestFlight，[https://testflight.apple.com/join/5HaBxGxZ](https://testflight.apple.com/join/5HaBxGxZ)，当然你可以通过下面的链接自行签名安装。

Android 暂未上架应用商店，可以直接（在手机上）通过下面的链接下载并安装。

[https://github.com/orangex/LazzyMusic/releases](https://github.com/orangex/LazzyMusic/releases)，即为该仓库的 Release 。

### 添加第一首音乐

服务端右键托盘图标→打开媒体库文件夹，将你的音乐文件扔到里面，你也可以在客户端上完成上述的步骤。

等待片刻，在客户端主页下拉刷新就会看见音乐在逐渐出现在列表中了。

你也可以订阅外部的歌单，目前仅支持 Bilibili 收藏夹，详见 Q&A。

## 功能特性:

- 支持视频形式的音乐：音乐不只是音频，将你最爱的现场视频 、MV 等珍藏起来吧！
- 多种形式入库：
    - 添加本地文件：你可以随时向音乐库文件夹里丢新的音乐文件它们会被第一时间感知并入库。
    - 从其他 APP 分享：刷到了喜欢的音乐？你可以系统分享到 Lazzy Music App，自动入库。
        
        目前支持的平台是：Bilibili
        
    - 订阅外部播放列表：懒得点分享？你也可以直接将该音乐收藏在该平台的自己的歌单(/收藏夹/播放列表)中，当在 Lazzy Music 中订阅该歌单后, 未来歌单中的新增歌曲会出现在你的音乐库中。
        
        目前支持的平台有：Bilibili
        
- 媒体信息刮削与编辑：
    - 入库刮削：歌曲入库时通过自动匹配歌曲信息，包括歌曲名，歌手，歌词，专辑封面，专辑曲目。即使你的文件信息残缺也会尝试通过声纹匹配。
    - 元信息编辑：对于匹配不成功，非原唱歌曲，同名歌曲专辑等等导致元信息需要纠正的情况，你可以随时轻松地为歌曲搜索指定正确的歌手，专辑，歌词。
    - 支持歌曲、专辑多歌手，专辑多音轨
    - “化繁为简”：歌名、歌手名等统一为简体，因此也不会有音乐库中同时存在周杰伦和周杰倫这种尴尬。
- 组织与播放：
    - 支持按专辑，歌手，歌单查看歌曲，并按常见关键字排序。
    - 支持播放队列，与常见循环模式
    - 支持歌词，支持双行歌词，并可以调整歌词时间偏移。
    - 支持后台播放，支持通过通知栏，控制中心控制。
    - 基于 Material 3 的简洁纯粹的 UI
- 多平台：
    - 服务端：Windows，Mac OS
    - 客户端：Android，iOS
- 外网访问：一键尝试开启端口转发以支持外网访问，同时你可以自定义自行设置好转发的端口。
- 音乐库(包括元信息)的一切均保存在您的设备上，无广无数据外泄，没有下架没有变灰，迁移友好。

## 截图展示

服务端除了托盘图标和菜单，目前没有 GUI，以下为客户端部分界面展示。
<p float="left">
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%201.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%202.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%203.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%204.png" alt="Description" width="300"/>
</p>


## Q&A

1. 如何反馈问题，提出建议？有主页吗？
    
    GitHub issues。 可以将这里暂时视作主页，正在思考创建其他更新动态的方式，比如社群、频道。
    
2. 我可以在多个地方登录吗？
    
    客户端可以多处登录。服务端不行，不然客户端不知道到底要连接哪个音乐库。而目前还未开发对服务端的登录限制，因此为了避免上述异常，如果你要在别处再次登录，请在先前的设备上先登出。
    
3. 什么是通过端口转发从外网访问？我没有公网 IP 可以吗？
    
    简单来说， 通过服务所在的公网 IP 加上端口可以访问一个公网上的服务，但对于内网中的服务，则无法直接访问，这时可以在路由器上配置转发规则将对该公网下某端口的请求映射到某内网 IP的某端口上。这样就实现了从外界访问你的本地服务。另，通过端口转发，实际上是将你局域网中的设备暴露在了互联网上，请知悉其有一定风险。
    
    不可以没有公网 IP，想要通过该方式从外网访问，一定需要公网 IP，目前国内的现状是普遍需要自行向运营商申请，申请方法和申请后的路由器配置网络上有很多经验贴可以参考。不过 Lazzy Music 并不要求公网 IP 是静态的。
    
    后续会考虑以更多形式支持从外网访问的需求，比如自行指定服务器地址等等。
    
4. 如何订阅外部歌单（Bilibili 收藏夹）?
    
    订阅外部歌单的行为是绑定在内部歌单上的，这是为了更好的归集不同歌单的音乐，比如你可以在一个叫“Live 集合”的内部歌单中订阅不同平台（虽然目前还只支持 bilibili）的“我喜欢的 Live” 歌单。
    
    订阅操作：你可以通过歌单→三个点→为歌单新增订阅一个外部歌单，也可以在应用顶部点击“+”号→订阅 bilibili 收藏夹的方式快捷创建一个订阅某外部歌单的歌单，均需要输入外部歌单的链接。
    
    Bilibili 收藏夹链接目前只能通过前往 Bilibili 网站获取，在收藏页面左侧找到你创建的收藏夹，复制此时浏览器地址栏的地址即可，地址形如：[https://space.bilibili.com/4932305/favlist?fid=1234567890&ftype=create](https://space.bilibili.com/4932305/favlist?fid=2813308305&ftype=create) ，也可以点击进入该收藏夹详情，复制此时地址栏地址，形如[https://www.bilibili.com/medialist/detail/ml1234567890?](https://www.bilibili.com/medialist/detail/ml2813308305?) ，注意收藏夹需要是公开的（默认就是公开的）。
    
    取消订阅：歌单→三个点→为该歌单取消订阅某个外部歌单，或者你可以直接删除某内部歌单，其订阅行为也随之消失。
    
5. 后续产品思路？
    
    核心还围绕为本身就有（本地）音乐收藏或着构建私人音乐库有兴趣的用户，让获取和入库音乐更简易，支持的方式和平台更多，让音乐库（元信息）的获取和整理变的更省心，同时提升音乐播放的质量和体验。
    
6. 定价？
    
    远远没来得及想，有计划会及时同步。
