---
title: "Algorithmic Trading : An Introduction"
seoDescription: "Discover algo trading: automated, precise trades with Python. Learn tickers, orders, analysis, and strategies for emotion-free trading"
datePublished: Sun Feb 12 2023 09:55:51 GMT+0000 (Coordinated Universal Time)
cuid: cle17o7bo000208l6d1na9nan
slug: algorithmic-trading-an-introduction
tags: fintech, algotrading, stockmarket, algo-trading, finance-technology

---

### Algorithmic Trading

**Algorithmic trading,** also known as algo trading, is the use of computer programs to follow a defined set of instructions for placing trades. It is a form of automated trading that allows traders to execute orders with speed and precision. Algo trading helps traders to identify and react to market opportunities faster, reduces emotions, and increases discipline. It also allows traders to track multiple accounts and multiple markets simultaneously.

> In this blog post, we will explore the basics of algo trading and its components. We’ll look at what a ticker is and the difference between quants and technical and fundamental analysis. We’ll also look at the basics of Python, strategies, libraries, backtesting, and paper trades.

I recently did a video on this too. Do check it out

%[https://youtu.be/uvby-fWe8Ts] 

## Ticker

**Let’s start by looking at what a ticker is**. A ticker is the state of an order book in any given instance. The tick includes the trades executed in the given instance with the bid/ask information. For each trading interval, four price points are available: open, high, low, and close. There are two kinds of participants: buyers and sellers. Participants place orders as bid and ask.

**Liquidity can be defined as the flow of bid and ask orders in a given time interval.** If the liquidity is high, it means it is easy to trade in the instrument and the slippage cost will be lower for the participants. The details of the bid and ask and trades at any given time are considered as an order book. The rule of the order book is, that the highest bid price in the market is the best bid and the lowest ask is the best ask. Most of the exchanges follow the price-time priority rule, where the bigger bid and smaller ask will be given precedence in trade execution. If the price is the same for the two orders then the time will factor will be used. The order that arrived earlier will be given priority in trade execution.

### Market & Order Types

There are different types of orders available, such as **market orders, limit orders, stop orders, iceberg orders, fill or kill orders, and immediate or cancel orders.**

* Market orders execute at the current best price available, while limit orders are placed to buy or sell a security at a specific price.
    
* Stop orders are also alternatively called stop-loss orders, which is an order to buy or sell an instrument once the price of the instrument reaches a specified price, known as the stop price.
    
* Iceberg orders are an order type that slices orders of larger quantity (or value) into smaller orders, where each small order, or leg, is sent to the exchange only after the previous order is filled.
    
* Fill or kill (FOK) orders are an order to buy or sell a security that must be filled in its entirety or else canceled.
    
* Immediate or cancel orders (IOC) are an order to buy or sell a security that attempts to execute all or part immediately and then cancels any unfilled portion of the order.
    

### Technical, Fundamental & Quants

Now let’s look at the **difference between quants and technical and fundamental analysis**.

* **Quants** use mathematical and statistical models to analyze financial data and make predictions.
    
* **Technical analysis** is the study of past price movements and trading volumes to identify patterns and make predictions about future price movements.
    
* **Fundamental analysis** is the study of economic and financial factors that can affect the price of a security.
    

### Python

**Python** is a programming language used by quants and traders to develop algo trading systems. It has libraries for data analysis, machine learning, and quantitative analysis.

**Strategies** are the core of algo trading.

* They are the set of rules and conditions that define when and how to enter and exit a trade.
    

**Backtesting** is the process of testing a strategy on historical data to evaluate its performance.

**Paper trading** is the practice of simulating the trading of securities without using actual money.

In conclusion, algo trading is a form of automated trading that allows traders to execute orders with speed and precision. It helps traders to identify and react to market opportunities faster, reduces emotions, and increases discipline.