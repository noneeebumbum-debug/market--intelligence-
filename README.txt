MARKET INTELLIGENCE PRO — ANDROID PWA
======================================
This build adds:
- Live Binance USDⓈ-M Futures ticker stream and live kline updates.
- Interactive TradingView Lightweight Charts chart (pinch/scroll zoom, pan, crosshair).
- Display-only pair suffix .P (the API symbol remains e.g. BTCUSDT).
- Light theme.
- PWA manifest, service worker and app icon for Add to Home Screen / install.
- EMA, Bollinger Bands and VWAP overlays; RSI, ADX, ATR, MACD; volume and range breakout; funding, open interest snapshot and order-book imbalance.
- Central weighted analytical engine with nine departments.
- Manual signal and on-demand scanner.

INSTALL AS AN APP (IMPORTANT)
1. Upload/extract this folder to a static HTTPS host (GitHub Pages is one free option) or serve it from a local HTTPS-capable server.
2. Open the HTTPS URL in Chrome on Android.
3. Chrome menu (three dots) -> Install app or Add to Home screen.
4. Launch Market Intelligence from the new home-screen icon.
A PWA cannot be installed reliably by opening index.html directly from the file manager. Installability requires HTTPS (or localhost).
Chart library loads from unpkg CDN; internet is required. The app shell can cache, but market data and chart library require network.

TRADING SYMBOLS
UI shows BTCUSDT.P; Binance endpoints receive BTCUSDT. The .P suffix is only a visual convention, not an exchange symbol.

LIMITATIONS
- "AI-assisted" here means an explainable weighted rules/statistical engine. There is NO trained machine-learning model or separate server backend in this build.
- Confidence/score is a heuristic, not a calibrated win probability.
- Auto scan ranks the 25 highest-quote-volume eligible pairs, not all contracts deeply.
- OI is a current snapshot, not historical OI change. Funding and order-book data refresh on manual analysis/context refresh.
- No liquidation heatmap, full depth heatmap, full volume profile, backtesting, walk-forward validation, or automatic trading.
- Never treat outputs as guaranteed. Paper trade and validate with fees/slippage before real capital.
- Binance public API/WebSocket availability, rate limits, CORS and network access may vary.
- No API key, account login or order placement.
