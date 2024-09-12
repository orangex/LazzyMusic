<div align="center">
<img width="" src="./icon_rounded_512.png"  width=160 height=160  align="center">

# LazzyMusic
</div>    

正如其名，我折腾是想大家不用折腾，LazzyMusic 是一个自带客户端（播放器）的，多平台的，本地音乐流媒体服务。

简单来说，你可以从不同的设备访问和播放你在电脑上的音乐收藏，支持视频格式，支持导入或订阅外部音乐，支持元信息刮削和编辑。

希望能给你一个涵盖音乐获取、管理、播放的无缝优质体验。

## 功能特性 :sparkles: 

- **支持视频形式的音乐**：音乐不只是音频，拯救想将 Live、MV 等统一纳入音乐收藏的你
- 实时转码和预加载：iOS 能听 Opus 格式，Android 上也能听 Alac，等等。畅听不等待。
- 多种形式入库：
    - 导入已有的本地文件：支持随意重命名文件和变更文件位置（在媒体库文件夹内）
        
    - **订阅外部播放列表**：不用离开当前 app，你只管收藏，我来定时检查并导入外部歌单新增的部分
        
      * [x] Bilibili 收藏夹
      * [ ] Youtube 播放列表
      * [x] 网易云歌单（可能需要设置代理,见 Q&A）
      * [ ] QQ 音乐、Spotify 等等
        
- 媒体信息刮削与编辑：
    - **入库刮削**：入库时自动匹配元信息（歌曲名，歌手，歌词，专辑封面，专辑曲目等），即使文件信息残缺也会尝试通过声纹匹配。
    - **元信息编辑**：随时轻松地为歌曲纠正和补充元信息，目前支持搜索和指定歌手，专辑，歌词。
    - 支持歌曲和专辑多位歌手，支持专辑多音轨
    - “化繁为简”：自动将信息源中的繁体歌名、歌手名等统一为简体，不会再有同时存在周杰伦和周杰倫这种尴尬。
- 组织与播放：
    - 支持按专辑，歌手，歌单查看歌曲，支持按常见关键字排序。
    - 支持播放队列和不同的循环模式
    - **支持歌词，支持双行歌词，并可以调整歌词时间偏移。**
    - 支持后台播放，支持通过通知栏，控制中心控制。
    - 基于 Material 3 的简洁纯粹的 UI
- 多平台：
    - 服务端：Windows，Mac OS
    - 客户端：Android，iOS
- **外网访问**：一键尝试开启端口转发以支持外网访问，同时你可以自定义自行设置好转发的端口。
- **音乐库(包括元信息)的一切均保存在您的设备上**，无广无数据外泄，没有下架没有变灰，迁移友好，哪天你用或者不再使用 LazzyMusic 了，你的音乐依然静静躺在那里。

## 快速开始 :rocket: 

 1. 在你的 PC 上安装 Lazzy Music 服务端。
 
 2. 在手机上安装客户端，登录同一个账号。

 3. 添加音乐：添加本地音乐（并扫描），或订阅 Bilibili 收藏夹、网易云歌单等。
 
 等待一会，下拉刷新，就可以在客户端上看到你的音乐库了。具体如下：

### 服务端

前往[这里](https://github.com/orangex/LazzyMusic-Server/releases)下载最新版本 ，安装运行后系统托盘中（Mac 为屏幕右上角状态栏）会出现 LazzyMusic 的图标，右键登录即可。

更新方式：Windows 下载新的版本后直接将旧版本的程序删除然后安装新版本运行即可，Mac 常规安装新版即会覆盖更新。均需先退出程序。

### 客户端

iOS 已上架 [TestFlight](https://testflight.apple.com/join/5HaBxGxZ)，当然你可以通过下面的链接自行签名安装。

Android 暂未上架应用商店，可以直接通过（在手机的浏览器上访问，最好别用微信内置浏览器）下面的链接下载安装。

[客户端最新安装包](https://github.com/orangex/LazzyMusic/releases)，该链接指向的就是该仓库的 Release 。

### 添加第一首音乐

服务端右键托盘图标→打开媒体库文件夹，将你的音乐文件扔到里面，然后扫描仓库。

或者，从 Bilibili 分享视频至 LazzyMusic App

或者，在 LazzyMusic App 中订阅 Bilibili 收藏夹。详见 Q&A。

等待片刻，在客户端主页下拉刷新就会看见音乐在逐一出现在列表中了。

## 使用须知 :warning:
1. 请尽量干净的网络环境下使用，也就是说如果你正在使用代理、vpn 等，你明白它们作用的范围和效果。
2. 音乐库(包括元信息)的一切均保存在您的设备上，无广无数据外泄。
3. 产品还处于早期阶段，有很多粗糙的地方，请多包涵，欢迎所有友善的建议与声音。
   
## 截图展示 :camera:

服务端除了托盘图标和菜单，目前没有 GUI，以下为客户端部分界面展示。
<p float="left">
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%201.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%202.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%203.png" alt="Description" width="300"/>
<img src="https://github.com/orangex/LazzyMusic/blob/main/Untitled%204.png" alt="Description" width="300"/>
</p>


## Q&A :question:

见 [Wiki](https://github.com/orangex/LazzyMusic/wiki/Q&A)
