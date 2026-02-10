# Clash Editor

一个可视化的 Clash Verge 节点配置编辑器，纯前端单文件，浏览器直接打开即可使用。

## 功能

- **导入配置** — 粘贴 YAML 文本、上传 `.yaml` 文件、或从零开始
- **粘贴链接添加节点** — 支持 `ss://` `vmess://` `vless://` `trojan://` `hysteria2://` `hy2://`，批量多行识别
- **机场订阅管理** — 添加 proxy-provider 订阅源，可选自动更新，支持被代理组 use 引用
- **节点卡片展示** — 网格布局，彩色边框区分协议类型
- **手动添加/编辑节点** — 表单式 UI，按类型动态字段，高级选项可折叠
- **代理组管理** — 新建/删除代理组、添加/移除成员、嵌套分组
- **导出配置** — 下载完整 `.yaml` 文件，原有 dns/rules 等配置原样保留，支持预览和一键复制

## 使用方式

1. 下载 `index.html`
2. 用浏览器直接打开
3. 开始编辑你的 Clash 配置

或者访问在线版本：https://korelyk.github.io/clash-editor/

## 技术细节

- 单文件 HTML，无需安装任何依赖
- 唯一外部依赖：[js-yaml 4.1.0](https://github.com/nodeca/js-yaml)（CDN 加载）
- 中文界面，暗色主题
- 所有数据仅在浏览器本地处理，不会发送到任何服务器

## 支持的协议

| 协议 | 链接解析 | 手动编辑 |
|------|---------|---------|
| Shadowsocks (SS) | SIP002 + 旧格式 | 完整字段 |
| VMess | Base64 JSON | 完整字段 |
| VLESS | URI 格式 (含 Reality) | 完整字段 |
| Trojan | URI 格式 | 完整字段 |
| Hysteria2 | URI 格式 | 完整字段 |

## 截图

打开 `index.html` 即可看到编辑器界面。

## License

MIT
