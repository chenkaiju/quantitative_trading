---
title: EMA
parent: TA
has_children: true
nav_order: 1
---

<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>

  
# EMA (指數移動平均)
離現在越遠的價格，影響力(權重)越小，權重以指數遞減 <br>
EMA公式為:  

$$ EMA_{n} = (K \times C) + ((1-K) \times EMA_{n-1}) $$
$$ C: 今日收盤價 $$
$$ N: 時間週期 $$
$$ K: 加權乘數(smoothing/(N+1)) $$
$$ smoothing: 平滑因子，通常設定為2 $$


| 時間週期 (N) | 加權乘數 (K) |
|:-----| :-----|
| 14|0.133|
| 13|0.143|
|12|0.154|
|11|0.167|
|10|0.182|
|9|0.200|
|8|0.222|
|7|0.250|
|6|0.286|
|5|0.333|
|4|0.400|
|3|0.500|
|2|0.667|
|1|1.000|

## EMA的優缺點
移動平均線(MA)是過去一段時間的平均價格，而EMA是加入權重的MA，他可以更好表示近期價格對於移動平均線的影響力。  

|優點|缺點|
|:-----|:-----|
|適合趨勢型的投資標的|不適用於盤整行情，因為進場訊號不夠清楚|
|經常做為市場價格的支撐或壓力|屬於落後指標|
|與其他指標配合性高，如多重平均線、MACD、布林通道|單一指標只能代表價格成本，須搭配其他指標|