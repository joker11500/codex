# Grid_EMA_RSI_Trading_Fixed_v6 EA Summary

This document captures the publicly shared description for the **Grid_EMA_RSI_Trading_Fixed_v6.mq5** expert advisor referenced in the ChatGPT share `t_68ecfabd0bd08191bf094212a3cea9c3`.

## Advertised features

- Automatic position sizing at **0.01 lots per $100** of account balance.
- **Grid Step:** 250 points between successive orders.
- **Partial Close:** Close 30% of the volume when floating profit reaches **$0.30**.
- **Trailing Stop:** 30 point distance.
- **Drawdown Protection:** reduce exposure after **27%** equity drawdown.
- **Dashboard:** Gold-themed dashboard positioned in the upper-left of the chart.
- **Multi-Symbol Support:** Designed to operate on **XAUUSD, BTCUSD, and EURUSD**.
- **Aggressive Hedge Mode:** Enables a counter-trend hedge strategy in volatile markets.

## Status

The shared conversation only contains the feature summary. The promised follow-up message with the full `Grid_EMA_RSI_Trading_Fixed_v6.mq5` source code is not present in the share, so the actual implementation is still outstanding.

If additional guidance or the source file becomes available, please update this document and add the implementation to the repository.

## Reported compilation issues

In lieu of the missing source, subsequent attempts to compile partial fragments have surfaced a few critical errors that still
need to be addressed:

- **Type truncation warning**: "possible loss of data due to type conversion from 'long' to 'int'" around line 417 suggests a
  variable is being down-cast without an explicit check.
- **Missing identifiers**: references such as `g_symbols` at line 420 fail to resolve, implying that required global state or
  headers are absent from the shared snippet.

These diagnostics reinforce that the currently available materials are insufficient to produce a working build. Any future code
drop should ensure the full project tree—including all dependent `.mqh` modules and global definitions—is provided so the
remaining issues can be reproduced and fixed.
