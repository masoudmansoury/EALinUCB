# Exposure-aware Cascading Bandits

This page presents the additional experimental results of paper: Mitigating Exposure Bias in Online Learning to Rank Recommendations

## Experimental results of RQ1 on Yahoo Music dataset

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_exploration.png" width="800"/>
<!-- ![alt text](/images/img_r2y_exploration.png?raw=true) -->

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_clicks.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_regret.png" width="400"/>

<!-- ![alt-text-1](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_clicks.png?raw=true "title-1") ![alt-text-2](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_regret.png?raw=true "title-2") -->

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_b.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_p.png" width="400"/>

<!-- ![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_b.png?raw=true)

![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_p.png?raw=true) -->

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_b.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_p.png" width="400"/>

<!-- ![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_b.png?raw=true)

![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_p.png?raw=true) -->

## (RQ2) Comparison to baselines

Performance of our EALinUCB with three different weight functions and the baselines on MovieLens dataset for $𝑑 = 20$ and $𝐾 = 5$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    |$\textbf{0.2166}$|0.329 | 0.3081 | 0.0506 | 0.0476 |
| EARSLinUCB | - | 0.2165 | 0.3257 | 0.3257 | 0.0495 | 0.0495 |
|FRMLinUCB | - | 0.2005 | 0.3334 | 0.4586 | 0.0504 | 0.0505 | 
|EALinUCB (ours) | Log | 0.2105 | 0.3799 | $\textbf{0.524}^*$ | $\textbf{0.055}$ | $\textbf{0.0546}$ |
|EALinUCB (ours) | RBP | $\textbf{0.2166}$ | 0.329 | 0.472 | 0.0506 | 0.0515 | 
|EALinUCB (ours) | Linear | 0.2069 | $\textbf{0.392}^*$ | 0.5142 | 0.0545 | 0.0535 | 