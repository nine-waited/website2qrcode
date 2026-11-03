# website2qrcode

轻量级「网址 → 二维码」工具：浏览器内生成，可下载 PNG。不在服务端存储内容。

## 在线地址

https://nineee.xyz/website2qrcode/

## 本地打开

直接用浏览器打开 `index.html` 即可（需同目录有 `qrcode.min.js`）。

## 安全校验

- 仅允许 `http://` / `https://`
- 拒绝 `javascript:` / `data:` / `vbscript:` 等危险协议
- 过滤控制字符、零宽字符与 `<>"`\`
- 禁止 URL 内嵌账号密码
- 长度上限 2048；粘贴时自动裁剪

## Nginx 部署

参考仓库内 `nginx.conf`（示例域名 `nineee.xyz`，路由 `/website2qrcode/`）。
