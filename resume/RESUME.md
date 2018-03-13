
# 个人简历

# 联系方式

- 手机：13537550750
- Email：7878906@qq.com 
- QQ：7878906

---

# 个人信息

 - 尹炬/男/1980 
 - 专科/中南大学-计算机应用 （1999-2002）
 - 工作年限：13年
 - 技术博客：http://blog.csdn.net/hero_yin
 - GitHub: http://github.com/heroyin
 - 期望城市：深圳

---

# 工作经历

## 深圳如意通科技有限公司 （2006年9月 ~ 至今 ） 架构师

- 负责团队建设，研发流程设计，从零开始组建了包括服务器端，客户端，测试，美工在内的十余人团队
- 设计开发流程，搭建开发环境，版本控制采用gitlab，ci采用jenkins，项目管理（工单、文档、支持）用redmine
- 为公司翻译了XMPP基础协议RFC6120-6122，部分XEP扩展协议，基于xmpp协议设计的私有扩展协议30余篇
- 基于标准c++开发了xmpp通讯sdk，跨平台设计，可以工作在Windows，Linux，MacOS，Android平台下
- 设计即时通讯服务器架构，采用微服务框架（Spring cloud），Apache Shiro为验证中心，缓存系统采用了redis，通讯服务基于openfire开发，负载均衡使用Ribbon/LVS，Hystrix提供容错支持。建立docker hub私有仓库哦，采用docker统一管理，分发。
- 设计并开发了QT版pc端，基于qml开发，可以运行在Windows，Ubuntu，MacOS，通过引入独立到2D引擎插件解决了在没有OpenGL环境下到兼容问题
- 设计并开发了Android版客户端，采用组件化设计，产品分拆成通讯SDK，界面SDK，可以方便到分拆与客户进行集成开发，从2012年开始涉及Android开发，是最早一批使用Android Studio的用户，在产品里引入了崩溃管理，插件框架，H5轻应用框架，热更新，VOIP等流行技术
- 设计P2P网络，用于客户端VOIP通讯，以及文件传输，设计扩展协议，兼容IMS/SIP通讯，结合opensip/Asterisk，让RTP产品完美对接传统的VIOP业务。

### 如意通项目 
如意通（ http://www.rooyeetone.com ）是一个基于XMPP协议的即时通讯产品，主要面对企业即时通讯市场。我负责协议设计规划，系统研发，以及团队建设，服务器端采用微服务（Spring cloud）架构，有效的管理不同服务，提供稳定，即时，高效的通讯服务。产品成功到应用到了各类公司行业，如：华润集团，美的集团，中国邮储银行等。

### 如意通服务器端

如意通服务器端是以即时通讯为核心的服务平台，在之前的旧版本上做微服务改造。
- 对比了Spring cloud和Dubbo，Spring Cloud的活跃度以及迭代更新速度都远优于Dubbo，最终选用了Spring cloud作为基础架构
- 验证框架，对比了Apache Shiro和Spring Security，由于Apache Shiro更偏向我们的业务场景，最终选择了它作为验证框架。
- 缓存模块，由于之前在IM的很多模块中都使用了redis，所以继承了这个选择
- 在模块划分上，对于提供传统xmpp长连接服务的核心通讯，继续之前的集群方式提供服务，而提供业务需求的REST服务，都转移到为服务的网关（Zuul）调度。

### 如意通Android客户端
如意通Android客户端是一个即时通讯客户端，项目由我带领团队负责设计并开发。我主要负责程序架构设计，核心通讯库开发。
- 引入AOP切面编程模型，有效的拆分了复杂逻辑，降低代码耦合度，由于当时团队成员还不太了解，针对这个情况我写了一些培训文稿。
- 为了解决即时通讯连接响应的问题，优化网络连接，改造DNS解析，最小化通讯进程，优化心跳维持连接，达到迅速建立连接保持通讯的效果。
- 组件化扩展功能，根据客户需求，利用Gradle定制打包，以满足不同的业务需求。
- 利用Nexus搭建包管理，将客户端的核心功能封装成AAR包，提供给客户做二次开发。
- 搭建Gitlab源码管理，通过jenkins自动测试，自动编译，自动发行。

### 如意通PC客户端
如意通PC客户端一个跨平台的架构，采用QT5+QML开发，可以工作在windows、mac和linux等桌面平台上。
- 采用标准C++开发了一个跨平台的XMPP通讯库，再利用QT包装一个用于QML访问的代理模块。
- QML是一个JSON风格的UI描述语言，与JS配合起来和H5有天然的相通，在开发过程中引入了facebook的Flux设计理念，通过单项数据流概念，将View和Data隔离成 Views和Stores，再通过中心Dispatcher来分发Action进行串联，Stores和Views只做单项数据绑定，意味着Views不可以直接修改Stores的数据，而是通过触发Action的方式通知Stores。Views组件变得单一，只负责渲染界面触发Action，从而让程序结构变得更加清晰易于扩展。
 
### 美信项目 
美信（ http://im.midea.com ）是用于美的集团内部的即时通讯产品。我负责和美的内部系统的集成设计，服务器对接，PC端SDK和Android端的架构设计。我带领到4人团队只用了短短月余时间即迅速上线，深得美的员工的喜爱，目前该产品服务于所有美的集团端员工，成了美的员工必备APP。

### 润工作项目
润工作（ http://rwork.crc.com.cn/ ）是华润集团面对内部员工的一站式办公平台。我负责团队协调，以及系统对接，包括统一验证，消息推送融合，以及客户端协同开发，该项目目前服务于华润集团以及旗下的各个分公司的30w员工。

### 广东省广电IMS项目
广电项目中即时通讯是其中的一个增值服务，除了提供基础的即时通讯服务外，需要客户端和IMS对接，为用户提供VOIP服务。我主要负责IMS的客户端（包括PC，Android，IOS）SDK开发，产品成功接入广电IMS网络，实现了与电话，机顶盒，视讯会议等服务的通讯。

---
# 技能清单
- 语言：JAVA/C++/delphi/ruby/javascript/QT
- Android：UI/Gradle/Dalvik/Plugin/Hotfix
- Windows：Win32 API/GDI+/QT/VCL/MFC
- 项目管理工具：Svn/Git/Jira/Confluence/Redmine/Jenkins/gitlab
- 开发工具：AndroidStudio/Eclipse/RubyMine/VisualStudio/Delphi/QtCreator
- 网络协议：TCP/IP/XMPP/HTTP/SIP/STUN
- 安全：TLS/SASL/SQL Injection/ProGuard 
- 操作系统：Windows/linux
