Trader Performance vs Market Sentiment

What This Project Is About

I wanted to see if Bitcoin's market sentiment (the Fear/Greed Index) actually affects how traders perform on Hyperliquid. Basically, do people trade differently when the market is scared vs when everyone's hyped?


Data I Used :-

Bitcoin Fear/Greed Index
Just dates and what the sentiment was that day

Hyperliquid Trader Data
Individual trades with PnL, position sizes, fees, all that stuff


What I Did :-

I loaded both datasets and checked them out first. Then I made sure the timestamps matched up so I could compare things daily. After that I merged everything together, putting trader activity next to the sentiment data.

I created some metrics to track things like how much money traders made or lost each day, their win rate (basically how often they were right), how many trades they made, average size of their positions, and the fees they paid.

Then I analyzed everything by sentiment category to see if there were patterns.


What I Found :-

Traders actually did better during Fear periods. Their win rates were highest when everyone else was scared, which was kind of surprising.

People traded MORE during Fear, not less. Looks like they see it as an opportunity rather than a time to step back.

Extreme Greed was rough. Performance dropped during these times, probably because people get overconfident and make mistakes.

Neutral markets were boring. Lowest activity overall. Traders seem to like when sentiment is strong either way.


Trading Ideas From This :-

When the market is fearful, this is when traders had the best accuracy. So maybe it's worth being more active during these periods. But you still need to manage risk properly and not go crazy.

When the market is extremely greedy, you need to watch out. This is where people seem to mess up the most. Probably should use less leverage and keep positions smaller.


Running This Yourself :-

Install the stuff you need:
pip install pandas numpy matplotlib seaborn

Open the notebook:
jupyter notebook

Then just run it.


Files :-

The project has a data folder, the main notebook file, and this readme.

Project Structure :-
Trader-Sentiment-Analysis/
 PRIMETRADE.AI/
│── fear_greed_index.csv
│── historical_data.csv
│── project.ipynb
│── readme.md
