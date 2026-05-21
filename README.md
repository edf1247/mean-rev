# mean-rev
Mean Reversion Screener and Strategy in Python

## Screener

I screened the 100 most popular cryptocurrencies for the following information:
- if the correlation coefficient between the z-score and daily return was <= -0.03, the coin was added to the results array

All calculations occured in log space

This resulted in 13 coins being added(stablecoins were removed).

## Strategy

I implemented a simple mean reversion strategy, using the 5 day moving average.

## Results

<img width="1431" height="764" alt="image" src="https://github.com/user-attachments/assets/f1b111f2-93b1-4028-a22f-0c198607e548" />
