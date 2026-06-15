# 🍏 TIMI RedmiBook Pro 14S 锐龙版 · OpenCore Hackintosh

<p align="center">
  <img src="https://img.shields.io/badge/macOS-Sonoma_14.8.2-0071BC?logo=apple&logoColor=white" alt="macOS" />
  <img src="https://img.shields.io/badge/CPU-AMD_Ryzen_7_5700U-ED1C24?logo=amd&logoColor=white" alt="CPU" />
  <img src="https://img.shields.io/badge/OpenCore-1.0.6-9cf?logo=opencollective&logoColor=white" alt="OpenCore" />
  <img src="https://img.shields.io/badge/Status-Working-success" alt="Status" />
  <img src="https://img.shields.io/badge/RAM-16_GB_3200MHz-8B5CF6" alt="RAM" />
  <img src="https://img.shields.io/badge/Storage-512GB_NVMe-10B981" alt="Storage" />
</p>

<div align="center">
  <i>将 RedmiBook Pro 14S 锐龙版带入 macOS Sonoma 的完整 EFI 配置方案。</i>
  <br>
  <b>AMD Ryzen 7 5700U · Vega 核显 · 2560×1600 · OpenCore 1.0.6</b>
</div>

---

## ✨ 功能清单

<table>
<tr>
<td align="center">🎨<br><b>显卡</b></td>
<td align="center">🖱️<br><b>触控板</b></td>
<td align="center">📷<br><b>摄像头</b></td>
<td align="center">🌐<br><b>Wi-Fi</b></td>
</tr>
<tr>
<td align="center">AMD Radeon RX<br>Metal 加速 ✅</td>
<td align="center">多指手势<br>Force Touch ✅</td>
<td align="center">XiaoMi USB 2.0<br>即插即用 ✅</td>
<td align="center">Intel AX200<br>正常连接 ✅</td>
</tr>
<tr>
<td align="center">🔋<br><b>电池</b></td>
<td align="center">🔊<br><b>声卡</b></td>
<td align="center">🦷<br><b>蓝牙</b></td>
<td align="center">💡<br><b>亮度调节</b></td>
</tr>
<tr>
<td align="center">电量显示<br>健康度 98.93% ✅</td>
<td align="center">内置扬声器<br>麦克风正常 ✅</td>
<td align="center">耳机 · 鼠标<br>可配对 ✅</td>
<td align="center">自动调光<br>夜览支持 ✅</td>
</tr>
</table>

---

## 💻 硬件规格

| 项目 | 规格 |
|------|------|
| **处理器** | AMD Ryzen 7 5700U (八核) |
| **内存** | 16 GB DDR4 3200MHz (三星) |
| **显卡** | AMD Radeon Graphics (集成，2GB VRAM) |
| **主板** | TIMI TM2013 |
| **显示器** | 14" 2560×1600 (NCP006A) |
| **存储** | KBG40ZNV512G KIOXIA (512GB NVMe) |
| **网卡** | Intel Wi-Fi 6 AX200 160MHz |
| **电池** | SUNWODA R14B02W (健康度 98.93%) |
| **声卡** | 瑞昱 @ AMD HD Audio |
| **摄像头** | XiaoMi USB 2.0 Webcam |

---

## 🖥️ 系统详情

<table>
<tr>
<td align="center"><b>机型伪装</b></td>
<td align="center">MacBook Pro (13-inch, 2020)</td>
</tr>
<tr>
<td align="center"><b>启动磁盘</b></td>
<td align="center">Mac</td>
</tr>
<tr>
<td align="center"><b>分辨率</b></td>
<td align="center">2560 × 1600 @ 60Hz</td>
</tr>
</table>

---

## 📸 截图预览

<details open>
<summary><b>点击展开/收起截图</b></summary>

<br>

> 💡 点击缩略图查看原始分辨率大图

<table>
<tr>
<td align="center"><a href="./关于本机.png"><img src="./screenshots/关于本机.png" alt="系统概览"><br>📋 系统概览</a></td>
<td align="center"><a href="./核显.png"><img src="./screenshots/核显.png" alt="显卡信息"><br>🎨 显卡信息</a></td>
</tr>
<tr>
<td align="center"><a href="./触控板.png"><img src="./screenshots/触控板.png" alt="触控板"><br>🖱️ 触控板</a></td>
<td align="center"><a href="./摄像头.png"><img src="./screenshots/摄像头.png" alt="摄像头"><br>📷 摄像头</a></td>
</tr>
<tr>
<td align="center"><a href="./电池.png"><img src="./screenshots/电池.png" alt="电池"><br>🔋 电池</a></td>
<td align="center"><a href="./hidpi.png"><img src="./screenshots/hidpi.png" alt="HiDPI"><br>🖼️ 显示设置</a></td>
</tr>
<tr>
<td align="center"><a href="./声卡.png"><img src="./screenshots/声卡.png" alt="声卡"><br>🔊 声卡</a></td>
<td align="center"><a href="./配置图.jpg"><img src="./screenshots/配置图.jpg" alt="配置图"><br>⚙️ 配置图</a></td>
</tr>
</table>

</details>

---

## 📦 使用说明

### 准备工作

1. **下载 EFI** → [123 云盘](https://www.123865.com/ps/HiZ0Vv-GxnNh)（提取码见盘内说明）
2. **制作启动盘**：使用 [BalenaEtcher](https://www.balena.io/etcher/) 或 Terminal 将 macOS 镜像写入 U 盘
3. **替换 EFI**：用 OpenCore Configurator 挂载 U 盘 EFI 分区，将本项目 EFI 完整复制进去
4. **首次启动**：选择 U 盘启动 → OpenCore 菜单 → Install macOS
5. **安装完成后**：将 EFI 复制到系统盘 EFI 分区，即可脱离 U 盘启动

> ⚠️ **注意**：本配置基于 AMD Ryzen 7 5700U + Vega 核显平台，<br>仅适用于同型号或相似硬件设备。不同批次硬件可能存在差异。

### 推荐工具

| 工具 | 用途 | 链接 |
|------|------|------|
| OpenCore Configurator | EFI 可视化配置 | [GitHub](https://github.com/OpenCore-Legacy-Patcher/OpenCore-Configurator) |
| Hackintool | 硬件检测与补丁 | [GitHub](https://github.com/dortania/Hackintool) |
| ProperTree | plist 编辑 | [GitHub](https://github.com/corpnewt/ProperTree) |
| CorpNewt 工具集 | USB / 磁盘工具 | [GitHub](https://github.com/corpnewt) |

---

<div align="center">
  <img src="https://img.shields.io/badge/Built_with_❤️_for_the_Hackintosh_Community-FF6B6B" alt="Built with love">
  <br>
  <sub>
  ⭐ Star 这个项目如果它对你有帮助！<br>
  有问题请提交 <a href="https://github.com/WT2072861996/TIMI-RedmiBook-Pro-14S-open-core-1.06/issues">Issues</a>
  </sub>
</div>
