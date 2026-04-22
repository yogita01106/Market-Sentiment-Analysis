## Market Sentiment vs Trader Behavior on Hyperliquid

###  Methodology

This analysis combines two datasets: Bitcoin market sentiment (Fear/Greed Index) and historical trader activity from Hyperliquid. The data was cleaned by handling missing values, removing duplicates, and standardizing timestamps. Both datasets were aligned at a daily level using a common date field.

Key metrics were engineered, including daily PnL per trader, win rate, average trade size (used as a proxy for leverage), trade frequency, and long/short ratios. Sentiment labels were merged with trading data to analyze behavioral and performance differences across market conditions.

Additionally, traders were segmented into groups (frequent vs infrequent, high-risk vs low-risk, consistent vs inconsistent) using aggregated behavioral features. A simple Random Forest model was also built to predict next-day profitability based on sentiment and trading behavior.

---

###  Key Insights

1. **Performance is highest during Extreme Greed**
   Traders achieved the highest average PnL and win rates during Extreme Greed periods, indicating that strong bullish momentum creates favorable trading conditions.

2. **Risk-taking increases during Fear, but with lower efficiency**
   Traders placed significantly larger trades during Fear periods, suggesting aggressive “buy-the-dip” behavior. However, this increased risk did not translate into higher profitability, highlighting inefficient decision-making under negative sentiment.

3. **Overtrading reduces consistency**
   Frequent, high-risk traders generated high profits but showed inconsistent performance, while infrequent and lower-risk traders demonstrated more stable returns.

4. **Behavior shifts with sentiment**
   Traders showed a stronger long bias and increased activity during Greed, whereas Fear periods were characterized by erratic position sizing and less predictable outcomes.

---

###  Strategy Recommendations

1. **Momentum Alignment Strategy (Greed Phases)**
   During Greed or Extreme Greed conditions, traders should align with market trends by increasing participation and maintaining a long bias. However, position sizes should remain controlled to avoid excessive risk.

2. **Defensive Strategy (Fear Phases)**
   During Fear periods, traders should reduce position sizes and avoid overtrading. A focus on selective, high-confidence trades or capital preservation can help mitigate losses caused by emotional decision-making.

---

### Conclusion

Market sentiment significantly influences both trader behavior and performance. While bullish conditions enhance profitability, bearish conditions trigger riskier but less effective strategies. Adopting sentiment-aware trading rules and maintaining disciplined risk management can improve long-term trading outcomes.
