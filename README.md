# 剪貼簿存檔器（DATA 複製神器）

把剪貼簿裡的文字、SVG 原始碼或圖片，快速存成 TXT、SVG、PNG、JPG 檔，並保留下載紀錄。

**線上使用**：https://kftseng2oo1.github.io/copy/

## 主要功能
- 四種模式：☰ 文字 TXT、◈ SVG、▣ PNG、◉ JPG
- 「貼上」直接讀剪貼簿；SVG 模式會檢查格式是否有效並可 ⬡ 預覽
- PNG／JPG 可設定尺寸與品質，SVG 可轉成點陣圖
- 下載紀錄含縮圖，可重新下載、還原內容或刪除

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- Clipboard API、Canvas、FileReader
- 紀錄存在 localStorage：`cs_pro_hist`
