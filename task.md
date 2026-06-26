# 任務進度追蹤 - gemini-voyager 測試與審查

- [x] 重新編譯專案以確保 `dist_chrome/` 為最新狀態 (`pnpm run build`)
- [x] 撰寫並優化 Playwright 自動化審查與載入測試腳本 (`scripts/automated_audit.js`)
- [x] 安裝 Playwright 專用 Chromium 乾淨沙盒以避免 Profile 衝突
- [x] 執行自動化側載與測試：
  - [x] 驗證並截圖 Extension Popup 頁面
  - [x] 驗證並截圖 Extension Options 頁面
  - [x] 驗證並截圖 Google Gemini 首頁的 Content Script 注入
- [x] 執行 Network Audit（網路行為審查）並生成報告：
  - [x] 稽核所有 Outgoing 網路請求
  - [x] 分類外部請求，核對白名單
  - [x] 證實 Extension 核心界面與 background service 無任何殘餘外部請求
- [x] 整理驗證報告並發布 `walkthrough.md`
