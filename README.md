# Option implied volatility
透過二分法搜尋選擇權隱含波動度
## code重點說明
1.  **容許誤差大小**
  - 由於波動度為大於0的任意實數，可能數值有無限多個，故需給定一個誤差範圍，只要一個波動度對應的誤差落在範圍內就停止繼續搜尋
2.  **保護機制**
  - 若搜尋次數>X則停止搜索，避免code出錯時仍會一直執行下去
3.  **畫圖驗證「波動度」和「選擇權價值」之關係是否滿足「單調函數」之條件**
