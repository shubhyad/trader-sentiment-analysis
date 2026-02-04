# trader-sentiment-analysis
Exploring how market sentiment impacts trader performance and behavior.


# Trading Behavior Analysis Using Fear & Greed Index

This project analyzes how trader performance and behavior change across different
market sentiment regimes (Fear, Greed, Extreme Fear, Extreme Greed, Neutral).
The analysis is performed using Python and Jupyter Notebook.

The study focuses on:
- Performance differences during Fear vs Greed days
- Behavioral changes in trading activity and risk-taking
- Segmentation of traders based on leverage, frequency, and consistency
- Strategy insights derived from sentiment-driven behavior

---

## Project Structure

- `analysis.ipynb`  
  Main Jupyter Notebook containing data cleaning, merging, analysis, visualizations,
  and answers to all assignment questions.

- `fear_greed_index.csv`  
  Dataset containing daily market sentiment classification.

- `historical_data.csv`  
  **Not uploaded due to large file size.**  
  This dataset contains historical trading data and is required to fully run the notebook.

- `requirements.txt`  
  List of Python libraries required to run the project.

---

## Tools & Libraries Used

- Python
- pandas
- numpy
- matplotlib

---

## How to Run the Project

1. Download or clone this repository from GitHub.

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt



## Summary: Methodology, Insights & Strategy Recommendations
### Methodology
- Merged historical trading data with the Fear & Greed Index using trade date.
- Analyzed trader performance using metrics such as average PnL, win rate,
  trade frequency, and position size.
- Used trade size as a proxy for leverage due to the absence of explicit leverage data.
- Segmented traders into high vs low leverage, frequent vs infrequent,
  and consistent vs inconsistent groups.
- Visualized results using bar charts and boxplots.
### Key Insights
1. Higher trading activity during Greed and Extreme Greed periods does not lead
   to better performance and increases downside risk.
2. Fear periods are associated with more disciplined trading, higher win rates,
   and smaller drawdowns.
3. Consistent winners outperform by controlling risk and trading selectively,
   rather than increasing trade frequency.
### Strategy Recommendations
1. **Greed-Phase Risk Containment Rule**  
   During Greed and Extreme Greed days, restrict leverage and trade frequency,
   especially for high-leverage and frequent traders.
2. **Fear-Phase Selective Participation Rule**  
   During Fear and Extreme Fear days, allow normal participation for consistent
   winners while reducing activity for inconsistent traders.

