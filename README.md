# Exposure-aware Cascading Bandits

This page presents the additional experimental results of paper: **Mitigating Exposure Bias in Online Learning to Rank Recommendation: A Novel Reward Model for Cascading Bandits**

## Experimental results of RQ1 on MovieLens dataset

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_exploration.png" width="800"/>
<!-- ![alt text](/images/img_r2y_exploration.png?raw=true) -->

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_clicks.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_regret.png" width="400"/>

<!-- ![alt-text-1](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_clicks.png?raw=true "title-1") ![alt-text-2](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_regret.png?raw=true "title-2") -->

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equality_b.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equality_p.png" width="400"/>

<!-- ![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_b.png?raw=true)

![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_p.png?raw=true) -->

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equity_b.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equity_p.png" width="400"/>

<!-- ![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_b.png?raw=true)

![alt text](https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_p.png?raw=true) -->

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

## (RQ2) Comparison to baselines on MovieLens dataset

Performance of our EALinUCB with three different weight functions and the baselines on **MovieLens** dataset for $𝑑 = 10$ and $𝐾 = 5$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    |$\textbf{0.2166}$|0.329 | 0.3081 | 0.0506 | 0.0476 |
| EARSLinUCB | - | 0.2165 | 0.3257 | 0.3257 | 0.0495 | 0.0495 |
|FRMLinUCB | - | 0.2005 | 0.3334 | 0.4586 | 0.0504 | 0.0505 | 
|EALinUCB (ours) | Log | 0.2105 | 0.3799 | $\textbf{0.524}^*$ | $\textbf{0.055}$ | $\textbf{0.0546}$ |
|EALinUCB (ours) | RBP | $\textbf{0.2166}$ | 0.329 | 0.472 | 0.0506 | 0.0515 | 
|EALinUCB (ours) | Linear | 0.2069 | $\textbf{0.392}^*$ | 0.5142 | 0.0545 | 0.0535 | 

<br/>

Performance of our EALinUCB with three different weight functions and the baselines on **MovieLens** dataset for $𝑑 = 10$ and $𝐾 = 10$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    | $\textbf{0.3722}$ | 0.3974 | 0.3656 | 0.0555 | 0.0507 |
| EARSLinUCB | - | 0.3721 | 0.3974 | 0.3848 | 0.0562 | 0.0541 |
|FRMLinUCB | - | 0.3574 | 0.4029 | 0.4157 | 0.0572 | 0.055 | 
|EALinUCB (ours) | Log | 0.3605 | 0.494 | $\textbf{0.514}^*$ | $\textbf{0.065}^*$ | $\textbf{0.065}^*$ |
|EALinUCB (ours) | RBP | $\textbf{0.3722}$ | 0.4074 | 0.434 | 0.0555 | 0.0557 | 
|EALinUCB (ours) | Linear | 0.3585 | $\textbf{0.498}^*$ | 0.5062 | 0.0601 | 0.0604 | 


<br/>

Performance of our EALinUCB with three different weight functions and the baselines on **MovieLens** dataset for $𝑑 = 20$ and $𝐾 = 5$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    |$\textbf{0.2343}$ | 0.4107 | 0.3891 | 0.0606 | 0.0579 |
| EARSLinUCB | - | $\textbf{0.2343}$ | $\textit{0.4271}$ | 0.4071 | 0.0592 | 0.0592 |
|FRMLinUCB | - | 0.2142 | 0.4137 | 0.4613 | 0.0607| 0.0597 | 
|EALinUCB (ours) | Log | $\textit{0.2275}$ | 0.4213 | $\textit{0.5811}$ | $\textbf{0.0641}$ | $\textbf{0.0639}$ |
|EALinUCB (ours) | RBP | $\textbf{0.2343}$ | 0.4107 | $\textbf{0.6109}$ | 0.0606 | 0.0579 | 
|EALinUCB (ours) | Linear | 0.2212 | $\textbf{0.5049}^*$ | 0.5017 | $\textit{0.0629}$ | $\textit{0.0617}$ | 

<br/>

Performance of our EALinUCB with three different weight functions and the baselines on **MovieLens** dataset for $𝑑 = 20$ and $𝐾 = 10$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    |$\textit{0.3975}$ | 0.5011 | 0.4671 | 0.0655 | 0.0617 |
| EARSLinUCB | - | $\textbf{0.398}$ | 0.523 | 0.503 | 0.0656 | 0.0656 |
|FRMLinUCB | - | 0.3775 | 0.5249 | 0.0658 | 0.0214 | 0.0201 | 
|EALinUCB (ours) | Log | 0.3881 | $\textbf{0.5283}$ | 0.4775 | 0.0731 | 0.0728 |
|EALinUCB (ours) | RBP | $\textit{0.3975}$ | 0.5011 | 0.5329 | 0.0654 | 0.0617 | 
|EALinUCB (ours) | Linear | 0.3878 | $\textbf{0.5583}$ | 0.4456 | 0.0674 | 0.0673 | 


<br/>




<br/>

Performance of our EALinUCB with three different weight functions and the baselines on **Yahoo Music** dataset for $𝑑 = 20$ and $𝐾 = 10$. For all metrics, higher value is more desired. $*$ indicates that the result is significant with 𝑝 < 0.01.
| Method | Weight function | $clicks$ | $Equality^{(B)}$ | $Equality^{(P)}$ | $Equity^{(B)}$ | $Equity^{({P})}$
| :---:   | :---: | :---: | :---: | :---: | :---: | :---: |
| LinUCB  |  -    | 0.3154 | 0.4469 | 0.404 | 0.4429 | 0.4002 |
| EARSLinUCB | - | 0.3157 | 0.4467 | 0.4467 | 0.4429 | 0.4429 |
|FRMLinUCB | - | 0.3085 | 0.4517 | 0.4596 | 0.4517 | 0.4498 | 
|EALinUCB (ours) | Log | 0.3073 | $\textbf{0.495}^*$ | 0.5174 | $\textbf{0.485}^*$ | $\textbf{0.473}^*$ |
|EALinUCB (ours) | RBP | $\textbf{0.3171}$ | 0.4489 | $\textbf{0.553}^*$ | 0.4614 | 0.4585 | 
|EALinUCB (ours) | Linear | 0.3008 | 0.4552 | 0.5312 | 0.461 | 0.4542 | 

<br/>

### Additional results corresponding to Figure 3

Comparison of LinUCB and EALinUCB with three weight functions in terms of clicks, n-step-regret, and exposure bias metrics per round on **MovieLens** dataset for $𝑑 = 10$, $𝐾 = 10$, $\alpha = 0.25$, and $\gamma = 0$. For exposure bias metrics, at each round $𝑡$, the metric value is computed over the accumulated exposure up to round $𝑡$.

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_clicks_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_regret_ea.png" width="400"/>

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equality_b_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equality_p_ea.png" width="400"/>

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equity_b_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_ml_cum_equity_p_ea.png" width="400"/>

<br/>

Comparison of LinUCB and EALinUCB with three weight functions in terms of clicks, n-step-regret, and exposure bias metrics per round on **Yahoo Music** dataset for $𝑑 = 10$, $𝐾 = 10$, $\alpha = 0.25$, and $\gamma = 0$. For exposure bias metrics, at each round $𝑡$, the metric value is computed over the accumulated exposure up to round $𝑡$.

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_clicks_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_regret_ea.png" width="400"/>

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_b_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equality_p_ea.png" width="400"/>

<img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_b_ea.png" width="400"/> <img src="https://github.com/masoudmansoury/ealinucb/blob/main/images/img_r2y_cum_equity_p_ea.png" width="400"/>
