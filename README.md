# 💊 臨床抗生素劑量與腎功能調整速查系統
> Clinical Antibiotics Renal Dosing Assistant

一個專為臨床醫師、藥師、專科護理師與醫護同仁設計的抗生素劑量速查工具，支援 eGFR / 透析（HD、PD、CRRT）劑量調整、Stat/Loading Dose 查詢與即時過濾。

---

## 🚀 快速開始 (Quick Start)

本系統採 **Zero-dependency（零相依、免安裝）** 前端架構設計：
1. 直接使用任一現代瀏覽器（Chrome, Edge, Safari, Firefox）開啟目錄下的 [`抗生素劑量調整.html`](file:///c:/Users/X4715G/Desktop/ANTIGRAVITY/Antibiotics%20dose/%E6%8A%97%E7%94%9F%E7%B4%A0%E5%8A%91%E9%87%8F%E8%AA%BF%E6%95%B4.html)。
2. 在上方搜尋欄輸入藥品學名、商品名或縮寫（如 `vanco`, `zefotam`, `curam`, `tapi`, `cefepime`），即時查看分級劑量。
3. 支援點選「IV 針劑」或「PO 口服」快速過濾給藥途徑。

---

## 📂 專案目錄結構 (Project Structure)

```text
Antibiotics dose/
├── PROJECT_RECORD.md          # 核心專案紀錄、系統架構與規格開發計畫
├── README.md                  # 專案快速入門與使用說明
├── index.html                 # 系統首頁 (供 GitHub Pages 預設載入與本地開啟)
├── 抗生素劑量調整.html        # 單檔式可執行查詢系統原型
├── 抗生素劑量調整.txt         # 原始代碼純文字備份
├── Antibiotics113-02-16.doc   # 臨床抗生素劑量基準手冊原始文件 (113-02-16 修訂)
└── .gitignore                 # Git 忽略檔案設定
```

---

## 🌐 發布至 GitHub Pages (Publishing Guide)

本工具為純靜態單頁應用，已配置標準 `index.html`，可一鍵免費部署至 GitHub Pages：

1. **建立遠端倉庫**：於 GitHub 建立新 Repository（例如名為 `antibiotics-dose-guide`）。
2. **推送本專案至 GitHub**：
   ```bash
   git branch -M main
   git remote add origin https://github.com/<您的帳號>/antibiotics-dose-guide.git
   git push -u origin main
   ```
3. **啟用 GitHub Pages**：
   - 進入 GitHub 倉庫的 **Settings** -> 左側選單 **Pages**。
   - 在 **Build and deployment** > **Source** 選擇 `Deploy from a branch`。
   - 在 **Branch** 選取 `main` / `(root)`，並點擊 **Save**。
4. **完成上線**：
   - 等待約 1~2 分鐘後，即可在 `https://<您的帳號>.github.io/antibiotics-dose-guide/` 隨時隨地開啟使用！

---

## 📋 功能特點 (Current & Upcoming Features)

- [x] **33+ 種常用抗生素收錄**：涵蓋 Penicillins, Cephalosporins, Carbapenems, Fluoroquinolones, Glycopeptides, Aminoglycosides, Antifungals, Antivirals 等 9 大類。
- [x] **腎功能分級劑量矩陣**：提供 Stat / Loading dose、>50 mL/min (常規)、10–50 mL/min (中度)、<10 mL/min (重度/透析) 清晰對照。
- [x] **單一藥物聚光燈預覽卡**：下拉快速鎖定單一藥物，卡片化檢視各分級。
- [x] **GitHub Pages 零配置即時發布**：自帶 `index.html`，推送到 GitHub 即可連線使用。
- [ ] **腎功能計算機整合 (即將推出)**：內建 Cockcroft-Gault CrCl 與 CKD-EPI eGFR 計算，自動高亮對應劑量級距。
- [ ] **資料結構化分離 (即將推出)**：抽離獨立 `antibiotics_data.json` 數據層，便於資料更新與校對。
- [ ] **行動介面強化與複製醫囑 (即將推出)**：提供手機直式卡片檢視與一鍵複製建議處方文字功能。

---

## 📖 詳細專案規格與開發計畫

請參閱完整的專案管理紀錄：[PROJECT_RECORD.md](file:///c:/Users/X4715G/Desktop/ANTIGRAVITY/Antibiotics%20dose/PROJECT_RECORD.md)。
