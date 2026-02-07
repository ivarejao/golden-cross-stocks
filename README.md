# Golden Cross Detection for SPY ETF

A data analysis project to detect "Golden Cross" moments for the SPDR S&P 500 ETF Trust (SPY) over the last 5 years.

## 📊 Project Overview

This project is a hands-on task from [Maven Analytics Data Drills - Turning Bullish](https://mavenanalytics.io/data-drills/turning-bullish). It focuses on identifying potential bull market signals using technical analysis indicators.

## 🎯 What is a Golden Cross?

A **Golden Cross** is a technical chart pattern that indicates the potential for a major rally. It occurs when:
- A short-term moving average (50-day MA) crosses **above** a long-term moving average (200-day MA)
- This crossover signals a shift from bearish to bullish momentum
- It's considered one of the most bullish signals in technical analysis

Conversely, a **Death Cross** occurs when the 50-day MA crosses below the 200-day MA, signaling potential bearish momentum.

## 🔍 Project Objectives

1. Calculate the **50-day moving average** based on closing prices
2. Calculate the **200-day moving average** based on closing prices
3. Identify every **Golden Cross** moment where the 50-day MA crosses above the 200-day MA
4. Analyze historical patterns and potential bull market signals
5. Visualize the data to understand market trends

## 📁 Project Structure

```
golden-cross-stocks/
├── README.md                    # Project documentation (this file)
├── golden_cross_analysis.ipynb  # Jupyter Notebook with analysis
├── LICENSE                      # MIT License
└── .gitignore                   # Git ignore file
```

## 📈 Data Source

The analysis uses historical stock data for the **SPDR S&P 500 ETF Trust (SPY)**, which:
- Tracks the S&P 500 Index
- Is one of the most liquid ETFs in the world
- Provides a good representation of the overall U.S. stock market

Data can be obtained from sources like:
- Yahoo Finance
- Alpha Vantage
- pandas-datareader
- yfinance Python library

## 🛠️ Requirements

To run this project, you'll need:

```bash
# Python 3.7+
pip install jupyter
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install yfinance  # For downloading stock data
```

Or install all dependencies at once:

```bash
pip install jupyter pandas numpy matplotlib seaborn yfinance
```

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ivarejao/golden-cross-stocks.git
   cd golden-cross-stocks
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook golden_cross_analysis.ipynb
   ```

4. **Run the analysis:**
   - Execute cells sequentially
   - Review visualizations and Golden Cross detections
   - Modify parameters as needed

## 📊 Analysis Methodology

The notebook follows this approach:

1. **Data Collection**: Download historical SPY closing prices
2. **Moving Average Calculation**:
   - Calculate 50-day Simple Moving Average (SMA)
   - Calculate 200-day Simple Moving Average (SMA)
3. **Golden Cross Detection**: Identify dates where:
   - Previous day: 50-day MA < 200-day MA
   - Current day: 50-day MA > 200-day MA
4. **Visualization**: Plot closing prices with both moving averages and highlight Golden Cross events
5. **Analysis**: Examine market performance following each Golden Cross

## 📉 Expected Outputs

- Historical price chart with 50-day and 200-day moving averages
- List of dates when Golden Cross occurred
- Performance metrics following each Golden Cross event
- Visual indicators marking each Golden Cross on the chart

## 🎓 Learning Outcomes

Through this project, you will:
- Understand technical analysis indicators
- Learn to calculate and interpret moving averages
- Identify trend reversals using crossover signals
- Gain experience with financial data analysis using Python
- Practice data visualization with stock market data

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Igor Varejão**

## 🙏 Acknowledgments

- [Maven Analytics](https://mavenanalytics.io/) for the data drill challenge
- Data from Yahoo Finance/yfinance
- The technical analysis community for Golden Cross methodology

## 📚 Additional Resources

- [Investopedia: Golden Cross](https://www.investopedia.com/terms/g/goldencross.asp)
- [Maven Analytics Data Drills](https://mavenanalytics.io/data-drills)
- [Technical Analysis of Stocks](https://www.investopedia.com/terms/t/technicalanalysis.asp)

---

**Note**: Past performance and technical indicators do not guarantee future results. This project is for educational purposes only and should not be considered investment advice.
