# LiqCor-trading-bot
Correlation liquidity python app

Uses data normalized from technical models to compute the R-value of certain algorithmic trading signals.  These signals are quantized to ease reverse-engineering profitable states and provide human-readable logs.  The end goal is an FPGA compatible decentralized statistical database, and private trade strategy work, which together with proof-of-profitability provides the foundation for LiqCor coin (which will be a separate project.

This project is in the planning stage.  Our next step is in the creation of a python backend to collect the needed data from Coinbase Pro. (Python and CBP will remain the reference backend until at least the Beta phase.  When this changes, the change will be informed by the most secure and maintainable APIs and languages at the time.  The same logic shall apply to blockchain selection) 

Optionally, this trading bot should support creating and managing limit orders outside the current bid-ask spread by a configurable percentage, for instance .005 or 0.5% to counter coinbase pro's spread taking. 

Although this protocol uses a form of proof-of work to secure any cloud data, it is not pointless work, and it is performed periodically rather than continuously)  The noise-reduced signals and human readable logs can provide reliable information that will support the formation of new financial laws and defi smart-contract strategies, as well as increasing the efficiency of markets.

A love for open-source liberty, a fail-early-and-often mindset, and a game theory or statistical background are the reasons you'll want to contribute to this promising project. Not to mention the possibilities once we're ready to publish the coin. (We will open source the code, but might include a way to secure a configured "donation address" into the miner's behavior, and license keys for removal or customization to enterprise clients.) 

The first feature is selection of monthly trade sizings using either a signals based Kelly formula or user override.
The daily trade features will likely use a private correlation table, generated from miner's account data to weight the signals from each active strategy.
Trades are executed hourly by default, though daily trades will definitely be added next. 

The strategies run hourly, grabbing up to 300 data points for each asset, then quantizing the results. Think sell, underperform, hold, overperform, buy
An example of planned strategies are below:
Macd trend following indicator
Contrarian price extreme market making arbitrage. (buy dips, sell rallies)
Market-cap weighted rebalancing
Order book smoothing
'Volume and Cash flow analysis
Any other useful indicator

If any of these strategies have demonstrated losses in online training, their weight will be negative, suggesting the opposite trades to be generated!


Any action the mining-by-trading bot takes will reflect a heterotelic approach. Getting as many things right as possible at once (just like in a game of blackjack.)
Finally, actual order creation is determined by a state machine, to ensure the executed trades match a sanity check.
