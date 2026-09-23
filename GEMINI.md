# 專案準則與設計規範 (Project Rules & Design Guidelines)

## 🚨 使用者核心指令與原則 (Strict User Principles)

1. **規劃優先原則**：
   - 「**接下來對話 都先規劃 說ok再執行**」
   - 任何涉及檔案修改、資源生成、Git 提交的操作，皆必須先列出規劃書，待使用者確認回覆「ok」後方可執行。
2. **局部更新與保護既有成果原則**：
   - 「**更新時 原設定及原則不變動 只更新要更新部分 不然本來改好的 又要一直重來**」
   - 嚴禁變動無關的資料欄位、排版樣式或已確認邏輯，每次更新皆需進行雙檔（`index.html` 與 `抗生素劑量調整.html`）SHA256 完整性校對。
3. **App Logo 核心原則**：
   - 「**好的手機 App Logo（應用程式圖示，App Icon）核心目標只有兩個：在極小的尺寸下一眼被認出，以及精準傳達產品的核心價值或風格。**」

---

## 🎨 專案正式設計風格記憶：文青紙感極簡線性圖標風

本專案的圖標與品牌視覺風格定調為：
**「文青紙感極簡線性圖標風（Minimalist Line Art Badge with Paper Texture）」**

融合了簡約線條與手作紙質的人文溫度，具體特色包含：

### 1. 四大核心視覺特徵
1. **極簡線性圖標（Minimalist Line Art / Iconography）**：
   - 以簡約流暢的粗線條與實心剪影呈現核心元素（細菌／病毒微粒、注射針筒、右下角的植物線條標記），造形結構乾淨易讀。
2. **圓角徽章佈局（Rounded Square Badge）**：
   - 外層以圓潤的粗外框收納主體，具備 App Icon、印章徽章或臨床指示圖樣的規格感。
3. **大地與醫療專業配色（Muted Earthy & Teal Palette）**：
   - **主視覺**：使用冷靜、專業的霧面藍綠色／湖水青（Muted Teal，`#3B8E96`）。
   - **外框**：溫潤沉穩的駝金／芥末土黃色（Ochre / Muted Gold，`#A18238`）。
4. **溫潤手作紙紋背景（Textured Cream/Washi Paper）**：
   - 底色非死白的螢幕純色，而是帶有細緻纖維顆粒感的米白手作紙／水彩紙質感（`#F8F6F0`），中和了醫療題材的生硬感，多了一份溫和人文氣息。

---

## 🔑 AI 繪圖提示詞配方 (Prompting Formula)

若需以此風格生圖或設計同系列視覺元素，請必定使用以下關鍵字組：

```text
minimalist medical line art icon, rounded square frame, muted teal and gold palette, textured cream paper background, clean flat iconography
```
