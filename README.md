📈  End-to-End Fraud Detection Research Project

Over the past few days, I worked on a synthetic FinTech fraud detection dataset to simulate the real-world challenges of detecting fraudulent transactions — with all the messiness, imbalance, and subtle patterns that come with it.

Project Goal:
Not to get “perfect” metrics, but to implement the complete data science workflow and understand the limitations, trade-offs, and decision-making in model building.

<img width="675" height="452" alt="Screenshot 2025-08-09 at 4 39 02 PM" src="https://github.com/user-attachments/assets/aa5fc149-2578-4e7a-bbd9-6f1ac23eedad" />


🔍 Stages of the Project

1️⃣ Data Understanding & Cleaning

Explored 18k+ transactions, including continuous (amount), categorical (transaction_country), ordinal (hour, day_of_week), and binary (is_fraud) features.
Handled datatype conversions & derived engineered features (log_amount, is_new_device, high_amount_flag).

2️⃣ Exploratory Data Analysis

<img width="777" height="597" alt="Screenshot 2025-08-09 at 11 25 06 AM" src="https://github.com/user-attachments/assets/cbef23a6-0ca9-4e73-a06e-2e641df74660" />
 (EDA)

Histograms, bar charts, correlation heatmaps to uncover trends.
Fraud behavior analysis by transaction amount, device type, and geography.

<img width="675" height="428" alt="Screenshot 2025-08-09 at 10 40 52 PM" src="https://github.com/user-attachments/assets/eab85317-ccc3-4d53-bc77-343383abee7b" />

3️⃣ Inferential Statistics

Applied t-tests, Mann–Whitney U, ANOVA, and Kruskal–Wallis to statistically validate fraud associations.
Learned when to use parametric vs non-parametric tests and how skewness affects results.

4️⃣ Feature Engineering

Created meaningful predictors from transaction time, geography, and device usage.
Applied One-Hot Encoding (OHE) for categorical features before regression modeling.

5️⃣ Regression Analysis

Ran Logistic Regression to identify significant predictors of fraud.
Learned how to interpret coefficients and odds ratios.

<img width="676" height="446" alt="Screenshot 2025-08-08 at 7 47 44 PM" src="https://github.com/user-attachments/assets/0799d449-e786-4c37-94fc-f2240cd06c5d" />


6️⃣ Predictive Modeling

Compared Logistic Regression with XGBoost (kept real-world imbalance intact — no oversampling).
Understood how class imbalance impacts recall and why perfect accuracy isn’t always realistic in fraud detection.


📊 Key Learnings

Real-world datasets are rarely perfectly separable — and that’s okay.
Statistical validation is as important as model performance.
OHE is essential when categorical variables are in play for regression.
Ethical considerations in data balancing — realistic results > artificially inflated metrics.
