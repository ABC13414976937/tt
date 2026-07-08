🌤 极简天气预报
一个无需 API 密钥、可直接运行的纯前端天气应用，支持城市搜索和定位，提供实时天气及未来 3 天预报。

![界面截图](https://via.placeholder.com/800x400?text=Weather+App+Screenshot)  
（*可替换为实际截图*）

## ✨ 功能特性

- 🔍 **城市搜索**：输入任意城市名称（支持中文），快速获取天气信息。
- 📍 **定位服务**：一键获取当前位置天气（需浏览器授权）。
- 🌡️ **实时天气**：显示温度、天气状况、湿度（模拟）、风速。
- 📅 **3 天预报**：展示未来三天的最高/最低温度、天气图标及文字描述。
- 🎨 **毛玻璃质感 UI**：现代、柔和、适配移动端，交互反馈流畅。
- 💾 **本地缓存**：自动记住上次搜索的城市，下次打开自动加载。

## 🛠 技术栈

- **HTML5** + **CSS3**（Flex/Grid 布局，毛玻璃效果）
- **原生 JavaScript**（ES6+，无任何第三方库）
- **字体与图标**：Google Fonts (Inter) + Font Awesome 6
- **天气数据**：[Open-Meteo API](https://open-meteo.com/)（免费、无需密钥、支持跨域）
  - Geocoding API → 城市转经纬度
  - Forecast API → 当前天气 + 每日预报

## 🚀 快速开始

### 在线体验
直接下载 `index.html` 并在浏览器中打开即可使用，无需安装任何依赖或配置环境。

### 本地运行
```bash
# 克隆仓库（或直接下载 HTML 文件）
git clone https://github.com/yourusername/weather-app.git
cd weather-app

# 使用任意 HTTP 服务器（推荐 VS Code Live Server 或 Python 内置）
# 例如 Python 3：
python -m http.server 8000
# 然后访问 http://localhost:8000
使用说明
在输入框中输入城市名称（如“北京”、“上海”、“佛山”）。

点击“搜索”按钮或按回车键。

点击定位图标可获取当前位置天气（需允许浏览器获取位置）。

页面会自动显示当前天气和未来 3 天预报。

📦 部署
由于是纯静态页面，你可以将其部署到任何静态托管服务：

Vercel / Netlify：直接拖拽 index.html 即可。

GitHub Pages：将文件推送到仓库，开启 Pages 功能。

CloudFlare Pages 或 任何 Web 服务器。

⚙️ API 说明
本项目使用 Open-Meteo 公开 API，无需注册或密钥：

用途	API 端点
地理编码（城市→坐标）	https://geocoding-api.open-meteo.com/v1/search
天气数据（当前+预报）	https://api.open-meteo.com/v1/forecast
注意：Open-Meteo 对免费请求有一定频率限制，但个人使用完全足够。

📁 项目结构
text
/
├── index.html          # 完整应用（HTML + CSS + JS 单文件）
└── README.md           # 项目说明
🤝 贡献
欢迎提交 Issue 或 Pull Request！如果你有改进建议或发现 bug，请随时提出。

Fork 本仓库

创建你的特性分支 (git checkout -b feature/AmazingFeature)

提交更改 (git commit -m 'Add some AmazingFeature')

推送到分支 (git push origin feature/AmazingFeature)

打开 Pull Request

📄 许可证
本项目基于 MIT 许可证开源 - 详见 LICENSE 文件。

🙏 致谢
数据提供：Open-Meteo

图标库：Font Awesome

字体：Inter

text

---

你可以将以上内容保存为 `README.md`，并根据实际情况修改（如替换截图链接、添加自己的仓库地址等）。如果还需要补充任何内容（如常见问题、环境变量说明等），请告诉我，我可以进一步调整。
