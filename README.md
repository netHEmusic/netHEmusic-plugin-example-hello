# netHEmusic 插件示例：Hello

netHEmusic 的示例插件，演示插件 API 的基本用法。

## 安装

**方式一（推荐）**：在 netHEmusic 里打开 **插件 → 插件市场**，找到「Hello 插件（示例）」点安装。

**方式二（手动）**：把 `manifest.json` 和 `main.js` 放进
`%APPDATA%\netHEmusic\plugins\example-hello\`，然后在「插件」页点「重新加载全部」。

## 这个插件做了什么

- 注入一段 CSS，切歌时在屏幕下方弹一条提示带（`ui` 权限）
- 监听 `track` 事件统计切歌次数（`events` 权限）
- 把次数写进插件自己的数据目录（`filesystem` 权限）
- 在设置页加一个开关（`settings` 权限）

## 自己写插件

开发文档见主仓库：[plugins/README.md](https://github.com/Laohehehe/netHEmusic/blob/main/plugins/README.md)

## 上架到插件市场

这个仓库本身就是范例：**根目录有 `manifest.json`，仓库带 `nethe-plugin` 话题**，
主仓库的 Actions 每天会自动把它收进插件市场清单。

## 许可

MIT
