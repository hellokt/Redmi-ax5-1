# 欢迎来到 适用于 IPQ807x||IPQ60xx||MT798X 设备的 Openwrt 编译仓库

# rm1800&ax5 固件[下载](https://github.com/breeze303/Redmi-ax5/releases)

## 云编译使用方法点击[链接](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

## ipq6000仓库更新日志：  
08.19更新日志：  
1.ssr-plus更新到最新版。  
2.添加了自动重启app，定时重启能提高使用体验，  
3.去掉了turboacc中的bbr加速状态，kernel 4.4不支持bbr加速。  

08.24更新日志：  
1.解锁网易云音乐使用go版本，节约内存，  
2.修复turboacc开启dns缓存再关闭之后dns解析不正常的问题，  
3.加入nsscrypto模块，或许对于某些软件的加解密过程有些作用。  

09.20更新日志：  
1.插件更新。  
2.最大连接数增加到65535。  

09.23更新日志：  
1.同步上游最新更新。  
2.cpu超频到1.8ghz。  

10.03更新日志：  
1.优化超频选项，根据跑分结果选定三档频率，1.0-1.4ghz。  
2.优化nss失效状态下的网络性能。  

10.14更新日志：  
1.源码还原部分默认设置。  
2.和目ax18固件精简版和完全版双版本更新。  
3.重构云编译脚本仓库，提升可读性。  
4.添加nss状态显示。  

10.16更新日志：  
1.更优雅的解决的端口回环设置失效的问题。  
2.简化云编译.config文件，方便二次修改。

10.20更新日志：  
1.梳理dnsmasq相关代码，修复bug。  
2.默认关闭“过滤ipv6 dns解析”。  
3.openssl升级到q版本。  

11.11更新日志：  
1.cpu频率开放更多挡位，0.8~1.8g。  
2.云编译添加红米ax6支持。

12.01更新日志：  
1.云编译添加了360t7设备支持。  
2.云编译添加了红米ax6000设备支持。  

12.25更新日志  
1.支持opkg在线安装软件。  
2.删除部分不必要改动。  
3.luci package仓库更新。  

01.10更新日志  
请fork的ipq6000库的及时更新到r23.01.10版本。  
r22.12.25存在几个有bug的阶段。

02.01更新日志：  
1.同步openwrt-19.07稳定分支代码。  
2.释放wifi部分的保留内存，可用内存增加51mb，现在开机约有140mb可用内存。  
3.ipq6000仓库新增了wifi分支，恢复wifi并为和目ax18设备增加专门的bdf，效果有待测试。（该分支不包含.2提到的更新。）  
4.一些插件的更新。例如，修复msd_lite播放4k源丢包的问题。  
5.一些不重要的更新。例如，删除了1.8g这个虚假的频率。360v6现在恢复原本的qihoo_v6设备名称，uboot下刷机或者ssh下使用sysupgrade -F命令升级。  

02.14更新日志：  
1.redmi_ax6改用patch的形式添加设备支持，不再需要手动维护。  
2.ssr-plus插件，trojan增加支持识别链接是否允许 “allowInsecure”。（only ipq6000）  
3.原ipq6000仓库改名ipq6018并不再更新。新仓库依然叫ipq6000。  
4.更新GitHub Actions output函数。  
