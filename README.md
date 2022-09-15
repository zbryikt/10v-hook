# 10v-hook

需要把你的網頁放到 10th.g0v.tw 下嗎？你需要兩步驟


## 設定你的專案庫

 - 在 `repo` -> `settings` -> `webhooks`, 建立一個新的 webhook, 並如下設定:
   - payload url: `https://10th.g0v.tw/extapi/deploy`
   - content type: `application/json`
   - secret: 自己隨便設定一個字串, 記得留存.
   - enable ssl verification on
   - just the push event
   - check `active`
 - 把 `tkirbot` 加入你的 collaborator 中.
 - 確認你的專案有一個 `gh-pages` 分支, 內含想要公開的內容


## 通知 Kirby

在 g0v-tw slack 上, 將您的以下資訊私訊給 tkirby:

 - 專案網址, 如 `https://github.com/zbryikt/10v-hook`
 - 想要的目錄名稱, 如 `hotdog` 會導到 `https://10th.g0v.tw/o/hotdog`
 - 在設定專案庫時隨便設定的一個 secret


## License

MIT
