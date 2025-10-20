---
layout: mypost
title: iOS 使用 SideStore 自签
date: 2025-09-23
published: True
categories: iOS
tags: 
 - sidestore
---

## 准备

- WIn10/11 系统桌面

- ≥ iOS 16 苹果设备并开启开发者模式

  > 苹果设备进入 **设置** → **隐私与安全性**→ **开发者模式**，打开并按提示重启，重启再次确认打开

- 系统桌面和平国设备连接到同一局域网

- 美区 AppleID

- 安装 [StosVPN](https://apps.apple.com/us/app/stosvpn/id6744003051)

- 安装 [爱思助手](https://www.i4.cn/)

  

## 安装

1. [点击下载 Side Store](https://github.com/SideStore/SideStore/releases/latest/download/SideStore.ipa)
2. 打开爱思助手，使用数据线连接苹果设备和电脑并在苹果设备上确认

3. 爱思助手切换到 **工具箱** 菜单，找到高级工具下的 **IPA 文件签名** 点击进入

4. 点击 **添加 IPA 文件**，选择下载的 `SideStore.ipa` 文件

5. 点击 **Apple ID 签名** → **添加 ID**，输入 Apple ID 和登录密码点击确定，注意要和苹果设备登录AppleID的一致

6. 勾选添加的 ipa 文件和 Apple ID 后点击 **立即签名**

7. 签名完成后关闭小窗，点击⬇进入下载中心，点击应用安装，安装应用

8. 安装完成后，苹果设备进入 **设置** → **通用** →  **VPN 与设备管理**，找到证书（显示为你的 Apple ID)，点击信任




## 配对

1. [点击下载 JitterBugPair 并解压缩](https://github.com/osy/Jitterbug/releases/latest/download/jitterbugpair-win64.zip)	

2. 确保苹果设备解锁，然后在解压缩目录顶部输入cmd并回车打开终端

3. 在终端中输入 j 并按 Tab 键补全后回车，出现 Success 表示成功在解压缩目录中生成配对文件

4. 使用局域网传输工具将配对文件下载到苹果设备，这里提供一个临时文件中转站：[FF2A FILE](https://file.ff2a.com)，建议使用Edge浏览器下载

5. 打开 SideStore，根据提示打开配对文件，如果使用Edge下载，文件位于 /Edge/Download

6. 在 SideStore 中登录 Apple ID 后就可以在 My Apps 刷新证书了，注意刷新前连接 WIFI 并打开 StosVPN 否则会失败

7. 注意更新或重置苹果设备后需要重新配对




## 插件

1. [点击下载 LiveContainer](https://github.com/LiveContainer/LiveContainer/releases/latest/download/LiveContainer.ipa)
2. 在 SideStore 中点击 My Apps，然后点击左上角 +，打开下载的 IPA 安装，注意安装前连接 WIFI 并打开 StosVPN 否则会失败

3. 安装完成后打开 LiveContariner，点击 设置，点击 **从 SiderStore 导入证书**

4. 导入证书成功后，点击 App 再点击左上角 + 安装应用



## 快捷指令

[点击链接](https://www.icloud.com/shortcuts/7f5c54917b814bc1a3cced41ccfe7268) 获取快捷指令并可自行添加到主屏幕

推荐添加自动化在特定时间自动执行




## 参考链接

- [iOS 侧载新选择！SideStore + LiveContainer，纯净无广，无限安装软件！！！](https://blog.mcxiaochen.top/posts/p5a0d/)