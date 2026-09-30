# Setup: from subscription to first live trade

There are four steps to a first live trade. Most subscribers are backtesting in 30 minutes and live within a week.

The hard parts (signal logic, session windows, risk controls) are baked into the strategies. Setup is just the mechanical stuff:

- Install the assembly.
- Point it at your broker.
- Pick a session.
- Confirm the backtest output matches what is on the [results page](https://huntersalgo.com/results).

If something looks off, the [Discord](https://huntersalgo.com/discord) answers fastest. The [FAQ](faq.md) has the same answers in writing.

## Step 1: Install on NinjaTrader 8 or TradingView

Download the assembly from your dashboard and import it into NinjaTrader 8, or paste the Pine Script into TradingView. Then activate your hardware-locked licence.

- Site guide: [How to install a NinjaTrader 8 strategy](https://huntersalgo.com/guides/install-ninjatrader-strategy)
- In this repo: [How do I activate my licence?](faq.md#how-do-i-activate-my-licence)

## Step 2: Run your first backtest

1. Open the NinjaTrader 8 Strategy Analyzer.
2. Pick the strategy you want to test.
3. Set commission and slippage to your broker's actual values.
4. Run a 90-day window.

The output you see should match the published backtest within tick-data noise. The published results are on the [results page](https://huntersalgo.com/results). They are hypothetical market replay or backtest results, not live returns.

- Site guide: [Backtesting vs live trading results](https://huntersalgo.com/guides/backtesting-vs-live-trading-results)

## Step 3: Configure session filters and exits

- Decide which New York-time windows you want the strategy to trade.
- Pick your exit mode: static, trailing or ATR-based.
- Set the daily trade cap.

The defaults are sensible for NQ and ES. SI and GC need different session windows.

- Site guide: [How HuntersAlgo session filters work](https://huntersalgo.com/guides/session-filters-explained)
- In this repo: [How do session filters work?](faq.md#how-do-session-filters-work) and [What exit modes are available?](faq.md#what-exit-modes-are-available)

## Step 4: Go live, or paper-test first

Switch the strategy from Sim101 to your live broker connection.

Most subscribers paper-trade for 5 to 7 days first, to confirm fills look the same as the backtest before scaling up. The Discord usually has someone on within minutes during US trading hours if you need a sanity check.

- [Join the Discord](https://huntersalgo.com/discord)

## Where to get help

### Fastest: Discord

The Discord is active during US trading hours. Subscribers and I answer most setup questions within minutes.

<https://huntersalgo.com/discord>

### Slower: email

Use email for licensing or billing issues that need a paper trail. Replies take 1 to 2 business days.

<https://huntersalgo.com/contact>

## If you do not have a subscription yet

The subscription starts with a 3-day trial through Whop. Cancel before day 3 to avoid the renewal charge. The plan and trial terms are on the [pricing page](https://huntersalgo.com/pricing).

---

Mirrored from huntersalgo.com on 30 September 2026. The site is the canonical version.

Futures trading involves substantial risk of loss and is not suitable for every investor. Past performance is not indicative of future results. HuntersAlgo sells software and does not provide financial advice.

<sub>NinjaTrader® is a registered trademark of NinjaTrader Group, LLC. No NinjaTrader company has any affiliation with the owner, developer, or provider of the products or services described herein, or any interest, ownership or otherwise, in any such product or service, or endorses, recommends or approves any such product or service.</sub>
