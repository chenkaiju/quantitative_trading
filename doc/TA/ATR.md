---
title: ATR
parent: Technical Analysis
has_children: false
nav_order: 4
---

# ATR (Average True Range)  

平均真實範圍(ATR)是技術分析中用來測量價格波動率的一個指標。

## TR (True Range)  
在計算ATR之前，要先計算TR，TR的定義是以下三個數字取其大:  
1. 今日最高價減最低價  
    $ R_1 = High_t - Low_t $
2. 今日最高價減昨日收盤價的絕對值  
    $ R_2 = \lvert High_t - Close_{t-1} \rvert $  
3. 今日最低價減昨日收盤價的絕對值  
    $ R_3 = \lvert Low_t - Close_{t-1} \rvert $  

$ TR = max(R_1, R_2, R_3) $  


## ATR的定義  

ATR值為TR值的N日指數移動平均線([EMA](../TA/EMA.md)):  
$ ATR = EMA(TR, N) $  

* TR值必為正  
* ATR值必為正  
* ATR值沒有界線範圍，數值主要呈現波動範圍的幅度  

## ATR指標的用法  

ATR指標的用於表示價格的波動性，並不是用來判斷未來價格的走向，因此，通常會搭配其它的技術指標一起使用。  

* 當趨勢往上，ATR數值也增加時，代表上升趨勢的動能增強。  
* 當趨勢往上，ATR數值卻減少時，代表上升趨勢的動能減弱。  
* 當趨勢往下，ATR數值也增加時，代表下降趨勢的動能增強。  
* 當趨勢往下，ATR數值卻減少時，代表下降趨勢的動能減弱。  



