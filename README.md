
### 相关教程请查看[甬哥博客与视频教程](https://ygkkk.blogspot.com/2023/09/openwrt-cdnip.html)

### 一键脚本
```
curl -ksSL https://gitlab.com/rwkgyg/cdnopw/raw/main/cdnopw.sh -o cdnopw.sh && bash cdnopw.sh
```
### 进入脚本快捷方式：```bash cdnopw.sh```
--------------------------------------

![47918a52b4d93487e5e7935d5916d34](https://github.com/yonggekkk/openwrt_win64-ddns-cdnip/assets/121604513/dd6758ec-f8d4-4a6c-b51d-9144ec993193)

优选IP天花板教程，小白懒人特供版！openwrt软路由优选IP高度自定义一键脚本，支持优选官方IP、反代IP、13个端口随便选、有无域名都支持TG通知，让你了解优选官方IP与反代IP的各自特点，一切近在你掌握中

小白们可以自己搞一个时时更新多个优选IP的域名，客户端地址都可用此优选域名。软路由脚本移植到了电脑端，优选IP的主要功能全部支持。利用反代功能，在无代理的情况下也支持Telegram机器人通知，也支持Pushplus微信通知，支持自定义批量优选IP上传到域名解析与删除解析记录（支持IPV4与IPV6混合）




视频教程（先看）：openwrt软路由优选IP终极小白教程第一期：一键脚本支持优选官方IP、反代IP、13个端口随便选、有无域名都支持TG通知，x-ui与CF vless联合演示，全网独家解读优选官方IP与反代IP的各自特点（https://youtu.be/jro6gYnfsVY?si=eV8fisxOesKhgUNq）



视频教程（推荐）：OpenWrt软路由优选IP终极小白教程第二期：更新支持多个优选IP解析同一个域名方案，全网独家电脑端优选IP一条龙应用发布，支持无代理TG与Pushplus微信通知，支持自定义批量优选IP上传到域名解析（https://youtu.be/axI6gUZ7qSM?si=4nlFimfkOSdMGj8s）



---------------------------------------------------------------------------------------------

说明链接：

点击Github项目地址：甬哥的CF-vless脚本（https://github.com/Kisoul/Cloudflare-workers-pages-vless）

TG机器人获取key与ID视频教程

甬哥使用的openwrt固件定制地址：https://openwrt.ai/

-----------------------------------------------------------------------------------

相关说明必看（想到哪写到哪）：



进入脚本的快捷方式：bash cdnopw.sh



一、软路由只要能进SSH，就输入脚本运行。如果不成功，选择卸载就可以，不会对软路由其他东西造成任何影响，因为脚本仅仅在一个文件夹里运行而已，不改任何路由器参数。放心折腾吧。



二、重要的事说三遍：

运行脚本时，指定的代理插件保持开启状态

运行脚本时，指定的代理插件保持开启状态

运行脚本时，指定的代理插件保持开启状态



三、有些路由器进入SSH后，默认可能不是root目录，请确保在root目录中运行脚本。比如，先输入cd /root



四、关于提示“xxxx not found”报错问题

一般情况下你可以尝试执行：opkg install xxxx名称

提示timeout not found：运行opkg install coreutils-timeout 

提示base64 not found：运行opkg install coreutils-base64

更新时代理开启或者关闭都尝试下

如果还是报错，只能离线更新或者换个固件试试了。。。。

目前已知必装依赖：timeout 、jq、base64、unzip，请大家先自查下有没有安装



五、如果你有自己的IP库，你必须选择CDN官方IP模式，安装好后，进入/root/cfipopw文件夹内，把ip.txt同名文件替换掉就可以了，由于反代IP模式每次自动运行会更新覆盖，而官方iP模式目前定死的，你们可以随便自定义IP（电脑版改ipv4.txt）



六、如果电脑版优选出现“hosts文件错误：[Errno 13] Permission denied”报错，请右击管理员身份运行



七、多个优选IP解析同一个域名方案，默认10个IP。可以在安装执行时修改显示个数，一般2-3个就可以了。

-------------------------------------------------------------

### 参考项目：[lee1080](https://github.com/lee1080/CloudflareSpeedTestDDNS)

### 感谢：CF优选IP库及程序作者[badafans](https://github.com/badafans/Cloudflare-IP-SpeedTest)、[XIU2](https://github.com/XIU2/CloudflareSpeedTest)
