# JDK 下载分享

由于甲骨文官网下载需要账号 所以收集了一些版本的**Windows x64环境**的JDK安装包

毕竟Linux都自带软件仓库 MacOS有HomeBrew

*如果使用IDE 如Intellij Idea开发Java应用程序 那么请在Idea里下载
无需在windows上安装JDK和配置环境变量*

**新手建议下载 Liberica JDK**

# 使用windows应用包管理器 winget 安装jdk（首选）

在win10 21H2 win11下可以通过windows应用包管理器 winget来安装jdk

**使用winget后 基本无需再去各地址下载JDK了**

搜索JDK
```shell
winget search jdk
```
![image](https://user-images.githubusercontent.com/20179864/160649271-31dba968-ef84-4300-a4fc-936b6331c754.png)


然后使用 `winget install [ID]` 命令安装对应ID的JDK即可

# Oracle JDK

如果下载Oracle JDK 那么你需要同意 Oracle [JDK使用协议][1]

[官方下载地址](https://www.oracle.com/java/technologies/javase-downloads.html)

国内下载JDK 如果有你需要的版本 也可以使用 

[华为云JDK镜像][2] 高速下载Oracle JDK

以下是本仓库提供的JDK

[JDK 1.5.22](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.5.22)

[JDK 6u41](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.6.41)

[JDK 6u43](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.6.43)

[JDK 6u45](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.6.45)

[JDK 7u75](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.7.75)

[JDK 7u76](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.7.76)

[JDK 7u79](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.7.79)

[JDK 7u80](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK1.7.80)

[JDK 8u221](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK8.221)

[JDK 8u241](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK8.241)

[JDK 9.0.4](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK9.0.4)

[JDK 10.0.2](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK10.0.2)

[JDK 11.0.1](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK11.0.1)

[JDK 11.0.2](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK11.0.2)

[JDK 11.0.6](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK11.0.6)

[JDK 12.0.2](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK12.0.2)

[JDK 13.0.2](https://github.com/LilithBristol/javajdkforwinx64/releases/tag/JDK13.0.2)

# Liberica JDK

BellSoft提供的OpenJDK版本 
相比于其他OpenJDK分发渠道
Liberica JDK提供了很多便利的特性
- 三种规模的打包版本  
  标准JavaSE的Standard标准版  
  完整包含JavaFX的full全量版  
  精简JDK的Lite版  
- 多种便利的分发渠道  
  包含Liberica JDK的Docker基础镜像  
  Linux仓库  
  支持多种包管理器Swoop,Brew,甚至还有刚推出的winget！  
  RestAPI查询，更新，下载服务支持  
- Windows 安装包自动配置环境变量，并且自动关联jar包  

可以说是对新手最友好的JDK版本
建议现在的Javaer都可以直接使用Liberica JDK

国内直连下载速度很快(AdoptOpenJDK出来挨打) 所以提供链接

[下载Liberica JDK](https://bell-sw.com/)

# Zulu JDK

Azul编译的OpenJDK版本
国内下载速度尚可 所以同样提供链接
相比其他OpenJDK 拥有很全的构建版本
覆盖从Java 6开始到最新的Java18早期预览版  
**如果需要JDK6，JDK7的OpenJDK 可以选择ZuluJDK**
毕竟大部分OpenJDK提供者并没有6,7版本

*但是Azul引以为傲的C4GC并未加入这个免费分发的OpenJDK版本
如果有需要超低暂停的JDK 看看RedHat JDK吧*

[下载Zulu JDK](https://www.azul.com/downloads/zulu-community/?&architecture=x86-64-bit&package=jdk#)

# Adopt OpenJDK

完全社区构建的OpenJDK版本 包含J9和HotSpot两种JVM
提供 8,11 两个长期支持版 和最新版(现在是14)
但是国内下载速度很慢（因为AdoptOpenJDK实际上使用GitHub来分发）

提供链接
[下载 AdoptOpenJDK](https://adoptopenjdk.net/?variant=openjdk8&jvmVariant=hotspot)

20.7.21 清华Tuna镜像已经支持AdoptOpenJDK分发 国内直连可使用此镜像 提供的架构、系统支持非常丰富
包括 linux,mac,win;arch64,arm,ppc,x86

[清华Tuna AdoptOpenJDK镜像](https://mirrors.tuna.tsinghua.edu.cn/AdoptOpenJDK/)


# Amazon Corretto JDK

亚马逊提供的OpenJDK编译版本 目前只提供了 8,11
得益于AWS支持 下载速度超快
而且提供了windows,linux,mac多系统的支持

提供链接
[目录 CorrettoJDK](https://docs.aws.amazon.com/corretto/index.html)

# ReadHat JDK
红帽维护的OpenJDK分发版 仅有windows版 而且还需要登录才能下载  
提供给红帽爱好者  
*红帽维护的OpenJDK在windows平台上支持了ShenandoahGC-新型亚秒级暂停的GC*
(可以使用winget安装 跳过红帽登录)

[ReadHat JDK](https://developers.redhat.com/products/openjdk/download)

[1]:https://www-sites.oracle.com/downloads/licenses/javase-license1.html#licenseContent
[2]:https://repo.huaweicloud.com/java/jdk/


