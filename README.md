# Belt & Braces V8.1

### XAUUSD TradingView Indicator — Community Testing Build

Belt & Braces V8.1 is a TradingView Pine Script indicator designed for structured **XAUUSD (Gold)** analysis.

The project combines trend direction, momentum, scoring, entry conditions, trade planning, exit warnings, market sessions, psychological levels and historical trade review into one system.

**This is a testing build. It is not presented as a guaranteed profitable trading system.**

---

## ⚠️ Important

Belt & Braces V8.1 is a decision-support and testing tool.

It does **not** guarantee profitable trades.

Trading XAUUSD and CFDs carries significant risk. Test the indicator on a **demo account** before considering any live trading.

Never risk money you cannot afford to lose.

---

# What V8.1 Does

V8.1 brings together several components:

* Fast / Medium / Slow EMA trend analysis
* Multi-timeframe direction
* RSI momentum
* ADX trend-strength analysis
* Bull/Bear scoring
* BUY and SELL decision engine
* A-grade and B-grade setups
* Entry, Stop Loss and Take Profit planning
* TP1 / TP2 / TP3 trade targets
* Exit warnings
* London and New York session filtering
* Dynamic entry zones
* Institutional zones
* Psychological price levels
* Historical trade review
* Near-miss / rejected setup diagnostics
* TradingView alerts
* Optional MT5 automation alerts

The current default EMA settings are:

**9 EMA / 21 EMA / 50 EMA**

These are adjustable within the indicator.

---

# Recommended Starting Setup

For community testing, start with the default settings rather than immediately optimising everything.

### Timeframes

The current default structure is:

| Purpose   | Timeframe  |
| --------- | ---------- |
| Execution | 5 minutes  |
| Direction | 15 minutes |
| Macro     | 1 hour     |

These settings are adjustable.

The purpose of testing is to establish how the system behaves **before** making large changes to the settings.

---

# Signal Grades

Belt & Braces can identify different grades of setup.

### A-Grade

Higher-quality setup according to the decision and trade engines.

### B-Grade

A valid setup with a lower classification than an A-grade trade.

The indicator provides separate TradingView alerts for:

* A-Grade BUY
* B-Grade BUY
* A-Grade SELL
* B-Grade SELL
* BUY NOW
* SELL NOW

The grading system should be treated as a **testing classification**, not a guarantee of outcome.

---

# Trade Planning

When a valid trade plan is produced, the system can provide:

* Entry
* Stop Loss
* TP1
* TP2
* TP3

This allows testers to evaluate not simply whether a BUY or SELL signal was correct, but **how the complete trade plan performed**.

---

# Exit Warnings

V8.1 includes an EXIT WARNING system.

An exit warning indicates that an active trade is weakening and should be reviewed.

The warning is intended as a decision-support feature rather than an automatic instruction to close every position.

---

# Market Sessions

The indicator includes optional session filtering.

Current default sessions are:

**London:** 07:00–16:00

**New York:** 13:00–21:00

The session timezone can be configured as:

* Europe/London
* America/New_York
* UTC

---

# Psychological Levels

V8.1 includes a psychological price-level map.

The system can display nearby:

* $25 levels
* $50 levels
* $100 levels

The larger levels are visually emphasised.

These levels are **informational only** and do not directly alter entries, exits or scores.

---

# Historical Trade Review

One of the important purposes of this project is to allow us to examine what the system actually does over historical data.

V8.1 includes a historical trade review facility.

Testers can review previous trades and examine the behaviour of the system rather than relying only on individual screenshots or isolated wins and losses.

---

# Diagnostics

V8.1 also contains optional diagnostic features.

These can show:

* Rejected setups
* Near-miss setups
* The main rule that prevented a setup from qualifying
* Historical trade analysis

Diagnostics are particularly useful during development because a **missed trade can be just as interesting as a winning trade**.

---

# TradingView Alerts

The indicator includes TradingView alert conditions for signals and trade events.

These include:

* A-Grade BUY
* B-Grade BUY
* A-Grade SELL
* B-Grade SELL
* BUY NOW
* SELL NOW
* Stop Hit
* TP3 Hit
* Plan Expired
* EXIT WARNING

For the MT5 automation feature, TradingView should be configured to use:

**Any alert() function call**

---

# MT5 Automation

V8.1 contains an optional MT5 automation bridge.

### Important

Automation is **disabled by default**.

The public testing version contains:

`CHANGE_ME`

as the bridge key.

**Do not replace this with a broker password.**

The bridge key is intended for communication with the user's own bridge system and should be treated as a private credential.

If you are only testing the TradingView indicator, you do **not** need to enable MT5 automation.

---

# How To Install

1. Open TradingView.
2. Open an XAUUSD chart.
3. Open the Pine Editor.
4. Copy the contents of `BeltandBraces_V8.1.pine`.
5. Paste the script into the Pine Editor.
6. Add the indicator to the chart.
7. Start with the default settings.
8. Use historical data to review signals.
9. Record the results.

---

# Community Testing

This repository exists so that we can test Belt & Braces with **real market data and multiple testers**.

We are particularly interested in finding:

### Good signals

* Did the signal work?
* How far did price move?
* Which target was reached?
* How much adverse movement occurred first?

### Bad signals

* Where did the trade fail?
* Was the market ranging?
* Was there a news event?
* Was the signal late?
* Did another condition appear to be misleading the engine?

### Missed signals

These are especially important.

If you see a move that you believe Belt & Braces should have caught, please report it.

### False signals

If the indicator produces a BUY or SELL that you believe should not have occurred, report it.

---

# What To Include In A Test Report

Where possible, include:

* XAUUSD
* Date
* Time
* Timeframe
* BUY or SELL
* A or B grade
* Entry
* Stop
* TP1
* TP2
* TP3
* Result
* Screenshot
* Any relevant market/news context
* What you think the system got right or wrong

This will allow us to compare results rather than relying on opinions.

---

# Development Roadmap

### V8.1

Current community testing build.

Focus:

**Does the system behave as intended?**

### V8.2

Potential improvements will be based on testing evidence.

Possible areas include:

* Signal quality
* Entry timing
* Exit behaviour
* Trade duration
* False signals
* Missed opportunities
* Scoring
* Market-condition filtering

### Future versions

Changes should be based on **test results**, not simply adding more indicators.

---

# Philosophy

The name **Belt & Braces** reflects the idea behind the project:

> Don't rely on one signal.

The system attempts to combine several pieces of information before producing a trade decision.

The aim is not to predict every movement in gold.

The aim is to create a structured process that can be **tested, measured and improved**.

---

# Disclaimer

This project is provided for research, development and educational purposes.

Nothing in this repository constitutes financial advice, investment advice or a recommendation to buy or sell any financial instrument.

Past performance does not guarantee future results.

XAUUSD and leveraged CFD trading can result in substantial losses.

Always conduct your own testing and risk assessment.

---

## Version

**Belt & Braces V8.1**

**Status: Community Testing**

**Instrument: XAUUSD**

**Platform: TradingView / Pine Script v6**
