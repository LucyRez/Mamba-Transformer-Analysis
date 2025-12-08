# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 759.09 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 2041
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 30580.78 GFLOPs
- Эффективная производительность: 40.29 TFLOPs

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
| 0 | 26.66 | 1 | 25.89 |
| 2 | 28.16 | 3 | 27.27 |
| 4 | 29.23 | 5 | 26.81 |
| 6 | 28.63 | 7 | 27.75 |
| 8 | 25.44 | 9 | 27.37 |
| 10 | 25.38 | 11 | 27.10 |
| 12 | 25.52 | 13 | 27.27 |
| 14 | 0.00 | 15 | 23.04 |
| 16 | 27.47 | 17 | 25.87 |
| 18 | 27.57 | 19 | 25.76 |
| 20 | 27.61 | 21 | 0.00 |
| 22 | 25.32 | 23 | 27.25 |
| 24 | 25.51 | 25 | 27.33 |
| 26 | 25.65 | 27 | 27.19 |
| 28 | 25.38 | 29 | 27.44 |
| 30 | 0.00 | 31 | 25.65 |
| 32 | 27.46 | 33 | 25.78 |
| 34 | 27.60 | 35 | 25.81 |
| 36 | 27.83 | 37 | 26.10 |
| 38 | 27.40 | 39 | 0.00 |
| 40 | 25.02 | 41 | 27.84 |
| 42 | 26.13 | 43 | 28.20 |
| 44 | 28.11 | 45 | 26.11 |
| 46 | 27.77 | 47 | 25.89 |
| 48 | 27.78 | 49 | 25.93 |
| 50 | 28.03 | 51 | 26.24 |
| 52 | 28.34 | 53 | 26.22 |
| 54 | 27.32 | 55 | 25.54 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 1031.226 | 4.2613 |
| NemotronHRMSNorm | 114 | 133.651 | 1.1724 |
| ReLUSquaredActivation | 50 | 53.845 | 1.0769 |
| MambaRMSNormGated | 54 | 40.491 | 0.7498 |
| Embedding | 2 | 0.727 | 0.3634 |

## Самые медленные модули (20)
- 35.410 ms — `lm_head` (Linear)
- 34.938 ms — `lm_head` (Linear)
- 7.419 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 6.811 ms — `backbone.layers.2.mixer.in_proj` (Linear)
- 6.714 ms — `backbone.layers.15.mixer.up_proj` (Linear)
- 6.478 ms — `backbone.layers.27.mixer.in_proj` (Linear)
- 6.465 ms — `backbone.layers.16.mixer.in_proj` (Linear)
- 6.464 ms — `backbone.layers.23.mixer.in_proj` (Linear)
- 6.458 ms — `backbone.layers.11.mixer.in_proj` (Linear)
- 6.422 ms — `backbone.layers.25.mixer.in_proj` (Linear)
- 6.379 ms — `backbone.layers.54.mixer.in_proj` (Linear)
- 6.370 ms — `backbone.layers.18.mixer.in_proj` (Linear)
- 6.365 ms — `backbone.layers.20.mixer.in_proj` (Linear)
- 6.360 ms — `backbone.layers.13.mixer.in_proj` (Linear)
- 6.306 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 6.306 ms — `backbone.layers.29.mixer.in_proj` (Linear)
- 6.289 ms — `backbone.layers.4.mixer.in_proj` (Linear)
- 6.250 ms — `backbone.layers.9.mixer.in_proj` (Linear)
- 6.207 ms — `backbone.layers.32.mixer.in_proj` (Linear)
- 6.202 ms — `backbone.layers.41.mixer.in_proj` (Linear)
