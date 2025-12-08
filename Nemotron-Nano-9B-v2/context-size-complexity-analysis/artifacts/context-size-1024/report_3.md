# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 234.20 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 503
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 7536.57 GFLOPs
- Эффективная производительность: 32.18 TFLOPs

## Графики
![](layer_time.png)

![](type_time.png)

![](block_time.png)


## Transformer-блоки
- Размер скрытого пространства: 4480
- Размер внутреннего пространства FFN: None
- Количество голов внимания: None
- Количество K/V голов: None
- Размер головы: None
- Тип внимания: None
- Количество параметров в блоке: 147 374 080
- FLOPs attention: 0.000 GF
- FLOPs FFN: 0.000 GF
### Эффективность по блокам
| Номер блока | Эффективность (TFLOPs) | Номер блока | Эффективность (TFLOPs) |
|---|---|---|---|
| 0 | 22.15 | 1 | 24.45 |
| 2 | 23.61 | 3 | 25.30 |
| 4 | 23.49 | 5 | 25.19 |
| 6 | 23.49 | 7 | 23.47 |
| 8 | 25.15 | 9 | 22.82 |
| 10 | 24.29 | 11 | 23.29 |
| 12 | 24.90 | 13 | 23.92 |
| 14 | 0.00 | 15 | 25.22 |
| 16 | 23.30 | 17 | 25.31 |
| 18 | 23.70 | 19 | 25.11 |
| 20 | 23.73 | 21 | 0.00 |
| 22 | 25.65 | 23 | 23.51 |
| 24 | 25.69 | 25 | 23.99 |
| 26 | 25.64 | 27 | 23.49 |
| 28 | 25.53 | 29 | 23.31 |
| 30 | 0.00 | 31 | 25.42 |
| 32 | 23.88 | 33 | 25.18 |
| 34 | 23.86 | 35 | 25.51 |
| 36 | 23.87 | 37 | 25.57 |
| 38 | 23.73 | 39 | 0.00 |
| 40 | 25.28 | 41 | 23.65 |
| 42 | 25.68 | 43 | 23.87 |
| 44 | 23.85 | 45 | 25.53 |
| 46 | 23.90 | 47 | 25.35 |
| 48 | 23.02 | 49 | 25.04 |
| 50 | 23.59 | 51 | 25.38 |
| 52 | 23.95 | 53 | 25.18 |
| 54 | 23.65 | 55 | 25.23 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 287.387 | 1.1876 |
| NemotronHRMSNorm | 114 | 29.541 | 0.2591 |
| MambaRMSNormGated | 54 | 16.778 | 0.3107 |
| ReLUSquaredActivation | 50 | 6.954 | 0.1391 |
| Embedding | 2 | 0.397 | 0.1984 |

## Самые медленные модули (20)
- 8.522 ms — `lm_head` (Linear)
- 8.417 ms — `lm_head` (Linear)
- 1.858 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.858 ms — `backbone.layers.48.mixer.in_proj` (Linear)
- 1.826 ms — `backbone.layers.9.mixer.in_proj` (Linear)
- 1.814 ms — `backbone.layers.27.mixer.in_proj` (Linear)
- 1.810 ms — `backbone.layers.11.mixer.in_proj` (Linear)
- 1.807 ms — `backbone.layers.18.mixer.in_proj` (Linear)
- 1.805 ms — `backbone.layers.23.mixer.in_proj` (Linear)
- 1.802 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.801 ms — `backbone.layers.9.mixer.in_proj` (Linear)
- 1.800 ms — `backbone.layers.20.mixer.in_proj` (Linear)
- 1.799 ms — `backbone.layers.6.mixer.in_proj` (Linear)
- 1.795 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 1.793 ms — `backbone.layers.29.mixer.in_proj` (Linear)
- 1.792 ms — `backbone.layers.7.mixer.in_proj` (Linear)
- 1.792 ms — `backbone.layers.16.mixer.in_proj` (Linear)
- 1.791 ms — `backbone.layers.16.mixer.in_proj` (Linear)
- 1.787 ms — `backbone.layers.44.mixer.in_proj` (Linear)
- 1.786 ms — `backbone.layers.25.mixer.in_proj` (Linear)
