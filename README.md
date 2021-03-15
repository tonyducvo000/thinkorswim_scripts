## ThinkOrSwim Scripts and Scanners

Repo containing collection of ThinkOrSwim scripts and scanners.

* **red_to_green_ratio.txt**  
This script will help quickly evaluate the ratio of red candles to green candles for a given length.  The idea here is
when the number of red outnumber green candles, the bears are winning. In this case, the trader may want to tighten the trailing stop or exit the position if price action moves under the prior day's low.

* **close_to_sma_distance.txt**  
A simple script to use for custom columns. This will calculate the distance between the closing price of the candle bar to a 20 SMA line.  The distance can be used as a way to gauge how strong the bearish/bullish momentum is.

* **TTM_yellow_hist.txt**  
This script is to be used in a custom scan filter.  When applied to a scanning filter, ToS will screen tickers that *currently* have yellow histogram bars in the TTM squeeze indicator; this indicates gaining momentum. See "TTM Squeeze Yellow Hist" in the custom_scanners.txt to see the scanner in action.

* **custom_scanners.txt**  
Custom scanners I have built:  
  **Standard Deviation Dip Scanner**:  This scanner will search tickers that have dipped at least 1 deviation level below the median on a weekly chart.  Great for investors who are interested in dip buying!  
![](screenshots/std_deviation_dip.png)

*  **Momentum Scanner - 3 day consecutive bars**:  This scanner will find tickers that have 3 consecutive green candle bars on a day-to-day time scale (i.e., the stock has been green for the past 3 days).  Useful for catching uptrend early and swing trading. 

* **Momentum Squeeze Above SMA**:  This scanner is a more refined momentum based scanner.  In addition to a momentum filter, this scanner screens for stocks 3% above a 20 SMA and uses a TTM Squeeze alert filter, for potential big price movements. 

* **TTM Squeeze Yellow Hist**:  A scanner with TTM_yellow_hist script (see above) applied to filter.  

* **RSI Oversold Momentum Scanner**:  Another dip based scan.  The dip is found by using an RSI crossover (oversold) with simple average type.  A filter for momentum (i.e., a filter for 3 consecutive green candle bars) is also applied, to screen for tickers where a dip *and recovery* has occurred.

* **52 Week High Gap Up Above SMA Intraday**:  This scanner scans for tickers that have gapped up at their 52 week high, inidicating a very strong bullish momentum.  A filter for openings 3% above the 20 SMA on a 3 minute time scale is also applied, ensuring there is bullish momentum on the intraday.  Good for day traders who are looking for a quick play, at anytime of the market.
  
