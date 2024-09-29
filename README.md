# Deep Hedging S&P500 Futures
Contains final script of Jupyter notebook performing data pre-processing, analysis and delta and deep hedging of S&amp;P500 futures with expiry on December 15th, 2023.
## Summary
The second worksheet of file 'takehome20902data.xlsx' contains Put and Call options' delta, gamma and price for several strikes. The underlying futures prices (E-MINI S&P500 futures dec 2024) and the "continuous" futures price series are also provided. All options, and the corresponding futures, expire on dec 15th 2023. For details on the security definitions and CME exchange go to

https://www.cmegroup.com/markets/equities/sp/e-mini-sandp500.html

The purpose of the exercise is to define a "statistical" hedging policy, based on the futures, which tries to "beat" the simple delta hedging (deltas and gammas are given for comparison). The futures track the forward, not the spot of the underlying, this has implications on hedging. Hedging should be done option by option.

We use the first 300 observations for training the model and the rest of the sample for testing.

The Colab notebook
1. computes the result of delta hedging each option using the provided deltas.
2. builds an alternative (deep) hedging proposal.
3. compares the results.
4. comments 1-3.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/teopozzii/deep-hedging-sp500/blob/main/TakeHome_FINTECH.ipynb)
