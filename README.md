# trader-sentiment-analysis
This project examines how market sentiment (Fear vs Greed) influences trader performance and behavior, using trading data to uncover patterns and suggest actionable strategies.


# Setup & Run Instructions

## Setup

1. Clone the repository:
Download the .zip file

3. Install required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn

## How to Run

1. Start Jupyter Notebook:
jupyter notebook

2. Open the file:
analysis.ipynb

3. Run all cells to reproduce results and visualizations.




#📄 Write-up


##🧠 Methodology

The analysis began with cleaning and preparing two datasets: market sentiment (Fear/Greed index) and historical trader data. Column names were standardized, missing values and duplicates were handled, and timestamps were converted into a consistent daily format.

Both datasets were then merged on the date field to align trading activity with corresponding market sentiment. Feature engineering was performed to derive key metrics such as daily PnL per trader, win/loss indicator, trade size, trade frequency, and long/short position ratio.

Exploratory data analysis was conducted to compare trader performance and behavior across different sentiment conditions (Fear vs Greed). Additionally, traders were segmented based on activity levels (frequent vs infrequent) to better understand behavioral differences across groups.


##📊 Key Insights

Trader performance varies significantly with market sentiment. Average PnL tends to be higher during Greed periods, indicating more favorable trading conditions in bullish markets.
Win rates decline during Fear and Extreme Fear periods, suggesting increased uncertainty and reduced predictability in market movements.
Traders exhibit higher risk-taking behavior during Greed phases, as reflected by larger trade sizes and increased trading activity.
Frequent traders benefit more during Greed periods but are more negatively impacted during Fear periods, indicating sensitivity to market conditions.


##💡 Strategy Recommendations

During Fear or Extreme Fear periods, traders should adopt a conservative approach by reducing position sizes and limiting trade frequency to manage risk and avoid losses.
During Greed periods, traders can take advantage of stronger market trends by applying momentum-based strategies, while maintaining controlled risk exposure.
Trading activity should be dynamically adjusted based on market sentiment. Frequent traders, in particular, should scale down during bearish conditions and increase participation during bullish phases.
