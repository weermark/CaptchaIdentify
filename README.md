# 驗證碼辨識

## 目標

從登入網頁抓取驗證碼，並透過深度學習模型辨識驗證碼，進而達成自動化。

<img src=".\result_pic\投影片2.JPG"/>

<img src=".\result_pic\投影片3.JPG"/>

## 過程

首先，從驗證碼網址抓取驗證碼圖片

<img src=".\result_pic\投影片4.JPG"/>

<img src=".\result_pic\投影片5.JPG"/>

<img src=".\result_pic\投影片6.JPG"/>

把名稱命名為驗證碼內容

<img src=".\result_pic\投影片7.JPG"/>

<img src=".\result_pic\投影片8.JPG"/>

進入程式部分。從資料夾讀取驗證碼圖片，進行切割，讓每張圖片皆為單獨字元。因為每個字元距離皆不同，尤其數字與英文字大小差更多，所以需要不斷調整切割距離與因應數字、英文字而動態改變切割大小。即使如此，仍然有圖片會切到字。

<img src=".\result_pic\投影片9.JPG"/>



接著，把處理後的資料轉灰階、轉陣列、轉成0-1間，減少因數值差異產生的模型錯誤。

<img src=".\result_pic\投影片10.JPG"/>

最後，與標籤一起分成訓練、驗證與測試資料。

<img src=".\result_pic\投影片11.JPG"/>

<img src=".\result_pic\投影片12.JPG"/>