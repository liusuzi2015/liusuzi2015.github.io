---
title: ta_lib_study
date: 2019-04-19 20:43:03
categories: 金融
tags: 量化分析

---


## 1 talib介绍

### 1.1 总体

Function Groups

Overlap Studies 重叠的研究
Momentum Indicators 动量指标
Volume Indicators 量指标
Volatility Indicators 波动性指标
Price Transform 价格指标
Cycle Indicators 循环指标
Pattern Recognition 模式识别
Statistic Functions 统计功能
Math Transform 数学变换
Math Operators 数学运算符


#### 1.1.1 Overlap Studies 重叠的研究

BBANDS               Bollinger Bands #布林带
DEMA                 Double Exponential Moving Average #双指数移动平均线
EMA                  Exponential Moving Average #指数滑动平均
HT_TRENDLINE         Hilbert Transform - Instantaneous Trendline #希尔伯特变换瞬时趋势
KAMA                 Kaufman Adaptive Moving Average #卡玛考夫曼自适应移动平均
MA                   Moving average #均线
MAMA                 MESA Adaptive Moving Average #自适应移动平均 
MAVP                 Moving average with variable period #变周期移动平均
MIDPOINT             MidPoint over period #在周期的中点
MIDPRICE             Midpoint Price over period #中间时段价格
SAR                  Parabolic SAR #抛物线转向指标
SAREXT               Parabolic SAR - Extended
SMA                  Simple Moving Average
T3                   Triple Exponential Moving Average (T3)
TEMA                 Triple Exponential Moving Average
TRIMA                Triangular Moving Average
WMA                  Weighted Moving Average

#### 1.1.2 Momentum Indicators 动量指标

ADX                  Average Directional Movement Index
ADXR                 Average Directional Movement Index Rating
APO                  Absolute Price Oscillator
AROON                Aroon
AROONOSC             Aroon Oscillator
BOP                  Balance Of Power
CCI                  Commodity Channel Index
CMO                  Chande Momentum Oscillator
DX                   Directional Movement Index
MACD                 Moving Average Convergence/Divergence
MACDEXT              MACD with controllable MA type
MACDFIX              Moving Average Convergence/Divergence Fix 12/26
MFI                  Money Flow Index
MINUS_DI             Minus Directional Indicator
MINUS_DM             Minus Directional Movement
MOM                  Momentum
PLUS_DI              Plus Directional Indicator
PLUS_DM              Plus Directional Movement
PPO                  Percentage Price Oscillator
ROC                  Rate of change : ((price/prevPrice)-1)*100
ROCP                 Rate of change Percentage: (price-prevPrice)/prevPrice
ROCR                 Rate of change ratio: (price/prevPrice)
ROCR100              Rate of change ratio 100 scale: (price/prevPrice)*100
RSI                  Relative Strength Index
STOCH                Stochastic
STOCHF               Stochastic Fast
STOCHRSI             Stochastic Relative Strength Index
TRIX                 1-day Rate-Of-Change (ROC) of a Triple Smooth EMA
ULTOSC               Ultimate Oscillator
WILLR                Williams' %R

#### 1.1.3 Volume Indicators 量指标


#### 1.1.4 Volatility Indicators 波动性指标


#### 1.1.5 Price Transform 价格指标


#### 1.1.6 Cycle Indicators 循环指标


#### 1.1.7 Pattern Recognition 模式识别

#### 1.1.8 Statistic Functions 统计功能


#### 1.1.9 Math Transform 数学变换


#### 1.1.10 Math Operators 数学运算符



### 1.2 细节

[python-ta-lib](https://github.com/mrjbq7/ta-lib)

talib的简称是Technical Analysis Library，主要功能是计算股价的技术分析指标。先简单看看Talib都给我们提供了那些计算技术指标的函数，按技术指标的类型示例如下：

```python
函数名：CDL2CROWS
名称：Two Crows 两只乌鸦
简介：三日K线模式，第一天长阳，第二天高开收阴，第三天再次高开继续收阴，收盘比前一日收盘价低，预示股价下跌。
例子：integer = CDL2CROWS(open, high, low, close)
```


```python
函数名：CDL3STARSINSOUTH
名称：Three Stars In The South 南方三星
简介：三日K线模式，与大敌当前相反，三日K线皆阴，第一日有长下影线，第二日与第一日类似，K线整体小于第一日，第三日无下影线实体信号，成交价格都在第一日振幅之内，预示下跌趋势反转，股价上升。
例子：integer = CDL3STARSINSOUTH(open, high, low, close)
```


```python
函数名 : MA
名称：Moving average 移动平均值
简介：移动平均值是在一定范围内的价格平均值
例子：ma = MA(close, timeperiod=30, matype=0)
```


```python
函数名：ADX
名称：Average Directional Movement Index 平均趋向指数
简介：ADX指数是反映趋向变动的程度，而不是方向的本身。
例子：adx = ADX(high, low, close, timeperiod=14)
```

```python
函数名：ATR
名称：Average True Range 平均真实波幅
简介：主要用来衡量价格的波动。因此，这一技术指标并不能直接反映价格走向及其趋势稳定性，而只是表明价格波动的程度。
例子：atr = ATR(high, low, close, timeperiod=14)
```

```python
函数名：OBV
名称：On Balance Volume 能量潮
简介：通过统计成交量变动的趋势推测股价趋势
计算公式：以某日为基期，逐日累计每日上市股票总成交量，若隔日指数或股票上涨，则基期OBV加上本日成交量为本日OBV。隔日指数或股票下跌，则基期OBV减去本日成交量为本日OBV
例子：obv = OBV(close, volume)
```


```python

```

```python

```


```python

```


```python

```

## 2 talib使用




## 3 talib原理研究



