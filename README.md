# 知命齋 · Jekyll 命理研習博客

一個典雅、深邃、溫潤的命理研習與人生覺察博客，基於 Jekyll 構建，完美相容 GitHub Pages 原生託管。

**核心特色：**
- ✍️ **寫文章超輕鬆**：只需在 `_posts/` 資料夾中新增 Markdown 檔案，首頁與標籤頁自動更新！
- 🌐 **繁簡隨心切換**：內建 OpenCC 繁簡即時轉換功能，右上角一鍵切換，滿足不同讀者需求。
- 📱 **全設備響應式**：針對手機、平板、電腦進行精準排版適配，閱讀體驗溫潤如紙。
- 🔍 **SEO & AI 友善**：內建 Schema.org Article / Person 結構化資料、Sitemap、RSS Feed 與 Meta 標籤。

---

## 📁 檔案結構

```text
mingli-notes/
├── _config.yml              # 站點設定檔（網站名稱、副標題、網址、作者等）
├── _layouts/                # 頁面版型模板
│   ├── default.html         # 預設通用版型（頂部導航、繁簡切換、頁腳、彈窗）
│   └── post.html            # 文章詳情頁版型（結構化數據、閱讀時間、社群卡片、上下篇）
├── _posts/                  # 所有研習文章（Markdown 格式）
│   ├── 2026-10-01-learning-mingli-from-fortune-telling-to-self-awareness.md
│   ├── 2026-10-04-yin-yang-five-elements-life-balance.md
│   └── 2026-10-07-astrology-and-bazi-life-map.md
├── assets/                  # 靜態圖片（頭像、QR Code 等）
├── css/
│   └── style.css            # 博客樣式表（宣紙底色 + 黛青玄墨主色 + 優雅襯線字型）
├── js/
│   └── main.js              # 滾動導航、行動端選單、平滑錨點、回到頂部腳本
├── index.html               # 博客首頁（Hero 橫幅、最新文章列表、心法引言）
├── tags.html                # 標籤聚合頁（標籤雲、按主題分類文章列表）
├── about.md                 # 關於齋主與知命齋理念介紹頁
├── Gemfile                  # 本地預覽相依套件設定
├── robots.txt               # 搜尋引擎爬蟲指引
└── README.md                # 專案說明文件
```

---

## 🚀 部署至 GitHub Pages

本專案已關聯至 GitHub 倉庫：`https://github.com/coachsunny/mingli-notes`
線上網址：`https://coachsunny.github.io/mingli-notes/`

### 啟用 GitHub Pages 步驟：
1. 前往 GitHub 倉庫頁面：[https://github.com/coachsunny/mingli-notes](https://github.com/coachsunny/mingli-notes)
2. 點擊頂部 **Settings**（設定）
3. 在左側選單點擊 **Pages**
4. 在 **Build and deployment** > **Branch** 中：
   - 選擇分支：`main`
   - 選擇目錄：`/ (root)`
5. 點擊 **Save**（儲存）
6. 稍候 1~2 分鐘，頁面頂部即會顯示已部署的網址：`https://coachsunny.github.io/mingli-notes/`

---

## ✍️ 如何新增文章

每次撰寫新文章，只需兩步：

### 步驟 1：在 `_posts/` 資料夾新增 Markdown 檔案

檔名格式規定為：`YYYY-MM-DD-文章英文標識.md`  
例如：`2026-10-15-bazi-ten-gods-psychology.md`

### 步驟 2：填寫 Front Matter 元資訊與正文

```markdown
---
layout: post
title: 你的文章標題
date: 2026-10-15
tags: [八字命理, 十神心性, 覺察體悟]
read_time: 6
description: 文章的一句話摘要，會顯示在首頁卡片與搜尋引擎預覽中。
---

這裡開始寫正文，使用標準 Markdown 語法即可。

<!--more-->

## 小標題

正文段落內容……

> 引言或古籍金句

**重點文字加粗**
```

> 💡 **提示**：正文中的 `<!--more-->` 標記為摘要截斷點，上面的內容將作為文章開頭導讀。

---

## 💻 本地預覽（選用）

若需要在本機電腦預覽效果：
```bash
# 1. 安裝 Ruby 相依套件
bundle install

# 2. 啟動 Jekyll 本地伺服器
bundle exec jekyll serve

# 3. 在瀏覽器打開 http://localhost:4000/mingli-notes/
```
