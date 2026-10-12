# ml-asset-pricing-and-portfolio-optimization
📊 **Can Machine Learning Generate Economic Value in Stock Selection?**

As part of my BrindCo assignment, I implemented a neural-network-based quantitative investment strategy inspired by the research paper *“Do Machine Learning Methods Add Economic Value in Asset Pricing?”*

The project explored a fundamental question in quantitative finance: **Do machine learning models that predict stock returns translate into economically meaningful portfolio performance after accounting for trading costs and investment constraints?**

Using historical daily market data for 481 stocks spanning January 2020 to May 2024, I built an end-to-end pipeline to predict next-month stock returns and evaluate the resulting investment strategies.

**Key components of the project:**

🔹 **Financial Feature Engineering:** Constructed return-based features, including 1-month, 3-month, 6-month and 12-month returns, along with 12–1 momentum signals.

🔹 **Neural Network Modelling:** Implemented an MLP Regressor to estimate future stock returns and rank stocks for portfolio selection.

🔹 **Quantitative Portfolio Construction:** Compared unrestricted stock-selection strategies against economically restricted portfolios incorporating liquidity and volatility filters.

🔹 **Portfolio Performance Evaluation:** Analysed annualised returns, volatility, Sharpe ratios, maximum drawdowns, portfolio turnover and cumulative performance.

🔹 **Transaction Cost Analysis:** Incorporated a baseline round-trip transaction cost of 32 basis points and conducted sensitivity analysis under different cost assumptions.

🔹 **Out-of-Sample Validation:** Implemented expanding-window retraining and a frozen-model holdout experiment to investigate generalisation and the stability of predictive signals.

🔹 **Benchmark Comparison:** Evaluated transaction-cost-adjusted portfolio returns against an equal-weighted market benchmark to distinguish absolute performance from benchmark-relative value creation.

**Key Takeaways:**

The results highlighted an important distinction between predictive accuracy and investment performance. While the neural network exhibited weak standalone cross-sectional predictive power, economically restricted portfolios showed stronger benchmark-adjusted performance in the evaluated holdout period.

The frozen-model experiment, however, produced an Information Coefficient close to zero, underscoring the challenges of signal stability and out-of-sample generalisation. Transaction-cost sensitivity analysis further demonstrated how high portfolio turnover can erode benchmark-adjusted performance.

This project strengthened my understanding of how machine learning, financial feature engineering, portfolio optimisation principles and realistic trading constraints interact in quantitative investment strategies.

**Tech Stack:** Python, Pandas, NumPy, Scikit-learn, Matplotlib, Neural Networks, Quantitative Finance, Portfolio Analytics.

#QuantitativeFinance #MachineLearning #AlgorithmicTrading #AssetPricing #DataScience #PortfolioManagement

