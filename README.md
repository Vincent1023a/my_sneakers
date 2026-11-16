# 球鞋圖鑑

以賽博龐克球場為視覺主題的繁體中文球鞋圖鑑，整理鞋款設計、發售資料與配色故事。網站以 Jekyll 將 Markdown 條目轉成網頁。

## 專案結構

| 路徑 | 用途 |
| --- | --- |
| [AGENTS.md](AGENTS.md) | AI 收錄、查證、排版與更新的規則 |
| [index.md](index.md) | 網站首頁 |
| [wiki/index.md](wiki/index.md) | 鞋款索引 |
| [wiki/sneakers/](wiki/sneakers/) | 鞋款條目 |
| [wiki/log.md](wiki/log.md) | 維護日誌 |
| [raw/](raw/) | 原始素材與來源紀錄 |
| [_config.yml](_config.yml) | Jekyll 設定 |
| [_layouts/](_layouts/) 與 [assets/](assets/) | 網頁版型、樣式與圖片 |

## 新增鞋款

在這個專案資料夾開啟 AI 助手，貼上照片、鞋名、鞋標款號或來源連結，請它「依照 AGENTS.md 收錄這雙鞋，補上配色故事並更新圖鑑」。

AI 會保存原始素材，檢查是否已有同款，再查證並新增鞋款條目或補充既有條目的配色。最後更新首頁、索引與維護日誌，並檢查連結和圖片。資料不足時，條目會標示待查證的項目。

## 發布到 GitHub Pages

1. 上傳前確認即將公開的原圖、來源紀錄與網站圖片都可分享。Jekyll 的排除清單只影響生成的網站，公開儲存庫裡的檔案仍可被瀏覽。
2. 將專案檔案上傳到 GitHub 儲存庫的 `main` 分支根目錄。保留 `_config.yml`、`index.md`、`_layouts/`、`wiki/` 和 `assets/` 的目錄位置。
3. 到 **Settings → Pages**，選擇 **Deploy from a branch**，指定 **main** 及 **/(root)** 後儲存。
4. 等候 Pages 完成建置，從 Pages 設定開啟公開網址。檢查首頁能否進到鞋款索引，點開鞋款後確認圖片、配色故事及返回連結。

[GitHub Pages 發布設定說明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
