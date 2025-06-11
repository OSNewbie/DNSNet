<div align="center">
  <img src="assets/feature-graphic.png" alt="DNSNet feature graphic" width="50%"/>
</div>

基于 DNS66，DNSNet 在现代 Android 开发下延续原应用：  
一个本地 DNS 屏蔽器，默认使用多份可信 hosts 文件拦截广告、恶意软件等。

<div align="center">
<a href="https://hosted.weblate.org/engage/dnsnet/">
<img src="https://hosted.weblate.org/widget/dnsnet/287x66-black.png" alt="Translation status" height="80" />
</a>
</div>

屏幕截图
-----------

<div align="center">
<img src="metadata/en-US/images/phoneScreenshots/start-p9p.png" width="20%" /> 
<img src="metadata/en-US/images/phoneScreenshots/hosts-p9p.png" width="20%" /> 
<img src="metadata/en-US/images/phoneScreenshots/apps-p9p.png" width="20%" /> 
<img src="metadata/en-US/images/phoneScreenshots/dns-p9p.png" width="20%" />
</div>

安装方式
----------

<div align="center">
<a href="https://f-droid.org/packages/dev.clombardo.dnsnet/">
<img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png" alt="Get it on F-Droid" height="80">
</a>
<a href="https://play.google.com/store/apps/details?id=dev.clombardo.dnsnet">
<img src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png" alt="Get it on Google Play" height="80">
</a>
<a href="https://accrescent.app/app/dev.clombardo.dnsnet">
<img src="https://accrescent.app/badges/get-it-on.png" alt="Get it on Accrescent" height="80">
</a>
</div>

或从 [Releases](https://github.com/t895/DNSNet/releases/latest) 下载 APK。

工作原理
------------

利用 Android VPN 服务 API，本地拦截所有 DNS 请求，按“过滤器”设置放行或阻止。  
缺点：  
- 持续运行会消耗一定电量；  
- 仅能与系统中唯一的 VPN 服务共存。

更多详情见 [FAQ](https://github.com/t895/DNSNet/wiki/FAQ)。

隐私保障
-----------------

DNSNet 只减少出站数据：除了下载 hosts 文件外，不会发送额外流量，也不添加请求信息。

参与贡献
------------

详见 [CONTRIBUTING.md](CONTRIBUTING.md)

编译说明
--------

前置工具：Rust、Python 3、Java 17+（可选 Android Studio）  
需添加 Android NDK 环境变量并安装 cmake、make。  
Windows 构建因 quiche 库问题暂不可用；macOS Android Studio 可能识别不到 Rust，请使用命令行或 `open -na "Android Studio.app"` 启动。

许可证
-------

本程序遵循 GNU GPL v3（或更高版本）。详见 [COPYING](COPYING)

行为准则
---------------

详见 [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

作者
-------

Charles Lombardo <clombardo169@gmail.com>  
界面服务由 Julian Andres Klode <jak@jak-linux.org> 提供  
部分代码源自 Daniel Brodie 的 AdBuster（https://github.com/dbrodie/AdBuster）
