# 网络诊断报告生成器 | Network Diagnostic Report Generator

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

一个功能强大的网络诊断报告可视化工具，支持实时编辑和移动端优化显示。

[English](#english) | [中文](#中文)

---

## 中文

### ✨ 特性

- 🎨 **现代化UI设计** - 采用玻璃态设计风格，视觉效果出色
- 📱 **完美移动端适配** - 针对 iPhone 16 等高分辨率设备优化
- ⚡ **实时动态波形** - 三种不同的波形动画（正弦波、对数函数曲线）
- 🎛️ **完全可定制** - 所有参数都可通过控制面板实时调整
- 📊 **多维度网络指标** - 展示速度、延迟、抖动、丢包等关键指标
- 🎮 **专项测速** - 包含网页、直播、游戏三种场景的测速数据
- 💾 **零依赖** - 纯原生 HTML/CSS/JavaScript 实现

### 🚀 快速开始

1. **克隆仓库**
```bash
git clone https://github.com/你的用户名/network-diagnostic-report.git
cd network-diagnostic-report
```

2. **直接打开**
```bash
# 在浏览器中打开
open network_dialog_generator_verticalvice.html
# 或
start network_dialog_generator_verticalvice.html
```

3. **开始使用**
   - 无需安装任何依赖
   - 无需构建步骤
   - 直接在浏览器中运行

### 📸 预览截图

#### 桌面端视图
![Desktop View](screenshots/desktop-view.png)

#### 移动端视图
![Mobile View](screenshots/mobile-view.png)

#### 动态波形展示
![Waveform Animation](screenshots/waveform-demo.gif)

### 🎯 功能详解

#### 1. 基本信息设置
- 城市位置定位（经纬度坐标）
- ISP 运营商信息
- 内外部 IP 地址显示
- 自定义报告时间

#### 2. 网络速度监测
- **下载速度** - 实时显示 Mbps，配有平滑正弦波形
- **上传速度** - 对数函数增长曲线展示
- **流量统计** - 显示已使用流量
- **网速评估** - 自动对比全国用户数据

#### 3. 网络质量分析
- **时延测试** - 闲时/下载/上传三种状态
- **抖动测量** - 三组独立抖动数据
- **丢包率** - 实时丢包率统计
- **稳定性** - 显示最低/最高延迟值

#### 4. 专项测速
- **网页打开速度** - 模拟网页加载时间
- **直播测速** - 直播场景网络延迟（蓝色主题）
- **游戏测速** - 游戏场景网络延迟（红色主题）

#### 5. 波形可视化
##### 下载波形（绿色）
- 多重正弦波叠加
- 可调节频率、振幅、速度
- 流畅的动画效果

##### 上传波形（蓝色）
- 对数函数增长曲线
- 动态波动效果
- 可调节基数和缩放

#### 6. 控制面板
- 30+ 可调参数
- 实时预览效果
- 响应式布局设计

### 🎨 技术栈

- **前端框架**: 纯原生 JavaScript（无框架依赖）
- **样式**: CSS3（Flexbox + Grid 布局）
- **动画**: Canvas API + requestAnimationFrame
- **图标**: Unicode Emoji
- **字体**: 系统默认字体栈

### 📱 设备兼容性

| 设备类型 | 分辨率 | 兼容性 |
|---------|--------|--------|
| iPhone 16 | 2556×1179 (460ppi) | ✅ 完美支持 |
| iPhone 15/14/13 | 2532×1170 | ✅ 完美支持 |
| Android 旗舰机 | 1080p+ | ✅ 完美支持 |
| iPad | 2048×1536+ | ✅ 完美支持 |
| 桌面浏览器 | 1280px+ | ✅ 完美支持 |
| 小屏手机 | 375px+ | ✅ 优化支持 |

### 🌐 浏览器支持

- ✅ Chrome 90+
- ✅ Safari 14+
- ✅ Firefox 88+
- ✅ Edge 90+
- ⚠️ IE 11（部分功能不支持）

### 📝 使用说明

#### 基础使用
1. 打开 HTML 文件
2. 在控制面板输入网络数据
3. 实时查看报告预览
4. 支持截图保存

#### 高级定制
```javascript
// 自定义运营商图标（可选）
const carrierImages = {
    '中国联通': 'data:image/png;base64,...',
    '中国电信': 'data:image/png;base64,...',
    '中国移动': 'data:image/png;base64,...'
};
```

#### 波形参数调整
- **频率**: 控制波形密集程度（1-20）
- **振幅**: 控制波形高度（0.1-0.5）
- **速度**: 控制动画速度（0.01-0.1）
- **对数基数**: 控制增长速度（1.1-5）

### 🔧 自定义配置

#### 修改颜色主题
```css
/* 在 <style> 标签中修改 */
--primary-color: #667eea;
--success-color: #00d4aa;
--warning-color: #ffd93d;
--danger-color: #ff4a4a;
```

#### 调整布局尺寸
```css
/* 修改报告最大宽度 */
.mobile-report {
    max-width: 400px; /* 自定义宽度 */
}
```

### 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

### 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

### 👨‍💻 作者

- 您的名字 - [@你的GitHub用户名](https://github.com/你的用户名)

### 🙏 致谢

- 感谢所有贡献者
- Canvas API 文档
- 现代浏览器开发团队

### 📮 联系方式

- GitHub Issues: [提交问题](https://github.com/你的用户名/network-diagnostic-report/issues)
- Email: your.email@example.com

---

## English

### ✨ Features

- 🎨 **Modern UI Design** - Glassmorphism design style with stunning visual effects
- 📱 **Perfect Mobile Optimization** - Optimized for iPhone 16 and high-resolution devices
- ⚡ **Real-time Dynamic Waveforms** - Three different waveform animations (sine wave, logarithmic curve)
- 🎛️ **Fully Customizable** - All parameters adjustable via control panel
- 📊 **Multi-dimensional Network Metrics** - Display speed, latency, jitter, packet loss
- 🎮 **Specialized Speed Tests** - Web, Live streaming, and Gaming scenarios
- 💾 **Zero Dependencies** - Pure vanilla HTML/CSS/JavaScript

### 🚀 Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/network-diagnostic-report.git
cd network-diagnostic-report
```

2. **Open directly**
```bash
# Open in browser
open network_dialog_generator_verticalvice.html
```

3. **Start using**
   - No installation required
   - No build process needed
   - Run directly in browser

### 📊 Key Metrics

- Download/Upload Speed (Mbps)
- Network Latency (Idle/Download/Upload)
- Jitter Measurements
- Packet Loss Rate
- Page Load Speed
- Live Streaming Latency
- Gaming Latency

### 🛠️ Tech Stack

- **Frontend**: Vanilla JavaScript (No frameworks)
- **Styling**: CSS3 (Flexbox + Grid)
- **Animation**: Canvas API + requestAnimationFrame
- **Icons**: Unicode Emoji
- **Fonts**: System font stack

### 📱 Device Compatibility

| Device | Resolution | Support |
|--------|-----------|---------|
| iPhone 16 | 2556×1179 (460ppi) | ✅ Perfect |
| iPhone 15/14/13 | 2532×1170 | ✅ Perfect |
| Android Flagship | 1080p+ | ✅ Perfect |
| iPad | 2048×1536+ | ✅ Perfect |
| Desktop | 1280px+ | ✅ Perfect |
| Small Phones | 375px+ | ✅ Optimized |

### 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

### 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

⭐ **If you find this project helpful, please give it a star!**
```

## 🏷️ GitHub 项目标签建议

在 GitHub 仓库设置中添加以下 Topics:
```
network-diagnostic
network-monitoring
speed-test
visualization
canvas-animation
mobile-first
responsive-design
glassmorphism
vanilla-javascript
html5-canvas
network-analysis
china-isp
bandwidth-monitor
latency-test
waveform-visualization
no-dependencies
single-page-application
```

## 📋 项目描述（GitHub About）

**中文版本：**
```
网络诊断报告可视化工具 - 支持实时编辑、动态波形、多维度网络指标展示。完美适配移动端，纯原生实现，零依赖。
```

**英文版本：**
```
Network Diagnostic Report Generator - Real-time editing, dynamic waveforms, multi-dimensional metrics visualization. Perfect mobile optimization, vanilla JS, zero dependencies.
```

## 📁 建议的文件结构
```
network-diagnostic-report/
├── README.md                    # 项目说明文档
├── LICENSE                      # MIT 许可证
├── network_dialog_generator_verticalvice.html  # 主文件
├── screenshots/                 # 截图文件夹
│   ├── desktop-view.png
│   ├── mobile-view.png
│   └── waveform-demo.gif
├── .gitignore                   # Git 忽略文件
└── CHANGELOG.md                 # 更新日志（可选）
