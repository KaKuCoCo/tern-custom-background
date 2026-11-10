# Fork changelog

上游：[naraaalt/tern-custom-background](https://github.com/naraaalt/tern-custom-background)

## 2026-11-10

### Added
- Surfaces 設定：分別調暗標籤列、狀態列與 omp 輸入框。
  - 原因：這些區域直接疊在圖片上，文字不易閱讀。

### Changed
- 圖片改為 `body::before` 透明圖層。
  - 原因：Tern 玻璃材質會清除 `body` 背景，黑色遮罩也擋住桌面透出。

### Fixed
- 浮動預覽與 Git 檔案面板改用半透明底色加模糊。
  - 原因：底下的 pane 文字與 commit graph 會穿透；不透明底色又會蓋掉圖片。
- 繪製失敗時清除繪製簽章。
  - 原因：重新安裝後引擎編好前繪製失敗，之後不會再重繪，Status 頁一直顯示失敗。
  - 上游：未回報。

## 已移除
