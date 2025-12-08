# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 190.11 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 249
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 3730.82 GFLOPs
- Эффективная производительность: 19.62 TFLOPs

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
| 0 | 13.86 | 1 | 15.96 |
| 2 | 14.93 | 3 | 16.71 |
| 4 | 15.12 | 5 | 16.65 |
| 6 | 15.03 | 7 | 15.17 |
| 8 | 16.87 | 9 | 15.17 |
| 10 | 16.73 | 11 | 15.17 |
| 12 | 16.97 | 13 | 15.12 |
| 14 | 0.00 | 15 | 16.59 |
| 16 | 15.07 | 17 | 16.78 |
| 18 | 15.01 | 19 | 16.90 |
| 20 | 15.33 | 21 | 0.00 |
| 22 | 16.65 | 23 | 15.02 |
| 24 | 16.88 | 25 | 15.01 |
| 26 | 16.66 | 27 | 15.05 |
| 28 | 16.80 | 29 | 14.94 |
| 30 | 0.00 | 31 | 16.87 |
| 32 | 14.95 | 33 | 16.34 |
| 34 | 14.80 | 35 | 15.95 |
| 36 | 14.69 | 37 | 16.33 |
| 38 | 14.83 | 39 | 0.00 |
| 40 | 16.29 | 41 | 14.70 |
| 42 | 16.38 | 43 | 14.72 |
| 44 | 14.84 | 45 | 16.33 |
| 46 | 14.58 | 47 | 16.39 |
| 48 | 14.68 | 49 | 16.51 |
| 50 | 14.58 | 51 | 16.62 |
| 52 | 15.17 | 53 | 16.96 |
| 54 | 14.99 | 55 | 16.81 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 240.264 | 0.9928 |
| NemotronHRMSNorm | 114 | 27.546 | 0.2416 |
| MambaRMSNormGated | 54 | 15.000 | 0.2778 |
| ReLUSquaredActivation | 50 | 4.906 | 0.0981 |
| Embedding | 2 | 0.300 | 0.1501 |

## Самые медленные модули (20)
- 26.536 ms — `backbone.layers.14.mixer.k_proj` (Linear)
- 6.207 ms — `lm_head` (Linear)
- 6.167 ms — `lm_head` (Linear)
- 1.424 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.332 ms — `backbone.layers.41.mixer.in_proj` (Linear)
- 1.331 ms — `backbone.layers.27.mixer.in_proj` (Linear)
- 1.331 ms — `backbone.layers.43.mixer.in_proj` (Linear)
- 1.326 ms — `backbone.layers.36.mixer.in_proj` (Linear)
- 1.325 ms — `backbone.layers.48.mixer.in_proj` (Linear)
- 1.323 ms — `backbone.layers.46.mixer.in_proj` (Linear)
- 1.322 ms — `backbone.layers.52.mixer.in_proj` (Linear)
- 1.318 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.317 ms — `backbone.layers.2.mixer.in_proj` (Linear)
- 1.316 ms — `backbone.layers.25.mixer.in_proj` (Linear)
- 1.315 ms — `backbone.layers.54.mixer.in_proj` (Linear)
- 1.314 ms — `backbone.layers.18.mixer.in_proj` (Linear)
- 1.314 ms — `backbone.layers.13.mixer.in_proj` (Linear)
- 1.313 ms — `backbone.layers.9.mixer.in_proj` (Linear)
- 1.313 ms — `backbone.layers.34.mixer.in_proj` (Linear)
- 1.312 ms — `backbone.layers.16.mixer.in_proj` (Linear)
