![](../images/banner.png)

<hr>


##### 硬酷R1主要应用场景：


1. **家庭防火墙（Firewall）：** <br>
   随着国内互联网过去10年的高速发展，黑客攻击和广告追踪，越来越影响我们的日常冲浪体验。借助硬酷R1，用户可安装pFsense、OPNsense、iKuai、OpenWRT等主要防火墙和流控的开源路由系统，轻松实现家庭网络的安全掌控。更有极客玩家安装ROS系统、Panabit等系统。在硬酷R1和各种开源的路由系统的加持下，我们可以轻松实现家庭网络去广告、自建DNS服务等，使我们的私有内网更安全。
2. **虚拟机（Hypervisor）：** <br>
   硬酷R1基于通用x86架构设计，你可以安装运行 XCP-ng、Citrix Hypervisor、ESXi、Proxmox 等虚拟机。
   - 4 个i226-IT 2.5G网口可让您将专用网络资源分配给各个虚拟机或容器；
   - 使用赛扬N5105/奔腾N6005，高达16GB内存可选，可以部署更多虚拟机；
3. **远程办公（Remote Office）** <br> **<small>（前提：有公网IP，且拥有一个可用于DDNS服务的域名）</small>** ：<br>在疫情期间，远程办公逐渐兴起。借助DDNS+端口转发，可以实现人在异地，远程通过Microsoft Remote Desktop工具登陆办公电脑，实现远程操控，体验更流畅。 
4. **Docker宿主机：**  (**<small>基于虚拟机之上玩各种套娃Docker服务</small>**)  <br>
   可以物理直装Linux系统，并安装docker服务，借助docker实现各种各样的微服务。也可以基于虚拟机之下的Linux系统上安装docker跑各种个性化需求的微服务。
   - Bitwarden/Vaultwarden —— 超好用的密码管理工具
   - Alist —— 超好用的在线网盘挂载工具
   - Qinglong —— 功能强大的定时任务管理面板
   - PhotoPrism —— 优秀的相册管理工具
   - Nginx Proxy Manager —— 强大的反向代理工具
   - Transmission/qBitorrent —— PT下载神器
   - 更多好玩有趣的docker镜像，等待您去发现...
5. **下载机：** <br>
   可以直装Windows当各种云网盘的下载机，也可以借助docker安装各种pt下载工具，轻松玩转pt。
6. **家庭媒体服务器：** <br>
   借助诸如jellyfin, Plex, alist等docker工具，轻松扮演家庭内网的媒体服务器。

<hr>


![](../images/Banner_tw.png)