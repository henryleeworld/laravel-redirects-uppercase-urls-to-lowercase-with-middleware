# Laravel 11 使用中介層將大寫網址重新導向為小寫

因為搜尋引擎是認網址，網址就是代表您這一頁的門牌，不管是搜尋引擎最佳化、Google Analytics 邏輯都是以網址來辨別，所以如果您的網址因為有大小寫，就可能會因為使用者手誤輸入錯誤，造成搜尋引擎最佳化、Google Analytics、使用者體驗發生不好的狀況。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/Welcome` 來重新導向網址為小寫 `/welcome`。

----

## 畫面截圖
![](https://i.imgur.com/4YQcE7L.gif)
> 以利搜尋引擎判斷網址參照的網頁是否相同
