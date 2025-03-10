
## 说明
由于官方开始加入驱动级保护，虽然本工具可以关闭驱动级自我保护，但考虑到公开后可能会被盯上，此项目将会很快废弃，并开发自己的驱动来进行对抗。

## 功能特色
### 本地功能
- **关闭驱动级自我保护**
- **解锁驱动级键盘锁**
- **解锁驱动级USB锁**
- **解锁驱动级网络锁**
- **解锁驱动级文件自我保护**
- **关闭/挂起行为管控和教学进程**
  - 这将不会同步更新行为管控和启动广播进程
  - 绕过软件限制策略
  - 若学生端主进程未退出，关闭这两个进程后会自动重新启动
- **自动窗口注入**
  - 持续检测目标进程是否启动，一旦启动自动注入 DLL
  - 强制将全屏广播转换为窗口广播
- **全局注入窗口广播**
  - 通过注册表特殊项将窗口化 DLL 注入所有新启动的进程
  - DLL 可识别是否为学生端进程，处于安全考虑建议谨慎使用
- **绕过 OSS 验证**
  - 针对机房保护系统
  - 在 OSS 任意工具的登录框打开时运行此功能，可实现任意用户名、密码登录
  - 解锁开机还原等功能

### 远程功能
- **无感崩溃教师端**
  - 崩溃教师端监控线程，使所有学生端画面停止更新
  - 造成整个教室学生端脱控
- **远程控制任意主机**
  - 仅在安装了实验室功能或者OSS的主机上可用
  - 利用 VNC 远程控制任意主机
- **暴力关机**
  - 直接调用系统底层函数强制关机（需要管理员权限）
  - 
## 获取有毒版
影响教学的功能仅限有毒版使用。

如何获取有毒版？
- **联系邮箱** `phtcloud@foxmail.com`，告诉我你的用途。
- **自己破解**：本工具是用 C 语言编写的，未加壳，使用 IDA 进行分析即可破解。

## 免责声明
本工具仅供学习与研究使用，请勿用于任何违法用途。开发者不对任何滥用或非法使用负责任。

