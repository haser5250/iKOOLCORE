1. **硬件配置如何？**

   | 参数 | 信息                                                         |
   | :--- | :----------------------------------------------------------- |
   | CPU  | 赛扬N5105、奔腾N6005                                         |
   | 内存 | 板载设计，双LPDDR4 4200颗粒（跑在2933），双通道，使用三星/海力士颗粒 |
   | 网卡 | 4 x Intel i226-v `优于i225-v`  （ `PVE` 原生支持，`ESXi` 已有社区驱动支持） |
   | 硬盘 | M.2接口，2242尺寸规格，`NVMe` 或 `SATA` 协议，二选一 `选择后无法支持另外一种协议` 。 |
   | 显示 | HDMI 2.0 4K60Hz视频输出                                      |
   | USB  | USB 3.1 Gen1 x 2; USB-C 3.1 Gen1 x 1; TF Card x 1            |
   | 散热 | 主动散热 （均热板+主动散热风扇）                             |
   | 供电 | USB-C接口供电 12V2A或12V3A <br>   <small>**(标配PD诱骗线，可使用PD充电头配合诱骗线供电 ;标配DC母转C公直通线，可以使用DC 12V电源供电)**</small> |
   | 尺寸 | 75 x 75 x 48 mm                                              |

2. **产品外观：**
   ![](https://wiki.ikoolcore.cn/images/mul_banner.png)

3. **产品售价**

    |   CPU   | 内存大小<br> `板载，双颗粒双通道，不可升级` | 硬盘大小<br> `SATA协议`或 `NVMe协议 二选一` |  价格  |                           购买链接                           |
       | :-----: | :-----------------------------------------: | :-----------------------------------------: | :----: | :----------------------------------------------------------: |
       |  N5105  |                     8GB                     |                   `不带`                    | ￥999  | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                    16GB                     |                   `不带`                    | ￥1299 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                                             |                                             |        |                                                              |
       |  N5105  |                     8GB                     |                    128GB                    | ￥1199 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                                             |                                             |        |                                                              |
       |  N5105  |                    16GB                     |                    512GB                    | ￥1799 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                                             |                                             |        |                                                              |
       | `N6005` |                     8GB                     |                   `不带`                    | ￥1199 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                    16GB                     |                   `不带`                    | ￥1499 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                                             |                                             |        |                                                              |
       |  N6005  |                     8GB                     |                    128GB                    | ￥1399 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |
       |         |                                             |                                             |        |                                                              |
       |  N6005  |                    16GB                     |                    512GB                    | ￥1999 | [![](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E8%B4%AD%E4%B9%B0-%E6%B7%98%E5%AE%9D-red)](https://item.taobao.com/item.htm?ft=t&id=682025492099) |


4. 带配置的硬盘是啥牌子？啥主控？啥颗粒？

   **<small>OEM定制的NVMe和SATA固态硬盘 </small>** ， 主控信息如下：<br>

   - NVMe主控：联芸(Maxio)科技 **MAP1202A-F1C  <small>(以128G为例，其他容量主控可能有变化) </small>** ，使用此款芯片的市售产品有： [海康威视CC500](https://zhuanlan.zhihu.com/p/394138333) 、[Lexar雷克沙NM610PRO](https://diy.pconline.com.cn/1535/15359085.html) 、[致态TiPlus5000](https://www.chongdiantou.com/archives/137851.html) 
   - SATA主控：联芸(Maxio)科技 **MAS1102B-B1C <small>(以128G为例，其他容量主控可能有变化) </small>**   ；
   - 颗粒：长江存储
   - 保修政策： **3年只换不修**
   - 硬盘标签纸：
     ![](..\images\SSD.jpg)

5. **散热如何？**
   **<small>主动散热设计，采用均热板和主动散热风扇结合的散热方式;单纯不讲负载，不说环境温度，聊发热/散热也是耍流氓。日常纯物理OpenWRT下，主动散热加持下，大部分地区（地区不同，环境气温不同）不会超过50度。作为体积极致小巧的机器，在产品品质层面，我们能做到的是高负载带来高发热的情况下，即使CPU温度超过70降频了，也不会死机，这个是产品质量底线;（注意测试样品CPU为N5100，TDP 6W， 相同条件下N5105预计温度会高一些。）</small> ** 。  压测信息如下截图：
   ![](https://wiki.ikoolcore.cn/images/weather_temp.jpg)
   ![](https://wiki.ikoolcore.cn/images/limited.jpg)

6. **产品扩展性如何？可以内置硬盘吗？**
   **<small>产品没有任何扩展性可言。如果您考虑扩展做存储设备，可以考虑其他产品。产品目前只有一个M.2硬盘位，无SATA位，无蓝牙位，无网卡位。只有两个外置USB3接口，一个USB C口。</small>**

7. **发货时间？**
   **<small>目前已经在积极量产中，受9月初深圳疫情封城一周，外加之前没有把国庆假期的时间考虑进去，比原来预期的9月28日-10月18日发货的时候，推迟2周左右，目前最新的发货时间为：10月18日至11月08日； </small>** **疫情严峻形势下，变数和不可控因素较多，烦请各位已经上车小伙伴理解 (理解万岁)！**

