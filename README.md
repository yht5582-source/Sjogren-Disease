# Sjögren Clinical Navigator

獨立單頁網頁（index.html），不需要安裝、後端、API Key 或網路連線即可輸入資料、計算及輸出分析。

## 功能
- ACR/EULAR 2016 5 項分類分數、適用條件與排除條件（區分未知/陰性）
- AG / albumin-corrected AG / urine anion gap（保留臨床解讀限制）
- 低血鉀及酸血症緊急警示
- distal RTA / TIN / GN / 慢性纖維化 / 淋巴瘤紅旗分流
- 指南等級的治療方向、臨床追蹤
- 8 個合成示範病例、匿名文字匯出、列印

## 使用
雙擊 `index.html` 在瀏覽器開啟；或放到靜態託管服務（例如 GitHub Pages）。無第三方 JavaScript 和病歷資料傳輸。

## 警告
僅供教學及醫療專業決策輔助，尚未經醫療器材驗證。不能替代病理確認、血氣判讀、緊急處置及醫師處方。2026-11 研究基準，臨床採用前須進行藥物審查與更新。

## 指南
- ACR/EULAR 2016: https://pmc.ncbi.nlm.nih.gov/articles/PMC5650478/
- BSR 2024/2025: https://pmc.ncbi.nlm.nih.gov/articles/PMC12013823/
- EULAR 2019/2020: https://ard.bmj.com/content/79/1/3

## v3.0 integrated page
The main entry point is `index.html`. The sixth main tab now contains:
- ESSDAI 12-domain weighted scoring (0–123) with domain-specific permissible activity levels. Unassessed domains never silently count as zero; severity selections require clinician confirmation against the official domain definitions.
- Renal biopsy consideration and immunosuppression pre-treatment checklist.
- Session-only longitudinal charts for eGFR, potassium, bicarbonate, and UPCR, with anonymous CSV export. Entries are not saved after page refresh.
- Integrated clinical differential and supportive-treatment considerations based on the existing main form.
- Four complex educational cases and 20 questions.

The earlier `advanced.html` remains accessible as a legacy link; all functions are integrated into the main page.

### Clinical boundaries
This is an educational decision-support prototype, not validated medical software or a prescribing device. It does not connect to hospital systems, persist patient records, confirm disease attribution, independently establish ESSDAI domain activity, or provide immunosuppression orders. Users must verify laboratory values, clinical exclusions, and institutional protocols.

ESSDAI original user guide: https://pmc.ncbi.nlm.nih.gov/articles/PMC4613159/
