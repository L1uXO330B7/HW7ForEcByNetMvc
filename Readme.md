# 職訓局 .NET Framework 4.8 MVC 電商網站

## 後台
管理員登入後，在 Session 塞入驗證資料，之後即可在後台暢行，如尚未登入，直接輸入 URL Request，將被 Controller Guard (Custom Attribute) 擋下。
管理員可以在後台做資料表的 CRUD，後台顯示的用戶密碼是已被做過 Hash 雜湊，管理員在刪除時會跳出 Modal 詢問。在更新資料時，使用 Ado.net 處理資料表外鍵條件限制問題。

## 前台 
會員可以瀏覽商品，登入後，可以將商品放入購物車(Local Storage)，再進行下單。下單後，購物車會清空，且彈回商品頁面。

## 資料庫
在會員註冊時，使用預存程序 Stored Procedure 來處理會員編號需要由二位文字與號碼組成的需求。
