# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 379.54 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 1014
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 15193.00 GFLOPs
- Эффективная производительность: 40.03 TFLOPs

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
| 0 | 28.15 | 1 | 29.55 |
| 2 | 29.21 | 3 | 28.81 |
| 4 | 28.60 | 5 | 29.39 |
| 6 | 28.81 | 7 | 28.87 |
| 8 | 28.30 | 9 | 28.87 |
| 10 | 28.37 | 11 | 28.47 |
| 12 | 28.48 | 13 | 28.49 |
| 14 | 0.00 | 15 | 28.41 |
| 16 | 28.66 | 17 | 28.29 |
| 18 | 28.33 | 19 | 28.22 |
| 20 | 28.75 | 21 | 0.00 |
| 22 | 28.58 | 23 | 28.63 |
| 24 | 27.61 | 25 | 28.37 |
| 26 | 28.18 | 27 | 28.44 |
| 28 | 28.19 | 29 | 28.50 |
| 30 | 0.00 | 31 | 27.92 |
| 32 | 28.22 | 33 | 27.72 |
| 34 | 27.69 | 35 | 27.75 |
| 36 | 28.16 | 37 | 27.98 |
| 38 | 28.24 | 39 | 0.00 |
| 40 | 27.58 | 41 | 28.32 |
| 42 | 28.11 | 43 | 28.42 |
| 44 | 28.34 | 45 | 28.17 |
| 46 | 28.66 | 47 | 28.43 |
| 48 | 28.54 | 49 | 27.80 |
| 50 | 28.03 | 51 | 27.98 |
| 52 | 28.27 | 53 | 28.15 |
| 54 | 28.41 | 55 | 28.23 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 508.913 | 2.1029 |
| NemotronHRMSNorm | 114 | 33.052 | 0.2899 |
| MambaRMSNormGated | 54 | 25.080 | 0.4644 |
| ReLUSquaredActivation | 50 | 21.324 | 0.4265 |
| Embedding | 2 | 0.499 | 0.2493 |

## Самые медленные модули (20)
- 15.894 ms — `lm_head` (Linear)
- 15.818 ms — `lm_head` (Linear)
- 3.255 ms — `backbone.layers.4.mixer.in_proj` (Linear)
- 3.153 ms — `backbone.layers.6.mixer.in_proj` (Linear)
- 3.142 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 3.112 ms — `backbone.layers.7.mixer.in_proj` (Linear)
- 3.069 ms — `backbone.layers.36.mixer.in_proj` (Linear)
- 3.064 ms — `backbone.layers.27.mixer.in_proj` (Linear)
- 3.063 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 3.062 ms — `backbone.layers.9.mixer.in_proj` (Linear)
- 3.062 ms — `backbone.layers.32.mixer.in_proj` (Linear)
- 3.061 ms — `backbone.layers.11.mixer.in_proj` (Linear)
- 3.058 ms — `backbone.layers.13.mixer.in_proj` (Linear)
- 3.057 ms — `backbone.layers.25.mixer.in_proj` (Linear)
- 3.057 ms — `backbone.layers.41.mixer.in_proj` (Linear)
- 3.054 ms — `backbone.layers.34.mixer.in_proj` (Linear)
- 3.054 ms — `backbone.layers.29.mixer.in_proj` (Linear)
- 3.049 ms — `backbone.layers.50.mixer.in_proj` (Linear)
- 3.043 ms — `backbone.layers.34.mixer.in_proj` (Linear)
- 3.030 ms — `backbone.layers.54.mixer.in_proj` (Linear)
