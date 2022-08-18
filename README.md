# Fashion-store
服飾店網拍型的合作專案
我負責首頁，客製化，我的最愛功能
資料庫最初的創建

## 首頁
首頁進去前有一個過場動畫，整體頁面主要是用bootstrap切版，利用javascript去微調。網頁  
RWD會根據視窗大小自動適應。旋轉木馬幻燈片是套用 jQuery之家的套件。首頁滾輪滾動一  
次是滑動半張網頁，這是利用網路上的範例滾動一次滑一頁去修改。 然後第四頁的輪播圖會  
抓取資料庫最新6筆商品的圖片來顯示。 

https://user-images.githubusercontent.com/107457598/180911882-175061cf-a3ee-4677-a48a-bcd2fea1f910.mp4

https://user-images.githubusercontent.com/107457598/180912351-d88731bc-f828-4f5c-b91a-04582f4ac59d.mp4


## 客製化
使用者可以自由選擇衣服的底色，上傳圖片，接著拉到衣服上面，超過的部分會遮起來，然後  
利用滾輪去調整圖片大小，一次最多只能上傳兩張圖片，完成客製後可以存到自己的電腦。再  
次上傳最終版本的圖片，下方會有預覽圖顯示，這個動作會將圖片轉成blob格是儲存在 mysql  
中。旁邊選擇要的尺寸與數量並傳到購物車當中。  


https://user-images.githubusercontent.com/107457598/180912370-d1101671-831c-41e9-9b1a-e38e7c21e7db.mp4


## 我的最愛功能
判斷使用者是否登入，未登入產品頁的愛心會顯示黑色無法點擊，登入後一般愛心呈現白色，  
點擊後會呈現紅色並加到資料庫當中，下一次登入一樣會呈現紅色，不需再重新加入。再次點  
擊愛心會變回白色並刪除 mysql的資料。已加的產品會顯示在我的最愛頁面，可以一筆一筆刪  
除也能一次全部清空。  


https://user-images.githubusercontent.com/107457598/180912380-5b7d6317-9682-42a7-aa1e-f1a19ce94e6d.mp4



### 技術點
。JS滾輪事件一次滑動一半頁面  
。HTML5 ondragstart事件連續複製不同的圖片  
。利用 html2canvas 把div轉成canvas變成圖片儲存到電腦  
。FileReader上傳圖片後預覽  
。圖片轉成二進制儲存成blob在mysql中  
。Axios 與 Ajax 傳送資料  
。node.js 應用 multipleStatements: tru


