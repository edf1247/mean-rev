# mean-rev
Mean Reversion Strategy in Python

## Strategy

This is a simple mean reversion strategy that uses the z-score statistic to determine signal. 
We enter a long position if the z-score at previous days close is less than -1.75, and enter a short position if the z-score is greater than 1.75. 

The z-score for a day $i$ is calculated via the following formula:
$\frac{c_i - \bar{x_t}}{\sigma_t}$, where $c_i$ is the days close log return, $\bar{x_t}$ is the SMA, and $\sigma_t$ is the rolling std.

The SMA window is 10.
 
![Returns Graph](./imgs/chart.png)

From the graph, we can see that this simple strategy beats buying and holding, generating returns of 37% over 2 years.

Sharpe: 1.034522565789126