# Unified Klines Streamer

A service that aggregates closed candles from multi-exchange trade streams (Bybit, BingX, etc.), normalizes them, and fans them out to multiple channels (Redis, RabbitMQ, WebSocket, Webhook, etc.) via pluggable consumers.

## Overview

This project aims to provide a unified interface for streaming candlestick (kline) data from multiple cryptocurrency exchanges. It normalizes the data format across different exchanges and distributes it to various consumers through a pluggable architecture.

## Features (Planned)

- **Multi-Exchange Support**: Connect to multiple exchanges simultaneously

  - Bybit
  - BingX
  - More exchanges to be added

- **Data Normalization**: Standardize candlestick data format across all exchanges

- **Pluggable Consumers**: Flexible output channels

  - Redis Pub/Sub
  - RabbitMQ
  - WebSocket Server
  - Webhook notifications
  - Custom consumer plugins

- **Real-time Streaming**: Process and distribute closed candles in real-time

- **Scalable Architecture**: Designed for high-throughput scenarios

## Project Status

🚧 **This project is currently in early development** 🚧
