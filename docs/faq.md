# FAQ

Most buyers ask the same questions about strategies, licensing and setup. I answer them honestly here.

If something is missing, the [Discord](https://huntersalgo.com/discord) is the fastest way to ask, and the [contact page](https://huntersalgo.com/contact) is the next fastest. For questions about pricing (trial mechanics, refunds, billing intervals), see the [pricing page](https://huntersalgo.com/pricing).

Sections:

- [General](#general)
- [Licensing](#licensing)
- [Trading](#trading)
- [Technical](#technical)

## General

### What is HuntersAlgo?

HuntersAlgo is a suite of automated futures trading strategies built for NinjaTrader 8 and TradingView.

The library covers band breakouts, Nadaraya-Watson kernel regression, EMA trend, momentum, ICT liquidity sweeps and opening-range logic. It is built for NQ, ES, GC and SI, with several strategies that run on any liquid future.

### Which markets are supported?

Most strategies are built for one of these:

- NQ (E-mini Nasdaq-100)
- ES (E-mini S&P 500)
- GC (Gold)
- SI (Silver)

Several run on any liquid futures contract. Each strategy page on the site lists its markets.

### What strategies are available?

- HunterML: machine-learning-tuned NQ futures
- HunterBreakOut: band breakout
- HunterGC: gold-specific NW kernel
- HunterNova: momentum
- HunterEMA: EMA crossover
- HunterSI: silver-tuned
- Hunter4PMBreak: 4 PM session break
- HunterICT: ICT liquidity model
- HunterKillShot: liquidity sweep
- HunterORB: opening range breakout
- HunterFlare: multi-EMA trend
- Hunter3BP: 3-bar play
- HunterASO: Absolute Strength Oscillator

### Do I need prior trading experience?

A basic understanding of futures trading is recommended, including concepts like contracts, margin and order types. I provide setup guides and onboarding resources to help you get started. The [setup guide](setup.md) is the place to begin.

## Licensing

### How does licensing work?

Licences are locked to your hardware ID (HWID). The current device allowance is in the [site FAQ](https://huntersalgo.com/faq).

You can see your registered machines and free a slot yourself on your account page at <https://huntersalgo.com/account/devices>.

### Can I transfer my licence to a new computer?

Yes.

1. Sign in to <https://huntersalgo.com/account/devices> with the emailed link.
2. Deactivate the old device.
3. Launch the strategy on your new machine. The HWID is detected automatically.

Any limit on how often you can transfer is in the [site FAQ](https://huntersalgo.com/faq).

### Is there a free trial?

Yes. The subscription includes a 3-day free trial with full access to everything: the full NinjaTrader 8 library and the available TradingView versions. There are no feature tiers.

A payment method is required at signup through Whop. Cancel before day 3 to avoid the renewal charge.

The plan, billing intervals and trial terms are on the [pricing page](https://huntersalgo.com/pricing).

### What happens when my subscription expires?

Trading automation stops once the subscription lapses. Your strategy configurations and settings are preserved for 90 days, so they are ready if you choose to resubscribe. Current rates are on the [pricing page](https://huntersalgo.com/pricing).

## Trading

### How do session filters work?

Session filters restrict trading to specific New York time windows. They help you avoid low-volume overnight periods or high-volatility events outside your preferred hours. You can configure start and end times per strategy.

### What exit modes are available?

There are three exit modes:

- **Static:** fixed tick-based stops and targets.
- **Trailing:** a dynamic stop that follows price.
- **ATR-based:** stops and targets scaled to the Average True Range.

Break-even automation and partial take-profit are included with every plan.

### What risk management filters are included?

The risk filters are:

- ATR (volatility)
- ADX (trend strength)
- RSI (momentum)
- Volume

You can also set daily trade limits to cap the number of entries per session, and a force-close time to flatten positions before market close.

### Are the strategies fully automated?

On NinjaTrader 8 the strategies are fully automated. They connect directly to your broker and submit orders without manual intervention.

On TradingView the strategies generate webhook alerts that your broker or automation tool can act on.

## Technical

### What are the system requirements for NinjaTrader 8?

You need:

- Windows 10 or later
- a stable internet connection
- an active futures broker account connected to NinjaTrader 8
- a valid NinjaTrader licence

A dedicated machine or VPS is recommended for 24/5 operation.

### How does the TradingView setup work?

I provide Pine Script indicators that run directly on TradingView charts. When a signal triggers, TradingView fires a webhook alert to your designated broker or automation endpoint for order execution.

### How do I activate my licence?

Your licence is the email address on your Whop account. There is no key to copy.

1. Import the strategy add-on in NinjaTrader 8 (Tools, then Import, then NinjaScript Add-On).
2. Add it to a chart.
3. Enter that email when the strategy asks.

Your hardware ID is detected automatically. The [NinjaTrader strategy install guide](https://huntersalgo.com/guides/install-ninjatrader-strategy) on the site walks through the whole flow step by step.

### Can I run multiple strategies simultaneously?

Yes. Each strategy instance runs independently on its own chart and instrument.

Every subscription includes the full strategy library, so you can run them all at the same time with separate configurations per strategy. The device allowance on your licence still applies.

Combined strategies can increase account exposure, so check position limits and test the configuration in simulation.

---

Mirrored from huntersalgo.com on 30 September 2026. The site is the canonical version.

Futures trading involves substantial risk of loss and is not suitable for every investor. Past performance is not indicative of future results. HuntersAlgo sells software and does not provide financial advice.

<sub>NinjaTrader® is a registered trademark of NinjaTrader Group, LLC. No NinjaTrader company has any affiliation with the owner, developer, or provider of the products or services described herein, or any interest, ownership or otherwise, in any such product or service, or endorses, recommends or approves any such product or service.</sub>
