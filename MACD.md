---
title: MACD
parent: Technical Analysis
has_children: false
nav_order: 2
---

# MACD (Moving Average Convergence Divergence)

應用兩條時間區間不同的EMA，區間較長(ex. $T_1=26$日 )的叫做慢線，區間較短(ex. $T_2=12$日)的叫做快線。  
計算快線和慢線之間的離差狀態(DIF)，  
$$ DIF = EMA(close, T_2) - EMA(close, T_1) $$  

再以時間區間($T_3=9$)對DIF做EMA，最後產生MACD線  
$$ MACD = EMA(DIF, T_3) $$  

> MACD是一種長期和短期的移動平均線即將要收斂或發散的徵兆，主要用來觀測趨勢的強弱變化  

經典參數 $(T_1, T_2, T_3) = (12, 26, 9)$  

反應更敏感的參數 $(T_1, T_2, T_3) = (5, 35, 5)$  

## MACD柱狀體  

$$ MACD\ Bar = DIF - MACD $$  
