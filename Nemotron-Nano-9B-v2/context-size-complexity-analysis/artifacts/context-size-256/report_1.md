# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 177.59 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 130
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 1947.82 GFLOPs
- Эффективная производительность: 10.97 TFLOPs

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
| 0 | 6.84 | 1 | 8.45 |
| 2 | 8.40 | 3 | 9.04 |
| 4 | 8.46 | 5 | 9.04 |
| 6 | 8.46 | 7 | 8.46 |
| 8 | 9.11 | 9 | 8.50 |
| 10 | 9.17 | 11 | 8.60 |
| 12 | 9.16 | 13 | 8.56 |
| 14 | 0.00 | 15 | 9.08 |
| 16 | 8.47 | 17 | 9.13 |
| 18 | 8.48 | 19 | 9.15 |
| 20 | 8.52 | 21 | 0.00 |
| 22 | 9.16 | 23 | 8.56 |
| 24 | 9.15 | 25 | 8.56 |
| 26 | 9.18 | 27 | 8.53 |
| 28 | 9.14 | 29 | 8.49 |
| 30 | 0.00 | 31 | 8.82 |
| 32 | 8.53 | 33 | 9.20 |
| 34 | 8.61 | 35 | 9.20 |
| 36 | 8.54 | 37 | 9.04 |
| 38 | 8.54 | 39 | 0.00 |
| 40 | 9.00 | 41 | 8.18 |
| 42 | 9.07 | 43 | 8.43 |
| 44 | 8.36 | 45 | 9.06 |
| 46 | 8.52 | 47 | 9.13 |
| 48 | 8.49 | 49 | 9.19 |
| 50 | 8.58 | 51 | 9.12 |
| 52 | 8.62 | 53 | 9.23 |
| 54 | 8.63 | 55 | 9.22 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 200.180 | 0.8272 |
| NemotronHRMSNorm | 114 | 25.717 | 0.2256 |
| MambaRMSNormGated | 54 | 14.370 | 0.2661 |
| ReLUSquaredActivation | 50 | 4.308 | 0.0862 |
| Embedding | 2 | 0.285 | 0.1427 |

## Самые медленные модули (20)
- 5.849 ms — `lm_head` (Linear)
- 5.760 ms — `lm_head` (Linear)
- 1.697 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.245 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.192 ms — `backbone.layers.41.mixer.in_proj` (Linear)
- 1.179 ms — `backbone.layers.43.mixer.in_proj` (Linear)
- 1.176 ms — `backbone.layers.16.mixer.in_proj` (Linear)
- 1.171 ms — `backbone.layers.4.mixer.in_proj` (Linear)
- 1.167 ms — `backbone.layers.46.mixer.in_proj` (Linear)
- 1.162 ms — `backbone.layers.7.mixer.in_proj` (Linear)
- 1.161 ms — `backbone.layers.9.mixer.in_proj` (Linear)
- 1.161 ms — `backbone.layers.2.mixer.in_proj` (Linear)
- 1.159 ms — `backbone.layers.18.mixer.in_proj` (Linear)
- 1.159 ms — `backbone.layers.20.mixer.in_proj` (Linear)
- 1.159 ms — `backbone.layers.6.mixer.in_proj` (Linear)
- 1.158 ms — `backbone.layers.16.mixer.in_proj` (Linear)
- 1.157 ms — `backbone.layers.6.mixer.in_proj` (Linear)
- 1.154 ms — `backbone.layers.44.mixer.in_proj` (Linear)
- 1.152 ms — `backbone.layers.2.mixer.in_proj` (Linear)
- 1.152 ms — `backbone.layers.20.mixer.in_proj` (Linear)
