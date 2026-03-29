# Malaysia stock market API

Real-time Malaysia stock market API with WebSocket, OHLCV, and snapshot endpoints for MYX.

## Overview

Kun Data provides real-time market data for Malaysia through a token-authenticated API stack designed for charting tools, watchlists, market overview pages, brokerage dashboards, and quant workflows.

This repository focuses on Malaysia market coverage with support for MYX, FTSE.

## API Capabilities

- Real-time WebSocket market data for Malaysia
- Historical OHLCV and candlestick data
- Exchange snapshot endpoint for lists, rankings, and overview pages
- Token-based authentication
- Query and subscribe by `market`, `exchange` or `venue`, `symbol`, and `symbols`

## Integration Model

- WebSocket realtime streaming for live prices and incremental updates
- Historical K-line endpoint with `interval` and `count`
- Exchange snapshot endpoint for batched market views
- Token-based access for HTTP and WebSocket requests

## Supported Exchanges

- `MYX`
- `FTSE`


## Common Use Cases

- Stock charting applications
- Trading terminals
- Watchlists and screeners
- Market movers and overview pages
- Internal financial dashboards

## Why This Repo Exists

Developers often search for terms like:

`Malaysia stock market API | Bursa Malaysia API | Malaysia stock data API | Malaysia OHLCV API`

This repository is designed to make Malaysia market API coverage easier to discover and evaluate.

## Links

- Website: https://kun.pro/stocks-en.html
- Docs: https://kun.pro/docs-en.html
- Main site: https://kun.pro

## Authentication

Your account token is used to access the API. HTTP requests can use bearer authentication, and WebSocket connections pass the token in the query string.

## Notes

- `market` is the access and authorization key for each product
- Historical data uses a single `symbol` in `EXCHANGE:TICKER` format
- Snapshot queries support filtering by market, venue, symbol, and ticker
- WebSocket subscriptions support market-wide or symbol-specific streaming
