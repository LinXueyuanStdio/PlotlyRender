# PlotlyRender

> 🎨 一个基于 Plotly.js 的在线 JSON 数据可视化工具

## 📖 项目简介

PlotlyRender 是一个简单易用的在线数据可视化工具，允许用户通过输入 JSON 格式的数据来快速生成各种类型的图表。该工具基于强大的 Plotly.js 库构建，提供了丰富的图表类型和交互功能。

## ✨ 主要特性

- 🎯 **即时渲染**：输入 JSON 数据，一键生成图表
- 📊 **多种图表类型**：支持折线图、柱状图、饼图、散点图等
- 🎨 **现代化界面**：采用 Tailwind CSS 构建的美观响应式界面
- 💾 **图表导出**：支持导出 PNG 和 SVG 格式
- 🔧 **实时验证**：JSON 格式实时校验和错误提示
- 📱 **响应式设计**：完美适配桌面和移动设备
- 🚀 **快速示例**：内置多个示例数据，快速上手

## 🛠️ 技术栈

- **前端框架**：原生 HTML/CSS/JavaScript
- **图表库**：[Plotly.js](https://plotly.com/javascript/)
- **样式框架**：[Tailwind CSS](https://tailwindcss.com/)
- **字体图标**：[Font Awesome](https://fontawesome.com/)
- **字体**：[Inter](https://rsms.me/inter/)

## 🚀 快速开始

### 在线使用

直接在浏览器中打开 `index.html` 文件即可使用。

### 本地运行

1. 克隆项目到本地：
```bash
git clone https://github.com/LinXueyuanStdio/PlotlyRender.git
cd PlotlyRender
```

2. 直接用浏览器打开 `index.html` 文件，或使用本地服务器：
```bash
# 使用 Python 3
python -m http.server 8000

# 使用 Python 2
python -m SimpleHTTPServer 8000

# 使用 Node.js
npx http-server

# 使用 Live Server (VS Code 扩展)
# 右键点击 index.html -> Open with Live Server
```

3. 在浏览器中访问 `http://localhost:8000`

## 📝 使用说明

### 1. 输入 JSON 数据

在左侧的文本框中输入符合 Plotly.js 格式的 JSON 数据。支持两种格式：

**格式一：完整对象格式**
```json
{
  "data": [
    {
      "type": "scatter",
      "x": [1, 2, 3, 4, 5],
      "y": [10, 15, 13, 17, 20],
      "mode": "lines+markers"
    }
  ],
  "layout": {
    "title": "我的图表",
    "xaxis": {"title": "X轴"},
    "yaxis": {"title": "Y轴"}
  }
}
```

**格式二：数据数组格式**
```json
[
  {
    "type": "bar",
    "x": ["苹果", "香蕉", "橙子"],
    "y": [12, 19, 3]
  }
]
```

### 2. 使用内置示例

点击工具栏中的示例按钮快速载入预设数据：
- 📈 **折线图**：展示时间序列数据
- 📊 **柱状图**：比较不同类别的数据
- 🥧 **饼图**：展示数据的比例关系
- 🎯 **散点图**：展示数据点的分布

### 3. 渲染图表

点击 "渲染图表" 按钮（或使用快捷键 `Ctrl+Enter`）生成图表。

### 4. 导出图表

图表渲染成功后，可以使用右上角的导出按钮：
- 🖼️ **PNG**：适合插入文档或演示
- 🎨 **SVG**：矢量格式，适合印刷和缩放

## 🎯 支持的图表类型

- **折线图** (`scatter` with `mode: 'lines'`)
- **散点图** (`scatter` with `mode: 'markers'`)
- **柱状图** (`bar`)
- **饼图** (`pie`)
- **直方图** (`histogram`)
- **箱线图** (`box`)
- **热力图** (`heatmap`)
- **3D 散点图** (`scatter3d`)
- **等高线图** (`contour`)
- **更多类型**：参考 [Plotly.js 文档](https://plotly.com/javascript/reference/)

## 🔧 高级功能

### 键盘快捷键

- `Ctrl+Enter` (或 `Cmd+Enter`)：渲染图表
- JSON 编辑器支持语法高亮和错误提示

### 自定义配置

您可以在 JSON 中添加 `config` 字段来自定义图表行为：

```json
{
  "data": [...],
  "layout": {...},
  "config": {
    "displayModeBar": true,
    "responsive": true,
    "toImageButtonOptions": {
      "format": "png",
      "filename": "my_chart",
      "height": 600,
      "width": 800
    }
  }
}
```

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本项目
2. 创建您的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## 📜 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🙏 致谢

- [Plotly.js](https://plotly.com/javascript/) - 强大的图表库
- [Tailwind CSS](https://tailwindcss.com/) - 优秀的 CSS 框架
- [Font Awesome](https://fontawesome.com/) - 图标字体库

## 📞 联系方式

如有问题或建议，请通过以下方式联系：

- 📧 Email: [linxy59@mail2.sysu.edu.cn]
- 🐛 Issues: [GitHub Issues](https://github.com/LinXueyuanStdio/PlotlyRender/issues)

---

⭐ 如果这个项目对您有帮助，请给它一个星星！
