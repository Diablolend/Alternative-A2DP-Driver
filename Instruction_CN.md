## 安装说明

**注意：以下信息仅供参考，可能无法正常工作或存在问题！如遇问题欢迎反馈 Issue。**

**（注意：此操作可能不适用于 Windows 11 24H2。可尝试使用 Windows 测试模式，具体见 DSE-Patcher 相关操作。）**

1. 从提供的压缩包中安装原版程序（AlternativeA2dpSetup-1.6.0.1.msi）。
2. 安装后关闭程序，不要做任何更改。将“crack”文件夹中的内容复制到程序目录（C:\Program Files\Luculent Systems\AltA2DP），并确认替换文件。
3. 运行 DSE-Patcher（如果你的系统版本早于 24H2），并禁用 DSE。
4. 启动 Alternative A2DP Driver，并按照原始手册安装驱动。通过 win+r > devmgmt.msc > 声音，检查驱动是否无误安装。
   - 如果伪签名失败，则每次开机都需要重复此操作。为简化流程，已附带 .bat 文件，但 DSE-Patcher 仍需手动运行。
5. 完成。如果重启后驱动能正常加载，则说明安装成功。祝使用愉快 :)

**注：如果不小心安装了原版驱动，可用如下命令卸载：**  
`pnputil.exe -f -d C:\Windows\System32\DriverStore\FileRepository\alta2dp.inf_amd64_8adcf7b721e1e624\AltA2DP.inf`

alta2dp.inf_amd64_8adcf7b721e1e624 可能与你的不同，请到 `C:\Windows\System32\DriverStore\FileRepository\` 查找你的 alta2dp 文件夹。

**（注：virustotal 或杀毒软件可能会报毒。这是未签名或伪签名应用的常见现象，但也涉及信任问题 :))**
**（注：根据反馈，建议安装 ALT 版本驱动，因为杀毒软件可能会误报并删除驱动文件。）**
