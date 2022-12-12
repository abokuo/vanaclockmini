# vanaclockmini：顯示 Vana'diel 時間的 JavaScript 程式
    
## 說明
作者：A-Bo Lee (https://abo.tw)

遵循 ES6 語法規定，為了讀取輕量化僅使用 CSS 語法，再匯入 Google 雲端字型美化。

運作參考：えふえふじゅういち時間 JavaScript版 
                                                Copyright (c) 2004 by koji27
                                              http://www.koji27.com/soft/ft/
## 基本定義
1. Vana'diel 起始時間為：天晶曆 934 年 8 月 4 日 1800 時
2. Vana'diel 一年為 360 日，一日為 24 小時，Vana'diel 的時間流速是地球時間的 25 倍。
3. Vana'diel 一週為八日，分別為：火、土、水、風、氷、雷、光、闇。
4. Vana'diel 月相每週變換，分為 12 個階段：二十日月、二十六夜、新月、三日月、七日月、上弦の月、十日月、十三夜、満月、十六夜、居待月、下弦の月。
5. 與 Vana'diel 初始時間相對應的起始地球時間是 2003 年 12 月 1 日 18:00:01。
6. 將當前地球時間減去地球起始時間（加上日本與臺灣的時差一小時加一秒，其他時區請自行轉換），得到的時間換算成秒再乘以 25 就等於 Vana'diel 自起始時間後經過的秒數。
7. 將 $vanaPeriodInSecs 加上 Vana'diel 原始時間（以秒計算）獲得 Vana'diel 當前時間（以秒計算）之後以取餘數除法運算得到當前的 Vana'diel 年、月、日、時、分與秒。
8. 月與日從 1 開始，與電腦計算的初始值：0 不同，因此要換算月與日時需減 1。

## 建議及聯絡
請洽 abokuo at gmail dot com
