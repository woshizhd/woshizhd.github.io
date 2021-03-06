---
layout:     post
title:      计算机网络发展史
subtitle:   从学习HCNA，再到学习HCIP，知识量不断增加，知识的理解却很浅薄。亟需梳理总结，弄懂基础网络知识的原理和由来
date:       2020-04-23
author:     Hank Z
header-img: img/home.jpg
catalog: true
tags:
    - 计算机网络
---

# 说明
- 这里的计算机网络 = 互联网 = internet
- 不断地追问，是此文的逻辑所在。在理解逻辑的同时，不要忘了探索那些宝贵的外链，在那里可以获取到更多的知识。
- 交流可以联系 zhd088@163.com

# 行文思路
- 九层高台，起于垒土；合抱之木，始于毫末。复杂的事物由简单组成，所以本文会从计算机网络最简单的结构出发，逐步演进到现代大规模应用的场景。

## 1. 什么是计算机网络？
个人较认同 IEEE [Tanenbaum 的定义](http://www.kfu.edu.cn/__local/5/12/31/621F7BE0D8218174C76EE8362BB_39A50BBC_39C6AC.pdf)
> “计算机网络是一组自治计算机互连的集合”
- 自治是指每个计算机都有自主权，不受别人控制
- 互连则是指使用通信介质进行计算机连接，并达到相互通信的目的

## 2. 那什么是计算机？
#### 上文计算机网络定义中的计算机，更精准地说，应该是电子计算机。详细定义参考：[电子计算机-wiki](https://zh.wikipedia.org/wiki/%E7%94%B5%E5%AD%90%E8%AE%A1%E7%AE%97%E6%9C%BA)
#### 计算机的几个关键发展阶段。详细发展过程参考：[计算机发展编年史](https://wenku.baidu.com/view/a39f83126bd97f192279e9a5.html) [计算机发展阶段-布衣码农](https://www.cnblogs.com/noteless/p/9242963.html)
- 机械时代：1623——1895
- 电子管时代：1911——1946
- 晶体管时代：1947——1958
- 集成电路时代：1959——1970
- 超大规模集成电路时代：1971——至今

## 3. 计算机如何互连？
#### 前期工作
- 能源支持——电
	- 详细内容参考：[《电的科学史》](https://book.douban.com/subject/30147046/)
	> 部分摘抄：“第二块基石是在这一伟大科学的基础上取得的技术进步。人类历尽艰辛，终于在电与磁之间建立了联系，Samuel Morse 发明的电报是电磁学的第一个成果。电报的产生是为了交流，这一点很重要。电力业务和电信业务都是同一学科的产物，但是后者在现代技术进步中的发展速度远远超过前者。”
- 垫脚石——已有的通信工具
	- 电报
	- 电话
	- 了解更多，参考：[通讯编年史](https://u.nu/pyi66)
- 几个重要的理论
	- 1820年，奥特斯发表论文向学术界宣告了电流磁效应的诞生
	- 1864年，麦克斯韦将电流磁效应完善并且建立了电磁理论系统
	- 1948年，香农提出信息论。[详细内容参考](https://u.nu/uw2dh)

#### 计算机的灵魂——编程语言
- 详细定义参考：[编程语言-baike](https://baike.baidu.com/item/%E7%BC%96%E7%A8%8B%E8%AF%AD%E8%A8%80)
- 编程语言的发展，参考：[编程语言编年史](https://www.omegaxyz.com/2018/01/24/programmla_his/)

#### 计算机的血肉——操作系统	
- 操作系统的定义和发展，参考：[操作系统-wiki](https://zh.wikipedia.org/wiki/%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F)

#### 计算机的躯干——硬件
- CPU
- Memory
- 存储硬盘
- 显卡
- 电源
- 输入／输出
- 主板（motherboard）	
- 了解更多，参考：[电脑基础知识](https://github.com/woshizhd/pc)

#### 计算机互连的演进 = 计算机网络的发展史。铺垫了这么多，终于到讲到题目了，所以另立章节，给予充分的尊重！
> 如需了解详细互联网的编年史，可参考：[互联网发展史-baike](https://baike.baidu.com/item/%E4%BA%92%E8%81%94%E7%BD%91%E5%8F%91%E5%B1%95%E5%8F%B2/4635625)

## 4. 计算机互连的演进／计算机网络的几个发展阶段
#### 主机直接互连
![host to host](https://tva1.sinaimg.cn/large/007S8ZIlly1ged0t080q7j30ii04m74e.jpg)
- 重要事件
	- 1965年 MIT林肯实验室的TX-2计算机与位于加州圣莫尼卡的系统开发公司的Q-32计算机通过1200bps的电话专线直接连接(没有使用包交换)。随后ARPA又将数据设备公司(DEC)的计算机加入其中，组成了实验网络

	> 值得注意的是。1965年，美国贝尔成功生产了世界上第一台商用存储程式控制交换机（也就是“程控交换机”），型号为No.1 ESS（Electronic Switching System）。这种程控式交换机被用于电话交换，后期 ARPANET 的主机互连正是借鉴了这种交换思想。

#### 早期的 ARPANET ————主机互连时代
![arpanet_april1971_large](https://tva1.sinaimg.cn/large/007S8ZIlly1ged1020e3og318m0u0wf6.gif)
- 重要事件
	- 1969年，ARPANET的首四個節點經已用電路連接，其速度為50kbit/s，在加利福尼亚大学洛杉矶分校、斯坦福大學研究中心、加利福尼亞大學聖塔芭芭拉分校、犹他大学這四個地點之間建立網絡。在分组交换網絡的理論中做出許多傑出貢獻的伦纳德·克莱因罗克協助了ARPANET的研發
- **特点**
	- 去中心化的分布式网络
	- 采用接口消息处理器IMP建立节点
	- 采用分组交换技术，详细内容参考：[分组交换-baike](https://baike.baidu.com/item/%E5%88%86%E7%BB%84%E4%BA%A4%E6%8D%A2)
	- 互连的电脑可以兼容，而实际情况是当时的大部分电脑相互之间不兼容（各大厂商间并没有共同遵守的约定）
- 通信应用
	- 1971年，ARPANET 已經連接了包含哈佛大學與麻省理工學院等四十多個學校、軍方及政府機構單位，並制定出遠程終端模擬 (Telnet) 與檔案傳輸 (FTP) 方法。
	- 1971年，BBN的Ray Tomlinson发明了通过分布式网络发送消息的email程序。最初的程序由两部分构成：同一机器内部的email程序(SENDMSG)和一个实验性的文件传输程序(CPYNET)。

#### ARPANET 采用 TCP/IP 协议————局域网时代
![bridgeprinciples](https://tva1.sinaimg.cn/large/007S8ZIlly1ged6xk5jhmj311a0qqtak.jpg)
- 重要事件
	- 1973年 Harvard大学Bob Metcalfe的博士论文首先提出了以太网的概念
	- 1974年，瑟夫與康恩 (Bob Kahn) 提出 TCP/IP 通訊協定 (Transmission Control Protocol/Internet Protocol) ， 解決了跨越不同電腦系統連接的問題
	- 1982年，Xerox與DEC及Intel組成DIX聯盟，並共同發表了Ethernet Version 2（EV2）的規格，並將它投入商場市場，且被普遍使用。而EV2的網絡就是目前受IEEE承認的10BASE5。了解更多，参考：[以太网-wiki](https://zh.wikipedia.org/wiki/%E4%BB%A5%E5%A4%AA%E7%BD%91)
	- 1983年1月1日，ARPANET从NCP协议切换为TCP/IP协议。运行较长时期曾被人们习惯了的NCP被停止使用，TCP/IP协议作为因特网上所有主机间的共同协议，从此以后被作为一种必须遵守的规则被肯定和应用
- **特点**
	- 个人PC普及，商业计算的复杂性要求大量终端设备的资源共享和协同操作。中继器、集线器、网桥应用到网络中，用来扩大网络连接距离和增加终端数量
	- 不再使用Honeywell或者多总线(Pluribus)IMP，TIP被TAC(terminal access controller，终端访问控制机)代替
	- 开始出现工作站，它们大多使用包含有IP网络协议的Berkeley Unix(4.2 BSD)操作系统
	- 连网需求从每个节点单独的大型分时计算机系统与Internet相连转为将一个局域网络与Internet相连
- 通信应用
	- 1976年，AT&T的Bell实验室开发了UUCP(Unix到Unix文件拷贝)，并于第二年同UNIX一同发行。
	- 1979年，Tom Truscott和Steve Bellovin使用UUCP协议建立了连接Duke大学和UNC的USENET，最初USENET只包括net.*新闻组。
	- 1980年10月27日，由于一种状态信息病毒出人意料的自我繁殖，ARPANET完全停止运行。
	- 1982年，外部网关协议(EGP，RFC 827)，EGP用于网络间的网关。


	
#### NSFnet 取代 ARPANET————早期互联网时代
![internet1](https://tva1.sinaimg.cn/large/007S8ZIlly1ged7dyyuj0j30xc0iiabe.jpg)
- 重要事件
	- 1984年，一个来自斯坦福大学的Leonard Bosack和Sandy Lerner教师夫妇在美国硅谷的圣何塞成立了一家名为思科(Cisco)的电子公司，他们设计了一种名为“多协议路由器(Access Gateway Server)”的联网设备，可以使斯坦福大学中不兼容的计算机网络连在一起。这就是如今被喻为网络里程碑的宽带路由器(Router)的前身。了解更多，参考：[路由器的诞生背景](https://u.nu/pwaeb)  [路由器的发展](https://u.nu/cwg3m)
	- 1986年，NSFnet建成(主干网速率为56K bps)。NSF在美国建立了五个超级计算中心，为所有用户提供强大的计算能力。(Princeton的JVNC，Pittsburgh的PSC，UCSD的SDSC，UIUC的NCSA，Cornell的Theory Center)这掀起了一个与Internet连接的高潮，尤其是各大学。
	- 1990年，ARPANET停止运营。世界在线(world.std.com)成为第一个Internet电话拨号接入服务提供商。
	- 1990年 ，Kalpana 公司（1994年被思科收购）发售世界上第一台交换式集线器 EtherSwitch
- **特点**
	- 以太网和路由器逐渐发展成熟，成为主流
	- TCP/IP 技术广泛运用，成为全球标准
- 通信应用
	- 1983年域名（domain name）系統的概念被提出。「.com」、「.gov」、「.edu」等字尾在一年後出現。
	- 1984 引入名字服务器系统(DNS)。
	- 1987年，在德国和中国间采用CSNET协议建立了email连接，9月20日从中国发出了第一封信。
	- 1988年，Jarkko Oikarinen开发了Internet网上聊天(IRC)。
	- 1988 11月2日 - Internet蠕虫在Internet上蔓延，全部60,000个节点中的大约6,000个节点受到影响。
	- 1990年在瑞士粒子物理實驗室(European Particle Physics Laboratory, CERN)英國的伯納斯李 Berners Lee。 Berners成功的提出與開發了全球資訊網(World Wide Web)，被稱為「WWW之父」。
	- 1993年2月，美國國家高速電腦中心針對Unix系統研發出 Mosaic 浏览器，它是第一套利用GUI (Graphical User Interface)介面程式，可以簡單讀取網頁上的圖文資料，將圖跟文 展現在螢幕上。
	- 1994年，诞生网上购物、网上银行，电台开始在网上提供不间断摇滚乐广播

#### ISP（Internet Service Provider） 兴起————现代互联网时代
![internet2](https://tva1.sinaimg.cn/large/007S8ZIlly1ged79i7a36j30u012ath8.jpg)
- 重要事件
	- 1995年 NSFNET恢复成为学术网络，美国大部分的主干网业务由互联的网络服务提供商办理。
- **特点**
	- ISP 的商业化模式促进全球网络互通，用户激增下 internet 获得了高速发展
	- 便携式计算机普及、操作系统成熟、各类网络服务涌现
	- 移动电话（手机）兴起，迎来移动互联网的浪潮
- 通信应用
	- 1995年，微软提供視窗95給軟體設計業者，視窗95協助建立了開發網際網路軟體的普遍標準，掀起許多創意人投入網際網路發展的浪潮。
	- 1996年，WWW浏览器之间的战争爆发，主要是在Netscape和Microsoft之间展开，这带来了软件开发的新时代，如今Internet用户急于测试即将发布的软件，使得每个季度都有新版软件发布。
	- 1998年，Google 成立，搜索引擎开始迅速发展。
	- 1999年，Blog 兴起，Blogger 是最早的Blog。到2005年，這股熱潮席捲全球，幾乎達到顛峰。
	- 2003年8月，詹士莊(Niklas Zennstrom)於盧森堡創立 Skype，這種利用P2P的軟體技術開發出的語音傳輸服務，衝擊傳統電信業者，卻造福了無數的電話用戶。
	- 2004年，Facebook 诞生。
	- 2005年2月，YouTube 成立。
	- 2005年5月，Google 率先推出其線上地圖搜尋服務—「Google Maps」。


## one more thing 想了解更多，可以参考以下资料

- 荐书：[图解网络硬件/HTTP/TCP/IP 三部曲](https://book.douban.com/subject/30564649/)
- 网络厂商资料：[https://github.com/woshizhd/cto](https://github.com/woshizhd/cto)
 