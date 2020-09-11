# Cryptocurrency Backtesting
The following tables list the technical information and tick data available for the backtesting. This document is provided for insight on the support levels that are available for backtesting within executium using technical indicators.  This document is correct as 11th September 2020, this is subject to change. You can view the following endpoint for up to date information `https://api.executium.com/api/v2/backtesting/availability`.

Exchange | Symbol | Executium Symbol Code | Interval | Tick Data | Start Date
------------ | ------------ | ------------ | ------------ | ------------ | ------------
Binance|BTCUSDT|binance-btcusdt|15m|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|1h|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|1m|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|2h|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|30m|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|3m|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|4h|YES|1st January 2018 00:00
Binance|BTCUSDT|binance-btcusdt|5m|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|15m|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|1h|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|1m|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|2h|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|30m|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|3m|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|4h|YES|1st January 2018 00:00
Binance|ETHUSDT|binance-ethusdt|5m|YES|1st January 2018 00:00


# Backtesting Information
The following indicators and candlestick pattern detectors are tested for presence.

Accumulation Distribution Line (ADL), Average Directional Index (ADX),  Average True Range (ATR),  Awesome Oscillator (AO),  Bollinger Bands (BB),  Commodity Channel Index (CCI),  Force Index (FI), Know Sure Thing (KST), Moneyflow Index (MFI),  Moving Average Convergence Divergence (MACD),  On Balance Volume (OBV),  Parabolic Stop and Reverse (PSAR),  Rate of Change (ROC),  Average Gain, Average Loss, Cross Up, Cross Down, Cross Over, Highest, Lowest, Standard Deviation, Sum, Relative Strength Index (RSI),  Simple Moving Average (SMA),  Stochastic Oscillator (KD), Stochastic RSI (StochRSI),  Triple Exponentially Smoothed Average (TRIX),  Typical Price,  Volume Weighted Average Price (VWAP),  Volume Profile (VP),  Exponential Moving Average (EMA),  Weighted Moving Average (WMA),  Wilder’s Smoothing (Smoothed Moving Average, WEMA), WilliamsR and the Ichimoku Cloud. The following candlestick patterns are detected, Soldiers, Bullish Top, Morning (unconfirmed), Shooting Harami Man Abandoned Top, Bearish Engulfing Pattern Gap, Doji, DragonFly Star, Three Top, Tweezer Marubozu, Evening Doji, BullishHarami, Bearish Marubozu, Bearish Engulfiing Spinning Cloud Bottom Hammer, Bearish Man, Hanging Cross, Bullish Line, Bullish Baby, Hammer (unconfirmed), Hanging Hammer, Hammer Star, Shooting Doji (Unconfirmed), Tweezer Star Cover, Downside Star, Morning Inverted White Inverted Black Star, Bearish Spinning Pattern, Bullish Star, Evening Pattern, Dark Harami, Piercing Doji Cross, Bullish Hammer, Bearish Tasuki Crows, Three Doji, GraveStone Harami Hammer, and anything considered Bullish or Bearish.

# Example output

```javascript

{
   "data":{
      "status":true,
      "label":"9th March 2018 21:43:00 until 9th March 2018 21:43:19",
      "from":1520631780323,
      "to":1520631799323,
      "seconds":19,
      "code":"binance-btcusdt",
      "count":13,
      "orderbook":[
         [
            1520631780323,
            9057,
            0.099251,
            9048.06,
            1
         ],
         [
            1520631781776,
            9057,
            0.099251,
            9048.06,
            1
         ],
         [
            1520631782870,
            9057,
            0.099251,
            9055,
            0.036007
         ],
         [
            1520631785135,
            9057,
            0.099251,
            9055,
            0.03655
         ],
         [
            1520631786182,
            9056.91,
            0.000395,
            9055,
            0.047734
         ],
         [
            1520631787370,
            9056.91,
            0.000395,
            9055,
            0.047293
         ],
         [
            1520631789682,
            9056.9,
            1.9,
            9055,
            0.047293
         ],
         [
            1520631790885,
            9056.9,
            1.9,
            9055,
            0.047293
         ],
         [
            1520631791979,
            9056.91,
            0.000395,
            9055,
            0.071579
         ],
         [
            1520631793104,
            9056.91,
            0.000395,
            9056.9,
            0.475922
         ],
         [
            1520631794307,
            9056.63,
            0.037866,
            9055,
            0.071579
         ],
         [
            1520631796573,
            9056.62,
            1,
            9048.05,
            0.14371
         ],
         [
            1520631797792,
            9056.62,
            1,
            9048.05,
            0.143449
         ]
      ]
   },
   "meta":{
      "api_version":2,
      "reqid":"60232G3195DT1599786152",
      "system_version":"2.0.5",
      "endpoint":"backtesting\/orderbook-data",
      "status":200,
      "timezone":"UTC",
      "request":"api\/v2\/backtesting\/orderbook-data",
      "auth_required":false,
      "ms":1599786153848,
      "time":1599786153,
      "process_time":1.090961,
      "process_full":1.092385,
      "requester":"<YOUR-IP>"
   }
}

```

# Visual Data
As follows is an example of output provided by executium backtesting system. The graphs show 10 minutes before the position is opened and 10 minutes worth of data after the position has been closed.

![](https://i.imgur.com/HVhng4t.png)
![](https://i.imgur.com/AaAFFLD.png)
![](https://i.imgur.com/ket6EMe.png)
![](https://i.imgur.com/LLxXrSt.png)
![](https://i.imgur.com/MGjnQxY.png)

Each backtested iteration provides a visual result for users to examine.

# Future updates
Executium is currently working to include dozens of other technical indicators to match our tick data.
