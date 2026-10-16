# TVBox WebDAV 运行库

公开发布不含账号、密码或私人配置的 Android DEX JAR 与在线配置入口。

## 在线配置（v1.0.1）

在 TVBox 配置地址填写：

```text
https://sss23457.github.io/tvbox-webdav-runtime/tvbox.json
```

加载后选择「WebDAV 网盘（直连）」→「配置 WebDAV 连接」，在 TVBox 原生窗口填写 WebDAV HTTPS 地址、专用用户名、专用密码和根目录。保存后返回「WebDAV 视频」分类刷新。凭据只保存在该手机应用自己的存储中，不上传到 GitHub；后续可从「设置 WebDAV」分类修改。

不需要在手机放置本地 JSON 文件，也不需要电脑服务。原有私有 JSON 方式仍受支持。

备用入口（内容相同，JAR 同样走对应域名）：

- Raw：https://raw.githubusercontent.com/sss23457/tvbox-webdav-runtime/main/tvbox-raw.json
- CDN：https://cdn.jsdelivr.net/gh/sss23457/tvbox-webdav-runtime@main/tvbox-cdn.json

Android API 21+，需要宿主提供 Java Spider、OkHttp 3.x 和 Okio 1.x。支持 `csp_WebDav` 和 `csp_Jiaofu`。网盘源只读取现有视频，磁力需先在网盘应用转存。

已通过 JVM 模拟接口测试，覆盖未配置时的入口和非空详情；真实 WebDAV 目录和播放链接解析已通过。原生设置弹窗及最终播放仍需当前 TVBox APK 真机验证。校验见 SHA256SUMS.txt。
