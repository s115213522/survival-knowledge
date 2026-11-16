# 末日生存知識站

以末日生存為主題的基礎防災學習網站。透過 AGENTS.md 統一文章格式與維護流程，讓 AI 可以依相同規則繼續擴充。

- 網頁：https://s115213522.github.io/survival-knowledge/
- Repository：https://github.com/s115213522/survival-knowledge
- 4 篇文章：避難包、飲水與食物清單、照明與電力、重要文件。
- 功能：搜尋、分類篩選、共同文章版型、可儲存的準備清單、手機排版。
- 原生 HTML / CSS / JavaScript，無後端、API key 或即時 LLM。

## 本機開啟
直接開啟 index.html 即可瀏覽。若要使用本機伺服器，在此目錄執行 `python -m http.server 8000`，再開啟 http://localhost:8000 。

## 新增文章
先讀 AGENTS.md，複製 article-template.json 的格式，在 content.js 的 window.ARTICLES 陣列新增物件。首頁、分類、文章頁與總清單會自動產生，不需手動新增卡片或 HTML。

執行 `node validate.cjs`，再以瀏覽器檢查搜尋、篩選、文章連結、勾選儲存與手機版面。

## GitHub Pages
Repository → Settings → Pages → Build and deployment → Deploy from a branch → main → /(root) → Save。部署完成後檢查正式網址。
更新檔案後提交至 main，GitHub Pages 會重新部署。

## 隱私與資料來源
清單只存在目前瀏覽器的 localStorage，不上傳、不跨裝置同步。個人證件與聯絡資料不應上傳到公開 Repository。各篇文章附官方資料來源；本站為課程學習作品，實際災害依官方與現場指示行動。
