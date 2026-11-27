# Redmi Watch 6 Weather — Vela Quick App

为 Redmi Watch 6 打造的天气时钟 Vela 快应用：大字时钟 + Open-Meteo 免费天气接口（无需 API Key），城市坐标可改，eSIM 版可独立联网。

**目标设备：Redmi Watch 6（432×514 方屏，designWidth 432）**，同时兼容 Redmi Watch 5 /
小米手表 S 系列等 Xiaomi Vela JS 快应用设备。

## 开发
本项目是标准的 Xiaomi Vela JS 快应用工程（AIoT-IDE / aiot-toolkit）：

```bash
npm install
npm run build     # 构建调试版 rpk
npm run release   # 构建正式版 rpk（需在 sign/ 放自己的签名证书）
```

用 AIoT-IDE 打开本目录即可在模拟器或真机（Redmi Watch 6）上调试；
生成的 `.rpk` 也可通过小米运动健康的开发者模式 / 第三方应用入口安装到手表。

## 目录
```
├── package.json
└── src/
    ├── app.ux            # 应用入口
    ├── manifest.json     # 包名 / 路由 / 系统能力声明
    ├── common/           # 公共脚本
    ├── i18n/             # 多语言
    └── pages/index/      # 主页面 (.ux: template + style + script)
```

## License
MIT
