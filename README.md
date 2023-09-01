# RedmiBookPro2022-Ryzen-Hackintosh-EFI
Redmi Book 2022 锐龙版（AMD Ryzen R5 6600H/R7 6800H）的 OpenCore 黑苹果 EFI，提前说一下，非常不完美！！

OpenCore 版本 0.9.4，理论上 macOS 10.15 Catalina+ 均可运行，实测 macOS 10.15 Catalina 与 macOS 13.6 Ventura 可以运行。

### 电脑配置

CPU：AMD Ryzen R5 6600H/R7 6800H

内存：16GB

硬盘：FORESEE XP2000F 512G

显卡：AMD Raedon Graphics

声卡：Conexant Senary Audio（Codec CX8070）

网卡（Wi-Fi）：MediaTek MT8721

键盘：PS/2

触控板：I2C HID

摄像头：USB

### 已驱动

- CPU、内存、硬盘等基本设备
- 键盘（有一定问题）
- 声卡（Conexant CX8070）
- 摄像头

### 未驱动

- 显卡（CPU 的核显，AMD Raedon Graphics）的绝大部分功能。由于 AMD CPU 没有被 Apple 官方使用过，AMD 核显完全无解。
- 网卡，可使用 USB 无线网卡或 USB 转网线接口修复。
- 蓝牙
- 麦克风（但是扬声器可以正常使用）
- 触控板
- 屏幕亮度控制（由于显卡的关系）
- iCloud（但是 Mac App Store 可用）
- 指纹

### 未知

- HDMI 接口
- 3.5mm 耳机孔
- 睡眠（macOS 在长时间不用时自动锁定电脑并黑屏，我不知道这算不算睡眠）

### 已知 Bug

- 一触碰触控板时，键盘失灵，重启恢复
- 启动时会有随机内核崩溃（卡在 EBLOG EXITBS START），可能原因是关于 NVRAM，但无法确定。
- 偶尔在键盘上输入一个键时，会自动开始连打，重启恢复。
- 还有 AMD CPU 黑苹果正常的所有 Bug

### 说明

在很多教程中都明文说明了 AMD 笔记本不能安装黑苹果。本 EFI 虽然可以帮助你安装，但是不用说问题也很多，且修复难度极大，所以作者已基本放弃维护。如果有大佬修复成功了，可以在 Issue 里报个喜，万分感谢（T_T）

另外，本 EFI 由于问题很多，仅供尝鲜，千万别想拿它当主力系统用（T_T）

