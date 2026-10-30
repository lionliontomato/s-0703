# Shuan × SHM 整合入口

此 GitHub Pages 專案以同一個入口切換載入原本兩個網站：

- Shuan：https://lionliontomato.github.io/shuan/
- SHM：https://lionliontomato.github.io/SHM/

## 保留方式

- 原網站以 iframe 載入，不重製或覆寫原網站的 HTML、CSS、字體、背景、動畫及互動程式。
- 兩個網站仍各自讀取原本的資料來源與試算表，不合併資料。
- 切換時會嘗試讀取目前頁面的原始 `link rel="icon"`，同步更新整合入口的瀏覽器分頁圖示與頁面標題。
- 「另開原網站」可在新分頁開啟目前選取的原網站。

## 發布到 GitHub Pages

1. 建立新的 Public Repository。
2. 將本資料夾內的 `index.html`、`README.md`、`.nojekyll` 上傳到 Repository 根目錄。
3. 開啟 Settings → Pages。
4. Source 選擇 Deploy from a branch；Branch 選 `main`，資料夾選 `/(root)`，按 Save。

## 注意事項

- 原本兩個網站必須持續公開，整合入口才能載入。
- 兩個來源網址目前同屬 `lionliontomato.github.io`，因此程式會在頁面載入後讀取該頁的原始 favicon。若未來改用不同網域或來源網站禁止 iframe 嵌入，則需調整整合方式。
- 本 ZIP 可檢查入口程式及切換邏輯；由於目前無法從此執行環境直接取得兩個來源網站的即時頁面，因此上線後仍請確認兩個 iframe 都能正常顯示，並確認瀏覽器分頁圖示與實際頁面標題。
