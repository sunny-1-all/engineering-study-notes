# Engineering Study Notes — AI Development Rules

## 1. 專案目的
建立一個工程學習筆記網站，整理大學工程相關科目的重要觀念、公式及範例。

目前包含：
- 資料結構 Data Structures
- 微積分 Calculus
- 材料科學 Materials Science

未來可以新增工程數學、熱力學及電路學等科目。

## 2. 使用技術
- HTML：建立網頁結構。
- CSS：設計網頁外觀。
- JavaScript：實作搜尋及分類功能。
- GitHub Pages：發布網站。

不需要後端、資料庫或額外 API。

## 3. 網頁風格
- 使用深藍色、白色與淺灰色。
- 採用簡潔的卡片式設計。
- 主要使用繁體中文，英文專有名詞需保留。
- 支援手機與電腦瀏覽。

## 4. 檔案結構

```text
engineering-study-notes/
├── index.html
├── AGENTS.md
└── README.md
```

## 5. 新增筆記規則

所有筆記必須包含以下欄位：

- id：唯一識別碼
- category：科目分類
- title：中文標題
- english：英文名稱
- concept：重要觀念
- formula：公式或規則
- example：應用範例

新增筆記時，應將資料加入 `index.html` 的 `notes` 陣列，不需要重新建立網頁。

例如：

```javascript
{
  id: "thermo-first-law",
  category: "熱力學",
  title: "熱力學第一定律",
  english: "First Law of Thermodynamics",
  concept: "能量不會憑空產生或消失，只會轉換形式。",
  formula: "ΔU = Q - W（封閉系統，忽略動能與位能變化）",
  example: "氣體吸收熱量後，部分能量可能轉換為對外作功。"
}
```

如果新增了新的科目分類，也必須同步更新網站的分類按鈕。

## 6. AI 修改規則

當 AI 收到新增或修改內容的要求時，必須：

1. 先閱讀 AGENTS.md。
2. 檢查是否已有相同主題。
3. 遵守既有資料格式。
4. 確保每筆資料有不同的 id。
5. 保留原本的網站功能。
6. 不隨意修改其他筆記。
7. 維持相同的網頁風格。
8. 修改完成後進行測試。

## 7. 測試規則

每次新增內容後，應確認：

- 網站可以正常開啟。
- 新筆記能正確顯示。
- 分類功能正常。
- 搜尋功能正常。
- 手機版面沒有明顯錯誤。

## 8. 未來擴充方式

未來可以持續新增工程相關科目。

AI 只需要閱讀本文件，就能依照相同的格式新增筆記，不需要重新設計整個網站。

這樣可以讓網站長期維持一致的結構，並提高後續開發效率。
