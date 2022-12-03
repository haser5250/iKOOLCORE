# 硬酷R1：

[TOC]

### 一、产品介绍：

![](https://u.iswott.com:8888/d/Pics/Banner_404.png)

> 硬酷R1（iKoolCore R1）是一个迟来的硬件项目，由推特网友 **[Jackeroo](https://twitter.com/isJackeroo)** 联合深圳的硬件工厂推出的目前市场最小巧且性能强大的4网口2.5G小主机。“方寸之间 尽享乐趣” 是硬酷R1的slogon。

#### 1. 设计初衷：

<h3><center>方寸之间 尽享乐趣！<br>
1️⃣极致小巧 颜值在线<br>
2️⃣性能强大<br>
3️⃣多网口2.5G<br>
拒绝❌傻❌大❌黑❌粗<br>
❌拒 绝 减/简 配！ ❌拒 绝 电 子 垃 圾❌<br>
聚集一群有共同兴趣爱好的小伙伴</center></h3>
![](https://u.iswott.com:8888/d/Pics/mul_banner.png)

#### 2. 硬件设计：

> 从零到一，独家开发。

##### 硬件选型：

- CPU：赛扬N5105、奔腾N6005

- 内存：LPDDR4 双通道，单颗粒8GB （`16GB内存双通道双颗粒`）

- 网卡：Intel i226-V  **<small>（优于Intel i225-V）</small>** 

- 硬盘： **<small>M.2 NVME 2242 （x2速率）<br>NVME/SATA双协议支持，但默认BIOS仅支持NVME协议硬盘。如有需要，后续放出支持SATA协议的BIOS。</small>** 

- 显示：HDMI 2.0 4K 60Hz视频输出

- USB： USB 3.1 Gen1 x 2；USB-C 3.1 Gen1 x 2；

- TF：TF Card Slot x 1 **<small>（支持启动）<br>已测试：Linux下可启动，Windows不可启动</small>** 

- 散热：主动散热<br> **<small>后续会有升级版本散热器单独销售。散热是我们一直会努力优化的点。</small>**

- 电源：标配 12V 2.5A 30W DC电源 **<small>（定制Type C接口电源） <br>特殊定制DC电源，请使用标配电源给R1供电！请勿使用其他C口PD电源供电，以免烧坏主板。因乱用电源烧坏主板，需要自行承担！</small>** 

- 尺寸：7.5 x 7.5 x 4.8cm **<small>(方寸之间，尽享乐趣)</small>**

  

##### 工程设计：

![](https://wiki.ikoolcore.cn/images/DesignFile_2.png)

![](https://wiki.ikoolcore.cn/images/DesignFile_3.png)

![](https://wiki.ikoolcore.cn/images/DesignFile_4.png)

![](https://wiki.ikoolcore.cn/images/DesignFile_1.png)



### 二、应用场景

1. **家庭防火墙（Firewall）：** <br>
   随着国内互联网过去10年的高速发展，黑客攻击和广告追踪，越来越影响我们的日常冲浪体验。借助硬酷R1，用户可安装pFsense、OPNsense、iKuai、OpenWRT等主要防火墙和流控的开源路由系统，轻松实现家庭网络的安全掌控。更有极客玩家安装ROS系统、Panabit等系统。在硬酷R1和各种开源的路由系统的加持下，我们可以轻松实现家庭网络去广告、自建DNS服务等，使我们的私有内网更安全。

2. **虚拟机（Hypervisor）：** <br>
   硬酷R1基于通用x86架构设计，你可以安装运行 XCP-ng、Citrix Hypervisor、ESXi、Proxmox 等虚拟机。

   - 4 个i226-IT 2.5G网口可让您将专用网络资源分配给各个虚拟机或容器；
   - 使用赛扬N5105/奔腾N6005，高达16GB内存可选，可以部署更多虚拟机；

3. **远程办公（Remote Office）** <br>
   **<small>（前提：有公网IP，且拥有一个可用于DDNS服务的域名）</small>** ：
   在疫情期间，远程办公逐渐兴起。借助DDNS+端口转发，可以实现人在异地，远程通过Microsoft Remote Desktop工具登陆办公电脑，实现远程操控，体验更流畅。

4. **Docker宿主机：** (**基于虚拟机之上玩各种套娃Docker服务**) <br>
   可以物理直装Linux系统，并安装docker服务，借助docker实现各种各样的微服务。也可以基于虚拟机之下的Linux系统上安装docker跑各种个性化需求的微服务。

   - Portainer——Docker图形化管理工具

   - Alist —— 超好用的在线网盘挂载工具

   - LibreSpeed——内外网测速工具

   - OpenSpeedTest——高颜值内外网测速工具

   - Squoosh——GoogleChromeLab团队出品的开源图片压缩工具

   - PhotoPrism —— 优秀的相册管理工具

   - TrwebOCR——OCR在线识别工具

     **<small>具体以默认系统部分信息为准</small>**

5. **下载机：**<br>
   可以直装Windows当各种云网盘的下载机，也可以借助docker安装各种pt下载工具（transmission/qbittorrent等），轻松玩转pt。同时也可以基于PVE/ESXi/Unraid等虚拟机下安装开源NAS系统，通过直通USB硬盘设备作为存储盘 **可行，但不推荐。R1产品定位没有为NAS场景考虑**。

6. **家庭媒体服务器：**<br>
   借助诸如jellyfin, Plex, alist等docker工具，轻松扮演家庭内网的媒体服务器。

![](https://u.iswott.com:8888/d/Pics/banner.jpg)




### 三、默认系统


> 默认均安装PVE最新版(`pve-manager/7.3-3/c3928077`)底层系统，并在PVE宿主机下安装好了路由系统虚拟机、Debian11虚拟机、Windows10虚拟机。路由系统负责处理网络，Debian11下安装有Docker服务，并部署了各种了非常易用的docker服务，Windows10 LTSC系统开启远程桌面访问，方便配合DDNS实现远程内网管理和7 x 24小时下载一些必须依赖于Windows系统下的网盘资源（百度网盘、阿里云盘、迅雷下载等）。以下为宿主机和虚拟机的详情说明：

##### 宿主机：

| 宿主机系统 |         管理后台         |  账号  |    密码     |          备注           |
| :--------: | :----------------------: | :----: | :---------: | :---------------------: |
|  PVE7.3-3  | Https://192.168.1.2:8006 | `root` | `ikoolcore` | `注意https、端口号8006` |

**<small>默认安装好[PVE Status Tools](https://github.com/iKoolCore/PVE_Status_Tools)（可显示PVE宿主机的各项参数信息） ，因为安装系统和测试会有少量的读写量和通电次数，属于正常。</small>** 

##### 虚拟机

- 路由系统：

  |                          虚拟机系统                          |   IP地址    | 用户名 |    密码     |                      备注                      |
  | :----------------------------------------------------------: | :---------: | :----: | :---------: | :--------------------------------------------: |
  | ~~**OpenWRT, 爱快, pfsense, OPNSense, Panabit<br>(某国内开源路由系统)**~~ | 192.168.1.1 |  root  | `ikoolcore` | 请根据自己的喜好，自行设置自己需要的路由器系统 |

- Debian11

  | 虚拟机系统 |        IP地址        |       用户名        |    密码     |           备注           |
  | :--------: | :------------------: | :-----------------: | :---------: | :----------------------: |
  |  Debian11  | 192.168.1.3 `固定IP` | `root`  `ikoolcore` | `ikoolcore` | 管理员root和用户密码相同 |

  基于Debian11，已经安装docker服务，并基于docker容器，部署有以下微服务：

  |      容器服务       |         后台地址         |   用户名    |        密码        |         用途         |
  | :-----------------: | :----------------------: | :---------: | :----------------: | :------------------: |
  |      Portainer      | https://192.168.1.3:9443 | `ikoolcore` | `8a2^myngJ!Ynpfc`  | 可视化docker管理服务 |
  |        Alist        | http://192.168.1.3:5244  | `ikoolcore` | `ikoolcoreisgreat` |     网盘挂载服务     |
  |    OpenSpeedTest    | http://192.168.1.3:3000  |      -      |         -          |     网络测速服务     |
  |       Squoosh       | http://192.168.1.3:7701  |      -      |         -          |     图片压缩服务     |
  |      Qinglong       | http://192.168.1.3:5700  | `未初始化设置` | `未初始化设置`    |     青龙脚本面板     |
  |      NextCloud      | http://192.168.1.3:8080  | `ikoolcore` | `ikoolcoreisgreat` |     在线协作平台     |
  | Nginx Proxy Manager |  http://192.168.1.3:81   | `ikoolcore` | `ikoolcoreisgreat` |     反向代理服务     |

- Windows10 LTSC：

  |   虚拟机系统    |                   IP地址                    |  用户名   |    密码     | 备注 |
  | :-------------: | :-----------------------------------------: | :-------: | :---------: | :--: |
  | Windows 10 LTSC | 192.168.1.4<br>3389远程桌面管理端口：已打开 | iKoolCore | `ikoolcore` |      |


**以上仅限已经选购带硬盘配置的订单。**



### 四、产品与服务：

##### 产品购买：

<center><b>方寸之间 尽享乐趣<br>颜  值  在  线  性  能  强  劲</b></center>


|  CPU  | 内存大小<br> `板载，双颗粒双通道`<br/>`不可升级` | **[硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)** 大小<br> `NVMe协议`<br>`（SATA协议需求少，暂不生产）` |  价格  |                           购买链接                           |
| :---: | :----------------------------------------------: | :----------------------------------------------------------: | :----: | :----------------------------------------------------------: |
| N5105 |                       8GB                        | `不带` **<small>[单独选购硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)</small>** | ￥1069 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                       16GB                       | `不带`**<small>[单独选购硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)</small>** | ￥1369 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                                                  |                                                              |        |                                                              |
| N5105 |                       8GB                        |                            128GB                             | ￥1269 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                                                  |                                                              |        |                                                              |
| N5105 |                       16GB                       |                            512GB                             | ￥1869 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                                                  |                                                              |        |                                                              |
| N6005 |                       8GB                        | `不带`**<small>[单独选购硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)</small>** | ￥1269 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                       16GB                       | `不带`**<small>[单独选购硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)</small>** | ￥1569 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                                                  |                                                              |        |                                                              |
| N6005 |                       8GB                        |                            128GB                             | ￥1469 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
|       |                                                  |                                                              |        |                                                              |
| N6005 |                       16GB                       |                            512GB                             | ￥2069 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |

##### 选购建议：

1. 如果是计划物理机安装开源操作系统，选择 `N5105 + 8GB + 128GB` 足够折腾；
2. 如果是计划玩虚拟机，那么建议内存优先考虑16GB，如果仅是PVE下双软路由，8GB内存也是足够的；
3. 关于带硬盘配置的硬盘品牌问题：
   硬酷科技找OEM合作厂商专属定制硬盘，质保3年，放心使用。<br>带**[硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)** 配置订单，如需要代为安装系统，需下单时备注所需安装的开源操作系统。<br>部分512GB NVMe协议硬盘为从某售后服务中心拿到的 *三星PM991、PM991A、镁光C2450* 等数量极少。<br>优先给早期项目支持者 <small>**（已结束）**</small>。
4. OEM定制硬盘标签纸如下图所示：<br>
   - **[硬盘](https://item.taobao.com/item.htm?ft=t&id=686963354915)** 芯片信息：
     - NVMe主控：联芸(Maxio)科技 **MAP1202A-F1C  <small>(以128G为例，其他容量主控可能有变化) </small>** ，使用此款芯片的市售产品有： [海康威视CC500](https://zhuanlan.zhihu.com/p/394138333) 、[Lexar雷克沙NM610PRO](https://diy.pconline.com.cn/1535/15359085.html) 、[致态TiPlus5000](https://www.chongdiantou.com/archives/137851.html) 
     - 颗粒：长江存储
     - 保修政策： **3年只换不修**

##### 产品价格：

**<small>首先，感谢所有在10.1之前下单的下伙伴，让你们等货太久了。Thanks for your trust, support, waitting and suggestions!<br>所有在10月15日之前下单的小伙伴在订单交易成功之后，可以获得额外的¥20 RMB的红包返还，这个属于延迟发货的补偿，但我有一个小小的请求：交易成功后，请给我们一个5🌟好评（只要是中肯有理的非五星，都接受），并且带上3-5张R1实拍图，感谢感谢！</small>**

> **<small>特别强调：R1由于研发成本、物料成本、生产成本等多方面的成本因素考虑，目前的售价是非常便宜的，不确定现货后是否会涨价，以及涨价幅度。</small>**
>
> - **<small>研发成本：产品完全从0到1进行开发，整个产品出来，超过20位研发人员参与；</small>**
>
> - **<small>物料成本：贸易环境恶化，芯片涨价，人民币汇率跌，任何一个因素都导致元器件采购成本上涨，现在是三个因素一起来；</small>**
>
> - **<small>生产成本：疫情一下，防疫大于一切，中间因为疫情静默7天；总体进度受疫情有14-28天的进度影响。</small>**
>
>   **<small>mini PC内卷白热化，需求相对小众，利润有限，不参加优惠活动。</small>**



##### 产品调整：

首先，感谢你的耐心与漫长的等待，在您拆封本定制产品之前，烦请注意以下几点产品更改：

1. **关于TF卡**：TF卡无法支持Windows下的启动，但是可以作为普通存储使用，支持Linux下的启动；
2. **关于外观宣传图和实物差异：**
   - ***侧面散热隔栅：*** 出于风道设计，由原来的细孔变成两个大孔，另外一侧开孔取消，跟详情页图片有细微差别；
   - ***上盖：*** 上盖宣传图也是塑胶材质，后续上盖会有金属材质版本，可直接作为硬盘散热器，正在开发中...
3. **关于硬盘：**
   - ***硬盘协议：*** 由于NVME扩展性比SATA更好，我们首批没有量产SATA版本，如果你下单的是SATA版本，现现免费升级到NVME版本；
   - ***硬盘规格***：硬盘规格为M.2接口，2242尺寸，NVME协议，烦请自备硬盘小伙伴不要购买错硬盘以免浪费；
4. **关于电源：**
   - ***电源类型：*** DC电源，**请勿使用各位手头有的PD协议的C口电源**，谨防烧掉R1主板。**切记！切记！切记！**
   - ***其他说明：*** 不再标配PD诱骗线和DC母头转C公头线缆，由于目前市售的不是所有PD充电头都有12V电压输出档位，所以为了不了解自己PD充电头的小伙伴不会因为不知道导致主板烧坏，故不在标配PD诱骗线; DC母头转C口公头，如果您真有需要，后续再找客服补发（需要年底）；
5. **关于退换货：**
   - **不支持7天无理由退换货： 定制产品，烦请谨慎思考后做购买决策；质量问题，随时联系客服处理，无忧售后；**
   - ⚠️**特别注意：拆封后非质量问题不退不货，质量问题，请拍摄长视频且不能压缩画质发送给客服确认问题点；如无法接受前面4点，请不要拆封产品，一经拆封，默认接受定制产品概念和实物的细微调整。**

**未尽事宜，以咨询客服为准。感谢各位等待硬酷R1的各位消费者。**

旺旺：**<small>烦请详细阅读以上信息，并回复「接受」或「不接受」给我们，你也可以直接在快递尚未发出之前，直接申请仅退款申请，感谢。</small>**





### 五、产品支持

##### 1. 售后服务：

因为行业内卷化严重，以及行业内有各种牛鬼蛇神，特做如下说明：

1. 产品未发货前，支持任意理由的退款申请；产品一经拆封，无法支持任何非硬件质量问题的退换货服务；<br> **<small>质量问题不包括：有噪音、有震动、有发热（或发热基于个人原因无法接受）、塞不进弱电箱、机器有灯光、机器上盖非金属材质等<br>质量问题特指（非人为的）：无法开机、网口故障、其他IO口故障等<br>任何售后疑问，以客服沟通为准。</small>**
2. 产品发货后，未拆封包裹之前，无条件支持退货退款申请；
3. 产品拆封后，一律不支持非硬件质量问题的退换货服务（包括人为损坏、人为故障）等，客服有最终解释权。
4. 产品整机质保一年，硬盘质保3年（只换不修）
5. 整机售后服务周期2年，期间超过1年不到2年之内的所有硬件问题，均成本芯片级维修，支持多次售后申请，直到问题解决 **(CPU不挂的前提下，一切硬件问题都不是问题)** ；



##### 2. 产品固件与驱动下载：

###### 固件推荐：

1. OpenWRT固件推荐：[点此前往下载](https://u.iswott.com:8888/ISOs/) 
2.  iKuai固件：[点此前往下载](https://u.iswott.com:8888/ISOs/) 
3. pfsense固件：[点此前往下载](https://u.iswott.com:8888/ISOs/) 
4. OPNsense固件：[点此前往下载](https://u.iswott.com:8888/ISOs/) 
5. Proxmox VE 固件：[点此前往下载](https://u.iswott.com:8888/ISOs/) 
6. VMware ESXi固件[点此前往下载](https://u.iswott.com:8888/ISOs/) 

###### 驱动与BIOS：

1. Intel i226-V驱动：[点此跳转到Github下载](https://github.com/KoolCore/ikoolcore/blob/main/docs/files/Intel%20i226-v%20Driver%20Wired_driver_27.6_x64.zip)
2. BIOS下载：
   - 出厂默认BIOS：[点此前往下载（未放出）]()
   - NVME协议BIOS：[点此前往下载（未放出）]())
   - SATA协议BIOS：[点此前往下载（未放出）]())

3. ##### 出厂默认配置：

   - R1整机 x 1 **<small>CPU型号和板载内存大小因消费者选购不同而有差异</small>**
   - VESA支架 x 1 **<small>支持7 x 7cm 和 10 x 10cm两种尺寸</small>**
   - 12V 2.5A DC转C专用电源 x 1 **<small>专用电源，请勿用于其他设备，其他设备电源也请勿用于R1，烧坏需付费维修</small>**
   - 说明书 x 1 **<small>纸质，中英双语。阅读在线[电子版](https://wiki.ikoolcore.cn/#/)说明书</small>**
   - M.2 2242 NVMe 硬盘 x 1 **<small>仅限选购带硬盘配置订单，未选购硬盘配置不包含</small>**

4. ##### 发货说明：

   - 订单会使用 **菜鸟裹裹商家（可系统自动录入快递单号，加快发货速度）** 物流发出；

   - 包裹和包裹内的机器均会使用防拆封标签， **机器一经拆封，不支持非质量问题的7天无理由退换货申请(这点需要额外注意)** ，介意此条者可于发货前、快递收到但机器未拆封前，申请 **仅退款** 和**退货退款申请** 。感谢理解！*

   - **整机质保一年 （过保成本维修），项目维护3年。**

