# GoHome

<img alt="GoHome 演示图" src="https://github.com/user-attachments/assets/26d12e76-d5c2-4c9c-9c4b-42c66dea7553" />

这是一个可以运行在 **小米手环9 Pro** 上的放假倒计时快应用。你可以通过这个应用，查看还有多长时间放假。在快应用中，你可以随时编辑放假时间，一键保存。

我们在2025年8月8日发布了2.0.1版本，如果您需要旧版本，请到release下载。

请到米坛社区查看详情：https://www.bandbbs.cn/resources/2873

## 如何构建

请阅读 Xiaomi Vela JS 的[应用开发文档](https://iot.mi.com/vela/quickapp/zh/guide/)。

本程序在打包时会将JS转换为JSC（`--enable-jsc`），你需要保证项目所在文件夹的**路径不包含特殊字符**（包括汉字）。

由于AIoT新版本特性，如果你尝试在 Redmi Watch 4 之类的低Vela版本上运行本程序，请手动指定`designWidth`，详见[开发文档](https://iot.mi.com/vela/quickapp/zh/guide/framework/style/page-style-and-layout.html#px)：

https://github.com/yzl3014/GoHome/blob/69f7be9c75a1d6c506e0d946f73171d16388aef8/src/manifest.json#L24
