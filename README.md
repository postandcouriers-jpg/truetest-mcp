# EA Trade Tester by TrueTest (MCP server)

**Check a trading robot before you risk money. The first read and the verdict are free - no sign-up.**

EA Trade Tester lets an AI assistant send TrueTest your MT5/MT4 Expert Advisor, indicator, Python bot or written
rules, or a finished trading record, and bring back the result: code faults, real trading costs, losing years, and
whether a good backtest is real or luck.

- **Try it free in the browser:** https://truetest.uk/?utm_source=github&utm_medium=readme
- **See a full example first (demo lab):** https://truetest.uk/lab/demo?utm_source=github&utm_medium=readme
- **Sample paid report (PDF, labelled SAMPLE):** https://truetest.uk/sample-report?utm_source=github&utm_medium=readme
- **Free luck bar calculator** (in the browser, nothing uploaded): https://truetest.uk/luck-bar?utm_source=github&utm_medium=readme

## Connect it to your assistant

Server address: `https://truetest.uk/mcp` (remote MCP, streamable HTTP). No account and no sign-in.

In Claude: Settings -> Connectors -> add a custom connector with that address. Other assistants that support remote
MCP servers use the same address. Full setup, examples and sample files: https://truetest.uk/connector

## The three tools

| Tool | What it does | Changes anything? |
|---|---|---|
| `test_strategy_code` | Reads your code (for example the .mq5 with its .mqh includes and .set settings) and lists code faults: wrong server clock, modules never called, settings never used, missing includes, unchecked orders, martingale or grid sizing. With your email it also opens a private Strategy Lab, where our rebuilt copy is backtested on up to 16 years of prices with real costs and a luck check. | Only with your email: it creates your lab. |
| `check_trading_record` | Judges an MT5 Strategy Tester report, an MT4/MT5 statement or a CSV of closed trades: real or luck, allowing for how many versions you tried, with costs, losing years and grid/martingale signs. | No. The record is read and discarded. |
| `get_lab_status` | Says where your lab stands and, once tested, the verdict and its reason. | No. |

## Things you can ask

- "Here is my MT5 Expert Advisor. Does it have any code problems?"
- "Is this backtest real or luck? I tried about 20 settings before this one."
- "What do I get for free?"

## Free and paid

The first read and the lab verdict are free (3 free labs a day per email, up to 10 versions a lab). The detailed
technical report is paid; its price is shown on your lab page before you buy. The assistant never buys anything for you.

## Good to know

- It backtests our own rebuilt copy: it never runs your code as given and never places trades.
- It is not financial advice. Read the results before you risk money.
- Privacy and data kept: https://truetest.uk/privacy - Security: https://truetest.uk/security
- Help: support@truetest.uk

This repository holds the listing files only (`server.json` for the MCP Registry). The service runs at truetest.uk.

Also from us: **WebAISEO** - is your website ready for AI search? https://github.com/postandcouriers-jpg/webaiseo-mcp
