# Анализ моделей Transformer+Mamba

## Структура репозитория

- `Llama-3.1-Nemotron-Nano-4B-v1.1/`
  - `layers-speeds-analysis/` — скрипты и артефакты профилирования времени по слоям.
  - `context-size-complexity-analysis/` — ноутбуки и отчёты по исследованию поведения модели при разных размерах контекста.
    - `artifacts/` — сгенерированные артефакты и отчёты (например, `report_*.md`), организованные по размеру контекста.
    - `src/` — код и ноутбуки анализа (например, `complexity-vs-context-size.ipynb`).
  - `forgetting-analysis/` — ноутбуки для экспериментов по «забыванию» 
  - `latency-throughput-batching/` — ноутбуки и скрипты для измерения задержек, пропускной способности

- `Nemotron-Nano-9B-v2/` — та же структура для версии модели 9B.
  - `context-size-complexity-analysis/`
  - `forgetting-analysis/`
  - `latency-throughput-batching/`
  - `layers-speeds-analysis/`


