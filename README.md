# TVBox WebDAV 运行库

公开下载的不含账号、密码或个人配置的 Android DEX JAR。支持 `csp_WebDav` 直连 HTTPS WebDAV 和 `csp_Jiaofu`。

TVBox 导入手机自己的私有 JSON，JSON 中的 `spider` 指向本仓库的 JAR 下载地址。WebDAV 专用凭据只存放在手机私有 JSON，勿提交到此仓库。

Android API 21+，需要宿主提供 Java Spider、OkHttp 3.x 和 Okio 1.x。网盘源只读现有视频，不创建磁力任务，不需要电脑服务。

版本 v1.0.0：目录列表、中文编码、自然集数排序、子文件夹分组、临时播放链接和直接视频鉴权。已通过 JVM 模拟接口测试及真实 WebDAV 目录/播放链接解析检查；Android 真机最终播放仍需验证。

JAR 下载：[v1.0.0](https://github.com/sss23457/tvbox-webdav-runtime/releases/download/v1.0.0/tvbox.jar)

校验见 `SHA256SUMS.txt`。
