# QuantCraft

[QuantCraft](https://www.quantcraft.cc) is a desktop trading platform for creating, testing, and improving algorithmic trading strategies in Python. You get one workflow for writing code, configuring tests, running backtests, and reviewing results without leaving the app.

This repository hosts **release installers** for QuantCraft **v1.0.0**. For full product documentation, see the [official docs](https://www.quantcraft.cc/documentation/v1?section=introduction).

## What QuantCraft includes

- **Code workspace** - File/folder sidebar, multi-tab Python editor, import/export for `.py` strategy files
- **Python editor** - Strategy authoring with formatting, themes, and a Packages UI for dependencies
- **Run and backtest** - Quick **Run** for script feedback; structured **Backtests** with configurable input parameters
- **Strategy runtime APIs** - Lifecycle callbacks (`on_init`, `on_bar`, `on_tick`, `on_timer`, `on_finish`), simulated account model, OHLCV bar data, fundamentals (when available), and chart indicator series
- **Results and diagnostics** - Output panel, test results (metrics, equity, trades), and export where supported
- **QuantCraft AI** (optional) - In-IDE assistant for explaining, generating, and editing strategy code

Backtests use a **simulated account** (paper behavior, not live brokerage execution). Strategies are Python scripts executed in the QuantCraft runtime context.

## Prerequisites

Before using strategy features, install:

- **Python 3.10+** (3.11 recommended) from [python.org](https://www.python.org/downloads/) - enable **Add Python to PATH** on Windows
- **pip** (usually included with Python)
- Internet access (packages and connected data/services)
- Disk space for projects, logs, and backtest outputs

## Download installers (v1.0.0)

Click a link below to download the installer (direct file URL). After installing, launch QuantCraft and open the strategy IDE/workspace area.

### Windows x64

- [QuantCraft_1.0.0_x64-setup.exe](https://media.githubusercontent.com/media/theallegrarr/quant_craft/main/v1/windows/x64/QuantCraft_1.0.0_x64-setup.exe) - NSIS setup (recommended)
- [QuantCraft_1.0.0_x64_en-US.msi](https://media.githubusercontent.com/media/theallegrarr/quant_craft/main/v1/windows/x64/QuantCraft_1.0.0_x64_en-US.msi) - MSI (enterprise / silent deploy)

### Windows x86 (32-bit)

- [QuantCraft_1.0.0_x86-setup.exe](https://media.githubusercontent.com/media/theallegrarr/quant_craft/main/v1/windows/x86/QuantCraft_1.0.0_x86-setup.exe) - NSIS setup
- [QuantCraft_1.0.0_x86_en-US.msi](https://media.githubusercontent.com/media/theallegrarr/quant_craft/main/v1/windows/x86/QuantCraft_1.0.0_x86_en-US.msi) - MSI (enterprise / silent deploy)

## Documentation

**Start here**

- [Introduction](https://www.quantcraft.cc/documentation/v1?section=introduction) - Product overview and core concepts
- [Getting started](https://www.quantcraft.cc/documentation/v1?section=getting-started) - Install Python, open the app, first strategy and backtest
- [Documentation index](https://www.quantcraft.cc/documentation/v1) - All topics (v1.0, latest)

### Core workflow

1. Create or open a strategy file
2. Write strategy logic and [input parameters](https://www.quantcraft.cc/documentation/v1?section=input-parameters)
3. Run/backtest with selected symbols and date range
4. Review logs, charts, and trade/performance metrics in [test results](https://www.quantcraft.cc/documentation/v1?section=test-results)
5. Adjust and rerun

### Topic guide

| Topic | Documentation |
| :--- | :--- |
| Workspace layout | [workspace-layout](https://www.quantcraft.cc/documentation/v1?section=workspace-layout) |
| Python editor | [python-editor](https://www.quantcraft.cc/documentation/v1?section=python-editor) |
| Import and export | [import-and-export](https://www.quantcraft.cc/documentation/v1?section=import-and-export) |
| Dependencies | [dependencies](https://www.quantcraft.cc/documentation/v1?section=dependencies) |
| Running code | [running-code](https://www.quantcraft.cc/documentation/v1?section=running-code) |
| Backtests | [backtests](https://www.quantcraft.cc/documentation/v1?section=backtests) |
| Strategy lifecycle | [strategy-lifecycle](https://www.quantcraft.cc/documentation/v1?section=strategy-lifecycle) |
| Account model | [account-model](https://www.quantcraft.cc/documentation/v1?section=account-model) |
| OHLCV and bar data | [ohlcv-and-bar-data](https://www.quantcraft.cc/documentation/v1?section=ohlcv-and-bar-data) |
| Fundamentals | [fundamentals](https://www.quantcraft.cc/documentation/v1?section=fundamentals) |
| Indicator series | [indicator-series](https://www.quantcraft.cc/documentation/v1?section=indicator-series) |
| Output panel | [output-panel](https://www.quantcraft.cc/documentation/v1?section=output-panel) |
| Test results | [test-results](https://www.quantcraft.cc/documentation/v1?section=test-results) |
| Optimization | [optimization](https://www.quantcraft.cc/documentation/v1?section=optimization) |
| QuantCraft AI | [quantcraft-ai](https://www.quantcraft.cc/documentation/v1?section=quantcraft-ai) |
| Reference | [reference](https://www.quantcraft.cc/documentation/v1?section=reference) |

## Quick start

1. **Install** - Python 3.10+, then a QuantCraft installer from [Download installers](#download-installers-v100) above
2. **Create a strategy** - New `.py` file in the workspace ([workspace layout](https://www.quantcraft.cc/documentation/v1?section=workspace-layout))
3. **Add callbacks** - `on_init`, `on_bar` (and/or `on_tick`, `on_timer`), `on_finish` ([strategy lifecycle](https://www.quantcraft.cc/documentation/v1?section=strategy-lifecycle))
4. **Define parameters** - Tunable values via [input parameters](https://www.quantcraft.cc/documentation/v1?section=input-parameters)
5. **Run a backtest** - Symbol(s), timeframe, date range; use **Test** and watch the [output panel](https://www.quantcraft.cc/documentation/v1?section=output-panel)
6. **Inspect results** - Logs, [test results](https://www.quantcraft.cc/documentation/v1?section=test-results), indicator overlays; iterate

Your setup is healthy when Python scripts run without import errors, backtests complete with result panels, and logs/charts match expected behavior.

## Practical tips

- Start simple; add complexity after baseline logic is stable
- Use input parameters instead of hardcoding tunable constants
- Log entry/exit decisions for easier debugging
- Validate on multiple symbols and date ranges before trusting performance
- Treat unusually strong backtest results as suspicious until stress-tested

## Links

- Website: [quantcraft.cc](https://www.quantcraft.cc)
- Documentation: [Introduction](https://www.quantcraft.cc/documentation/v1?section=introduction)
- Privacy policy: [Privacy Policy](https://www.quantcraft.cc/privacy-policy)
- Terms of service: [Terms of Service](https://www.quantcraft.cc/terms-of-service)

---

QuantCraft installers in this repository are version **1.0.0**.
