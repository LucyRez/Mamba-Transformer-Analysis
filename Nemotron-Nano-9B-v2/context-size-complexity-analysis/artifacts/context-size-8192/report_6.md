# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 1506.98 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 4025
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 60307.51 GFLOPs
- Эффективная производительность: 40.02 TFLOPs

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
| 0 | 30.43 | 1 | 27.85 |
| 2 | 28.83 | 3 | 24.95 |
| 4 | 26.52 | 5 | 24.72 |
| 6 | 27.08 | 7 | 26.85 |
| 8 | 24.61 | 9 | 26.86 |
| 10 | 25.09 | 11 | 27.23 |
| 12 | 25.34 | 13 | 27.42 |
| 14 | 0.00 | 15 | 25.16 |
| 16 | 27.09 | 17 | 24.78 |
| 18 | 26.73 | 19 | 24.73 |
| 20 | 27.01 | 21 | 0.00 |
| 22 | 24.76 | 23 | 26.49 |
| 24 | 24.78 | 25 | 27.05 |
| 26 | 25.33 | 27 | 27.27 |
| 28 | 25.23 | 29 | 27.11 |
| 30 | 0.00 | 31 | 25.26 |
| 32 | 26.91 | 33 | 24.09 |
| 34 | 25.22 | 35 | 23.98 |
| 36 | 26.08 | 37 | 23.85 |
| 38 | 25.39 | 39 | 0.00 |
| 40 | 23.88 | 41 | 25.61 |
| 42 | 23.85 | 43 | 26.40 |
| 44 | 26.21 | 45 | 24.15 |
| 46 | 26.70 | 47 | 25.00 |
| 48 | 26.88 | 49 | 25.33 |
| 50 | 27.10 | 51 | 25.20 |
| 52 | 26.96 | 53 | 24.84 |
| 54 | 26.50 | 55 | 24.37 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 2042.264 | 8.4391 |
| NemotronHRMSNorm | 114 | 353.111 | 3.0975 |
| ReLUSquaredActivation | 50 | 108.450 | 2.1690 |
| MambaRMSNormGated | 54 | 71.538 | 1.3248 |
| Embedding | 2 | 0.881 | 0.4406 |

## Самые медленные модули (20)
- 76.856 ms — `lm_head` (Linear)
- 75.687 ms — `lm_head` (Linear)
- 13.455 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 13.015 ms — `backbone.layers.34.mixer.in_proj` (Linear)
- 12.926 ms — `backbone.layers.41.mixer.in_proj` (Linear)
- 12.832 ms — `backbone.layers.44.mixer.in_proj` (Linear)
- 12.684 ms — `backbone.layers.36.mixer.in_proj` (Linear)
- 12.660 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 12.603 ms — `backbone.layers.41.mixer.in_proj` (Linear)
- 12.483 ms — `backbone.layers.34.mixer.in_proj` (Linear)
- 12.468 ms — `backbone.layers.43.mixer.in_proj` (Linear)
- 12.447 ms — `backbone.layers.7.mixer.in_proj` (Linear)
- 12.437 ms — `backbone.layers.54.mixer.in_proj` (Linear)
- 12.408 ms — `backbone.layers.4.mixer.in_proj` (Linear)
- 12.393 ms — `backbone.layers.52.mixer.in_proj` (Linear)
- 12.360 ms — `backbone.layers.48.mixer.in_proj` (Linear)
- 12.360 ms — `backbone.layers.23.mixer.in_proj` (Linear)
- 12.323 ms — `backbone.layers.36.mixer.in_proj` (Linear)
- 12.310 ms — `backbone.layers.23.mixer.in_proj` (Linear)
- 12.260 ms — `backbone.layers.46.mixer.in_proj` (Linear)
