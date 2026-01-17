# High-Frequency Transformer Benchmark

## 🚀 Project Overview
**Can Transformer models handle the microsecond-level latency requirements of High-Frequency Trading (HFT)?**

This project investigates the **inference latency** and **throughput bottlenecks** of state-of-the-art Time-Series Transformers (Informer, Autoformer, PatchTST) on high-frequency Limit Order Book (LOB) data.

Unlike traditional benchmarks that focus on *forecasting accuracy* (MSE), this project focuses on **System Efficiency**:
- **Latency Analysis:** Inference time per tick (P99 latency) on GPU vs. CPU.
- **Throughput:** Maximum ticks processed per second under varying batch sizes.
- **Memory Footprint:** VRAM usage during high-load streaming.

## 🛠️ Tech Stack
- **Data Engineering:** Apache Spark, Polars (for TB-scale LOB data processing)
- **Models:** HuggingFace Transformers, NeuralForecast
- **Infrastructure:** Docker, CUDA Profiling Tools

## 📊 Preliminary Roadmap
- [ ] **Data Pipeline:** Ingesting Binance Level-2 Order Book data (Tick-level).
- [ ] **Baseline:** Benchmarking LSTM vs. Transformer inference speed.
- [ ] **Optimization:** Experimenting with quantization (INT8) and TensorRT for HFT deployment.

## 👤 Author
**Qishi Xing** (Data Engineer & Researcher)
*Focusing on Efficient ML Systems & Quantitative Finance.*
