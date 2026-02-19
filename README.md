rader Performance vs Market Sentiment

Primetrade.ai – Junior Data Scientist Assignment

📌 Objective

This project analyzes how Bitcoin market sentiment (Fear/Greed Index) impacts trader behavior and performance on Hyperliquid.

The goal is to identify statistically validated patterns and translate them into actionable trading insights.

🛠 Methodology
1️⃣ Data Preparation

Converted timestamps to datetime format.

Aggregated trade data at daily level.

Aligned trading metrics with daily sentiment classification.

Verified missing values and duplicate handling.

2️⃣ Feature Engineering

Constructed daily metrics including:

Daily PnL

Win rate

Trade frequency

Average trade size

Long/Short ratio

Unique active traders

Drawdown proxy (cumulative PnL vs rolling max)

3️⃣ Sentiment-Based Comparison

Compared Fear vs Greed regimes across:

Profitability

Win rate

Trading intensity

Risk exposure (drawdown)

4️⃣ Statistical Validation

Performed independent t-test on daily PnL:

t-statistic = 2.69

p-value = 0.007

Result: Profitability differs significantly between Fear and Greed regimes.

5️⃣ Trader Segmentation

Segmented traders into:

High vs Low performers

Frequent vs Infrequent traders

Analyzed behavioral differences across sentiment regimes.

🔍 Key Insights

Daily PnL is significantly higher during Greed regimes (p < 0.01).

Trade frequency increases during Greed, indicating more aggressive behavior.

Drawdowns worsen during Fear periods, increasing downside risk.

Low-performing traders show higher sensitivity to sentiment shifts.

📈 Strategy Recommendations

Reduce leverage exposure during Fear regimes.

Increase trade activity selectively during Greed for historically profitable traders.

Tighten risk controls during sentiment transitions (Greed → Fear).

⚠️ Limitations

Analysis is conducted at daily aggregation level.

Broader macro volatility factors are not explicitly modeled.

Findings are specific to Hyperliquid trader behavior.

🚀 How to Run

Clone the repository:

git clone <repo-link>

Install dependencies:

pip install -r requirements.txt

Open the notebook and run all cells.

📄 2️⃣ Short Write-Up (Max 1 Page)

You can either:

Put this as a final markdown section inside the notebook

OR create a file named writeup_summary.md

Below is your 1-page summary:

Executive Summary – Trader Behavior Insights

This analysis investigates the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader performance on Hyperliquid.

Daily trade data was aggregated and aligned with sentiment classification. Key behavioral metrics including PnL, win rate, trade frequency, and drawdown proxy were engineered.

Statistical testing (t = 2.69, p = 0.007) confirms that average daily PnL differs significantly across sentiment regimes. Traders perform better during Greed periods compared to Fear periods.

Behavioral analysis shows that trade frequency and directional bias increase during Greed regimes, indicating higher aggression. Conversely, Fear regimes are associated with sharper drawdowns and reduced profitability.

Segment analysis reveals that low-performing traders are more sensitive to sentiment changes, while high-performing traders demonstrate more stability across regimes.

Strategic Implications

Reduce leverage exposure during Fear periods to mitigate downside risk.

Allow increased activity during Greed regimes, selectively for consistent performers.

Monitor sentiment transitions to tighten risk controls proactively.

This study demonstrates that market sentiment materially influences trader behavior and performance, and can be incorporated into risk-adjusted trading strategies.
