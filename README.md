# 🏸 Badminton Pro 3D - 羽球殺球與技術學習平台

<p align="center">
  <img src="https://img.shields.org/badge/WebGL-60\_FPS-0284c7?style=for-the-badge\&logo=three.js\&logoColor=white" alt="WebGL 60FPS">
  <img src="https://img.shields.org/badge/Three.js-r128-38bdf8?style=for-the-badge\&logo=three.js\&logoColor=white" alt="Three.js">
  <img src="https://img.shields.org/badge/Web\_Audio-API-10b981?style=for-the-badge" alt="Web Audio API">
  <img src="https://img.shields.org/badge/License-MIT-f59e0b?style=for-the-badge" alt="License MIT">
</p>

> \*\*精準角度 ‧ 高效發力 ‧ 3D WebGL 羽球擊球與戰術模擬學習系統\*\*  
> 結合第一人稱視角 (FPS)、羽球空氣動力學物理引擎、甜區 (Sweet Spot) 發力 Timing 與 AI 機器人動態對戰。

\---

## 📌 專案簡介 (Overview)

**Badminton Pro 3D** 是一款基於純前端技術（WebGL / Three.js）開發的高效能 3D 羽球技術學習與動態對戰平台。

不同於傳統第三人稱俯瞰視角的羽球遊戲，本專案採用 **第一人稱視角 (First-Person Perspective)**，真實還原球員站在場地上的視角視野。使用者可透過滑鼠仰俯角瞄準高點擊球，配合畫面下方的發力 timing 條與起跳機制，體驗 150+ km/h 以上的極速扣殺震撼！

\---

## 💡 專案緣由與開發動機 (Motivation \& Origin)

### 1\. 解決真實羽球訓練的空間與視角痛點

在羽球運動中，「殺球下壓角度」與「擊球高點預判」是許多初學者最難掌握的技巧。然而，傳統 2D 或第三人稱遊戲無法提供真實的仰面打擊感與視角高低落差。

### 2\. 打造零延遲、無需安裝的高效學習平台

希望開發一款**無需安裝任何下載包、不需依賴大型伺服器**的單頁 WebGL 應用程式。只要開啟瀏覽器，就能讓使用者在幾秒鐘內體驗到極致流暢的 3D 羽球揮拍、戰術拉鋸與數據分析。

\---

## 🌟 核心特色 (Key Features)

### 🎯 1. 第一人稱視角 (FPS) 仰俯角瞄準

* 使用滑鼠自由調控視角，模擬真實抬頭瞄準高點羽球的打擊視野。
* 支援鍵盤 <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> 走位與 <kbd>SPACE</kbd> 騰空起跳下壓。

### ⚡ 2. 甜區 (Sweet Spot) 與 Timing 發力系統

* 內建動態發力指針，玩家需要在 Timing 進入綠色甜區 (68% - 92%) 的瞬間揮拍。
* 完美的 Timing 配合起跳能解鎖最大殺球初速 (200+ km/h) 與震撼打擊音效。

### 🤖 3. 智慧 AI 影子對手 (Dynamic AI Rally)

* 後場 AI 機器人具備即時預判落點能力，支援動態移動與連續來回拉鋸。
* 提供「簡單、普通、困難、大師」四階難度與四種訓練關卡。

### 🏸 4. 五大戰術球路與拍面切換

* **重殺 (Smash)**：陡角下壓，極速貫穿對手防線。
* **切球 (Drop)**：網前輕吊，破壞 AI 後場節奏。
* **平球 (Drive)** / **高遠球 (Clear)** / **撲推 (Push)**：靈活變換，支援 <kbd>Q</kbd> / <kbd>E</kbd> 直線與斜線攻擊。

### 🛒 5. 裝備商城與實時數據 HUD

* 累積訓練得分可解鎖「雷霆重殺拍」、「疾風輕羽拍」與「帝王金龍拍」，即時變更 3D 第一人稱球拍塗裝與屬性加成。
* 儀表板實時計算「對戰勝率 (Win Rate)」、「甜區命中率 (Accuracy)」、「殺球初速 (km/h)」與下壓角度。

\---

## 🚀 專案研發歷程 (Development Journey Timeline)

```
Phase 1: 物理與視角系統  ---> Phase 2: AI 對戰與球路  ---> Phase 3: 裝備與難度分級  ---> Phase 4: 門面整合與體驗優化
```

* **PHASE 1 ‧ 3D WebGL 場景與第一人稱視角**

  * 建構標準羽球場地、球網與高空場館模型。
  * 實作第一人稱視角綁定與空氣阻力 Drag 物理拋物線演算。
* **PHASE 2 ‧ AI 對戰與 5 大球路系統**

  * 研發 AI 機器人動態腳步演算法，實現來回拉鋸。
  * 加入重殺、切球、平球、高遠與撲推 5 種球路與斜線轉換。
* **PHASE 3 ‧ 球拍商城與難度分級**

  * 引入 Web Audio API 純前端純音效合成器。
  * 開發球拍裝備系統與四階 AI 難度（EASY \~ MASTER）。
* **PHASE 4 ‧ 一頁式 showcase 與無縫線上試玩**

  * 整合一頁式門面網頁（`cover.html`）與全功能體驗區。
  * 加入 Suno AI 原創主題曲《Smash the Limits》專區與極速打擊感震波特效。

\---

## 🛠️ 技術架構 (Technical Architecture)

本專案採用 100% 前端純原生架構，無需任何後端 Build Step：

* **3D 渲染引擎**：[Three.js (r128)](https://threejs.org/)
* **UI 樣式與佈局**：Tailwind CSS (CDN)
* **音效合成**：Web Audio API (原生 OscillatorNode \& GainNode 手繪音波)
* **圖示與字型**：Font Awesome 6.4.0, Google Fonts (Outfit \& Noto Sans TC)

\---

## 🎮 操作指南 (Controls)

|操作動作|按鍵 / 滑鼠|
|-|-|
|**視角瞄準**|移動滑鼠 (Mouse Look)|
|**場地走位**|<kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> / 方向鍵|
|**騰空起跳**|<kbd>SPACE</kbd> (空白鍵)|
|**揮拍擊球**|滑鼠左鍵 (Left Click)|
|**球路切換**|<kbd>1</kbd> 重殺 / <kbd>2</kbd> 切球 / <kbd>3</kbd> 平球 / <kbd>4</kbd> 高遠 / <kbd>5</kbd> 撲推|
|**直線/斜線**|<kbd>Q</kbd> 或 <kbd>E</kbd>|

\---

## 📂 檔案結構 (File Structure)

```text
.
├── cover.html          # 一頁式門面展示頁面 (含原生 3D 遊戲對戰入口)
├── index.html          # 全螢幕 3D 羽球遊戲主程式引擎
├── zsky-62ff36e9.mp4   # 實機展示對戰宣傳短片
└── suno\_theme\_song.md  # Suno AI 主題曲歌詞與音樂 Style 設定檔
```

\---

## 📄 授權條款 (License)

本專案採用 [MIT License](LICENSE) 授權條款。歡迎自由下載、學習與二次開發。


