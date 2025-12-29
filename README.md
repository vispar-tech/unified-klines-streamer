# Unified Klines Streamer

A Rust service that aggregates closed candles (klines) from multiple cryptocurrency exchange trade streams (such as Bybit, BingX), normalizes their data, and publishes them to different backends (Redis, RabbitMQ, WebSocket, Webhook, etc).

## Overview

This project is written in Rust and provides a unified interface for streaming kline data from several cryptocurrency exchanges. All data is normalized into a single Rust struct and sent through multiple channels.

## Planned Features

-   **Multi-Exchange Integration**:

    -   Connect to several exchanges concurrently (e.g., Bybit, BingX, others).

-   **Data Normalization**:

    -   Unified `Kline` struct for candle data.

-   **Output to Various Systems**:

    -   Redis Pub/Sub publisher
    -   RabbitMQ producer
    -   WebSocket server (tokio + tungstenite)
    -   Webhook dispatcher (reqwest)
    -   Custom Rust consumers

-   **Real-Time Streaming**:

    -   Processes and emits closed candles with low latency using async Rust.

## Project Status

🚧 **Rust implementation in early development** 🚧

PRs, ideas, and community feedback are welcome!
