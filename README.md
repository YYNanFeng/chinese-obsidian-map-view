# Chinese Map View for Obsidian

> 🍴 本仓库是 [esm7/obsidian-map-view](https://github.com/esm7/obsidian-map-view) 的 Fork，在原版基础上增加了中国地图支持和完全中文化。通过trae改动。

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/esm7)

一个为 [Obsidian.md](https://obsidian.md/) 提供的**交互式地图插件**，将你的笔记转化为个人地理信息系统（GIS）。

![](docs/img/sample.png)

## 🇨🇳 本 Fork 的改动

相比原版，Chinese Map View 做了以下改动：

### 高德地图支持

- **内置高德地图源**：默认使用高德地图瓦片作为地图底图
- **坐标自动转换**：自动处理 WGS84 到 GCJ-02（火星坐标系）的坐标转换
- **智能检测**：当使用包含"高德"或"autonavi.com"的地图源时自动应用坐标转换
- **完美兼容**：标记、路径、搜索结果、路由等在高德地图上均能正确显示
- **高德"在...中打开"**：默认添加通过高德地图打开位置的操作

### 完全中文化

- **设置界面**：所有设置项名称、描述、按钮全部中文化
- **右键菜单**：地图和编辑器中的右键菜单全部中文化
- **控制面板**：地图视图的控制面板（预设、编辑、链接等）全部中文化
- **对话框**：离线瓦片管理、显示规则编辑器等对话框全部中文化
- **提示信息**：所有 Notice 提示全部中文化

### 默认配置优化

- 默认地图源为高德地图（原版为 CartoDB）
- 已有用户升级时自动添加高德地图源

## 功能介绍

Map View 搜索笔记中的地理位置和路径，将它们放在交互式地图上，并提供丰富的工具：

- 通过搜索、地图、外部地图服务或设备 GPS 添加位置
- 查看 GeoJSON、GPX、KML 和 TCX 格式的路径
- 使用编辑模式在地图上绘制位置和形状
- 计算点之间的路线（驾车、骑行、步行）
- 使用显示规则自定义标记图标、徽章、颜色和路径样式
- 使用布尔查询语言查询和过滤标记
- 在笔记中嵌入实时地图
- 保存地图以供离线使用
- 与 Obsidian Bases 集成

![](docs/img/edit-mode.gif)

## 安装

### 手动安装（推荐）

1. 从 [Releases](https://github.com/YYNanFeng/chinese-obsidian-map-view/releases) 页面下载最新版本
2. 将 `main.js`、`manifest.json` 和 `styles.css` 解压到 Obsidian 库的 `.obsidian/plugins/obsidian-map-view/` 目录下
3. 在 Obsidian 设置中启用 Map View 插件

### 从原版社区插件安装

如果你想使用原版（非中文版），可以在 Obsidian 社区插件商店搜索 **"Map View"** 安装。

## 文档

**完整文档（英文）：** [esm7.github.io/obsidian-map-view](https://esm7.github.io/obsidian-map-view/)

- [快速入门](https://esm7.github.io/obsidian-map-view/quick-start/)
- [位置格式](https://esm7.github.io/obsidian-map-view/location-formats/)
- [查询系统](https://esm7.github.io/obsidian-map-view/queries/)
- [显示规则](https://esm7.github.io/obsidian-map-view/display-rules/)
- [更新日志](https://esm7.github.io/obsidian-map-view/changelog/)

## 致谢

- 原版插件作者 [esm7](https://github.com/esm7)
- 坐标转换算法参考 [geosmart/obsidian-chinese-map-view](https://github.com/geosmart/obsidian-chinese-map-view)

## 支持原版

如果你觉得原版 Map View 有用，请考虑 [请作者喝杯咖啡](https://www.buymeacoffee.com/esm7)。

Bug 和功能请求请提交到 [原版 Issues](https://github.com/esm7/obsidian-map-view/issues)。
