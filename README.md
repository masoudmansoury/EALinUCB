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

Performance of our EALinUCB with three different weight functions and the baselines on *MovieLens* dataset for $𝑑 = 20$ and $𝐾 = 5$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    |$\textbf{0.2166}$|0.329 | 0.3081 | 0.0506 | 0.0476 |
| EARSLinUCB | - | 0.2165 | 0.3257 | 0.3257 | 0.0495 | 0.0495 |
|FRMLinUCB | - | 0.2005 | 0.3334 | 0.4586 | 0.0504 | 0.0505 | 
|EALinUCB (ours) | Log | 0.2105 | 0.3799 | $\textbf{0.524}^*$ | $\textbf{0.055}$ | $\textbf{0.0546}$ |
|EALinUCB (ours) | RBP | $\textbf{0.2166}$ | 0.329 | 0.472 | 0.0506 | 0.0515 | 
|EALinUCB (ours) | Linear | 0.2069 | $\textbf{0.392}^*$ | 0.5142 | 0.0545 | 0.0535 | 

<br/>

Performance of our EALinUCB with three different weight functions and the baselines on Yahoo Music dataset for $𝑑 = 20$ and $𝐾 = 5$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    |0.1802 | 0.3602 | 0.3316 | 0.3559 | 0.3278 |
| EARSLinUCB | - | 0.1807 | 0.3591 | 0.3591 | 0.3556 | 0.3556 |
|FRMLinUCB | - | 0.1721 | 0.3514 | 0.42 | 0.3514 | 0.3501 | 
|EALinUCB (ours) | Log | 0.1772 | $\textbf{0.3662}$ | 0.5396 | $\textbf{0.3599}$ | $\textbf{0.3641}$ |
|EALinUCB (ours) | RBP | $\textbf{0.1814}$ | 0.365 | 0.5812 | 0.358 | 0.362 | 
|EALinUCB (ours) | Linear | 0.1706 | 0.3661 | $\textbf{0.5879}^*$ | 0.3563 | 0.3582 | 


<br/>

Performance of our EALinUCB with three different weight functions and the baselines on MovieLens dataset for $𝑑 = 20$ and $𝐾 = 10$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    | $\textbf{0.3722}$ | 0.3974 | 0.3656 | 0.0555 | 0.0507 |
| EARSLinUCB | - | 0.3721 | 0.3974 | 0.3848 | 0.0562 | 0.0541 |
|FRMLinUCB | - | 0.3574 | 0.4029 | 0.4157 | 0.0572 | 0.055 | 
|EALinUCB (ours) | Log | 0.3605 | 0.494 | $\textbf{0.514}^*$ | $\textbf{0.065}^*$ | $\textbf{0.065}^*$ |
|EALinUCB (ours) | RBP | $\textbf{0.3722}$ | 0.4074 | 0.434 | 0.0555 | 0.0557 | 
|EALinUCB (ours) | Linear | 0.3585 | $\textbf{0.498}^*$ | 0.5062 | 0.0601 | 0.0604 | 


<br/>

Performance of our EALinUCB with three different weight functions and the baselines on Yahoo Music dataset for $𝑑 = 20$ and $𝐾 = 10$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    | 0.3154 | 0.4469 | 0.404 | 0.4429 | 0.4002 |
| EARSLinUCB | - | 0.3157 | 0.4467 | 0.4467 | 0.4429 | 0.4429 |
|FRMLinUCB | - | 0.3085 | 0.4517 | 0.4596 | 0.4517 | 0.4498 | 
|EALinUCB (ours) | Log | 0.3073 | $\textbf{0.495}^*$ | 0.5174 | $\textbf{0.485}^*$ | $\textbf{0.473}^*$ |
|EALinUCB (ours) | RBP | $\textbf{0.3171}$ | 0.4489 | $\textbf{0.553}^*$ | 0.4614 | 0.4585 | 
|EALinUCB (ours) | Linear | 0.3008 | 0.4552 | 0.5312 | 0.461 | 0.4542 | 


### Additional results corresponding to Figure 3

Comparison of LinUCB and EALinUCB with three weight functions in terms of $Equality^{(𝑃)}$ per round on MovieLens dataset for $𝑑 = 10$, $𝐾 = 10$, $\alpha = 0.25$, and $\gamma = 0$. At each round $𝑡$, $Equality^{(𝑃)}$ is computed over the accumulated exposure up to round $𝑡$.

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_clicks_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_regret_ea.png" width="400"/>

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equality_b_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equity_b_ea.png" width="400"/>

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equity_p_ea.png" width="400"/>
