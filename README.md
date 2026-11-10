# Canada Link Windows 测试包

Windows x64 双端代理工程原型，版本 `0.1.0-prototype`。仅供测试，不是已完成真实网络验收的 VPN 成品。

## 下载

打开本仓库中的 `CanadaLink-Windows-v0.1.0-prototype.zip`，选择 **Download raw file** 下载并解压。加拿大电脑不需要安装 Codex。

ZIP 内含 `CanadaLink.exe`、中文说明、测试报告、许可证、完整 Go 源码和测试代码。代理内核不随 ZIP 分发；程序会提示从 SagerNet 官方 GitHub 下载并校验固定版本的 sing-box。

## 测试状态

- 已完成 Go 单元测试、静态检查和 Windows x64 交叉编译。
- 已用官方 Linux 内核检查生成的配置。
- **没有在 Windows 或真实中国至加拿大网络上验证运行、速度、稳定性或防泄漏。**
- 运行级集成测试受执行环境能力限制，未完成。
- Codex 桌面端入口只是环境变量启动试验，不代表全部流量经过代理。

先阅读 ZIP 内 `README-中文.txt` 和 `TEST-REPORT.txt`。如系统安全策略阻止运行，请停止核实，不要关闭杀毒、SmartScreen 或防火墙。

## 安全提醒

此包不包含用户连接配置、真实代理密码、证书私钥或个人资料。使用后生成的 `client-connection.SECRET.json`、服务器私钥、配置和日志不要上传到本仓库。

程序不会自动修改系统代理、路由、DNS、Tailscale 或防火墙。实际部署仍需自行确认两端设备及网络的授权、适用要求与服务条款。

## 校验

`CanadaLink-Windows-v0.1.0-prototype.zip` 的 SHA256：

```
8e14f4db7d63a4a3e655915487cbb74413031c84273bd24f142c23b993080bca
```

源代码许可证见包内 `LICENSE.txt`。单独下载的 sing-box 保留其上游许可证。
