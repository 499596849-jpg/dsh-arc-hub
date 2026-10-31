# dsh-arc-hub · 弧梦数字中枢 DSH 插件

把「弧梦数字中枢 / 海拉」接入 DeepSeek Harness：
- Host 工具：rc_hub_status / rc_hub_persona（只给摘要）/ rc_hub_mode / rc_hub_search / rc_hub_open_dir + 常驻锚点卡
- Client：设置页「弧梦中枢」+ 右下角数字中枢圆（粒子环绕，点击打开中枢）
- 人设卡支持加密读取（AES-256-GCM + Windows DPAPI）

## 安装

在 DSH 插件管理里「添加插件」粘贴本仓库地址，或本地安装：

``
plugin_manager(action:"install_bundle", target:"https://github.com/<你的用户名>/dsh-arc-hub")
``

装完**重启一次 DSH**，右下角出现中枢圆、设置里出现「弧梦中枢」。

## 依赖

需要先安装主程序 ArcDream Hub（提供 127.0.0.1:8799 服务）。默认数据目录 %LOCALAPPDATA%\ArcDreamHub；自定义过数据目录的话，设置环境变量 ARC_HUB_ROOT 指向它。

## License

MIT
