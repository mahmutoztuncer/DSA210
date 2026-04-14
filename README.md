The Petrol Panic Index

This project investigates the impact of geopolitical tensions—specifically the Hormuz Strait crisis—on global oil market volatility. By correlating real-time news intensity from GDELT with Brent Petrol financial data from Yahoo Finance, we aim to determine if "media panic" serves as a leading indicator for price fluctuations.

Current Progress (April 14, 2026):

As per the project requirements, the following milestones have been completed:

Data Collection: Automated pipelines established for yfinance (financials) and GDELT (global news volume).
EDA (Exploratory Data Analysis): Visualized the relationship between price spikes and news intensity peaks.
Hypothesis Testing: Conducted a T-Test to compare volatility during high-panic vs. low-panic periods.
Robustness: Implemented a rate-limit handler and fallback mechanism for API stability.

To reproduce the analysis, follow these steps:
Install dependencies:pip install -r requirements.txt
Run the analysis:python3 analysis.py

The initial analysis focuses on the March-April 2026 period.
Null Hypothesis(H0): News intensity has no significant effect on petrol price volatility. 
Result: The script outputs a P-Value. If P < 0.05$, we reject H0, suggesting that geopolitical news is a significant driver of market panic.

References & Data Citations
Financial Data: Yahoo Finance. (2026). Brent Crude Oil (BZ=F). finance.yahoo.comNews Data: The GDELT Project. (2026). Global Database of Events, Language, and Tone. gdeltproject.orgTechnical Stack: * yfinance for market data retrieval.gdeltdoc for GDELT API wrapping.SciPy & Pandas for statistical analysis and data manipulation.

AI Disclosure & Transparency
In alignment with academic integrity, I acknowledge the use of AI (Gemini 3) as a collaborative tool for this project. AI assistance was utilized for:
Debugging & Optimization: Resolving `yfinance` MultiIndex column issues and implementing robust rate-limit handlers for the GDELT API.
Documentation: Assisting in the technical structure of this README and refining the project proposal's language.
Statistical Guidance: Conceptualizing the T-Test framework and data merging logic.
