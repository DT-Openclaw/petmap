# 🐕 迷雾遛狗地图 (PetMap)

一款类似 Keep 跑步记录但带有游戏化迷雾探索机制的遛狗轨迹记录工具。

![Version](https://img.shields.io/badge/Version-v1.0-green)
![License](https://img.shields.io/badge/License-MIT-blue)

## 🐕 迷雾遛狗地图 v1.0

**在线访问**: http://118.178.125.76:5004

---

## ✨ 功能特性

### 🛰️ GPS 轨迹记录
- 实时 GPS 定位与路径绘制
- 精确计算：里程、时长、平均速度、消耗卡路里
- 支持开始/暂停/结束遛狗
- 自动保存遛狗记录到本地

### 🌫️ 迷雾森林探索机制（核心特色）
- 初始状态：除起点周围 50 米外，全部被迷雾覆盖
- 走到新地方自动消散周边迷雾（默认 30 米半径）
- 已探索区域永久保留，下次打开仍可见
- 显示全局探索进度百分比

### 📋 历史记录管理
- 保存所有遛狗记录（日期、时长、里程、速度、轨迹）
- 点击历史记录可回放轨迹
- 支持删除单条/清空全部
- 显示累计遛狗次数和总里程

### 🎮 额外功能
- 🗺️ 切换地图类型（标准/卫星/地形）
- 🎯 探索半径调节（20-50米可调）
- 🏆 成就系统（7个成就）
- ⏰ 遛狗提醒闹钟
- 🌙 夜间模式

## 🚀 快速开始

### 在线访问
直接访问：**http://118.178.125.76:5004**

### 本地运行
```bash
# 克隆项目
git clone https://github.com/DT-Openclaw/petmap.git
cd petmap

# 使用 Python 启动
python3 -m http.server 8080

# 或使用 Node.js
node -e "require('http').createServer((r,s)=>{s.writeHead(200);require('fs').readFile('index.html',(e,d)=>s.end(d))}).listen(8080)"
```

然后浏览器打开 `http://localhost:8080`

## 📱 使用说明

1. **首次打开** → 允许浏览器获取位置权限
2. **点击"开始遛狗"** → 开始记录轨迹
3. **走在路上** → 迷雾会自动消散
4. **点击"结束"** → 保存本次遛狗记录

## 🔧 技术栈

- HTML5 + CSS3 + JavaScript（原生的，无框架依赖）
- Leaflet.js 地图库 + OpenStreetMap
- 浏览器 Geolocation API
- localStorage 本地存储

## 📄 许可证

MIT License

---

Made with ❤️ for dog lovers 🐕