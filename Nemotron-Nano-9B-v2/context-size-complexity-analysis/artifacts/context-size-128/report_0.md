# Llama-3.1-Nemotron-Nano-4B-v1.1

## Общие параметры
- Время forward-pass: 155.07 ms
- Размер скрытого пространства: 4480
- Длина входной последовательности: 61
- Количество Transformer-блоков: 56
- Количество параметров: 8 298 823 680
- FLOPs / forward: 913.98 GFLOPs
- Эффективная производительность: 5.89 TFLOPs

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
| 0 | 0.02 | 1 | 1.11 |
| 2 | 4.28 | 3 | 4.90 |
| 4 | 4.40 | 5 | 5.00 |
| 6 | 4.47 | 7 | 4.48 |
| 8 | 5.07 | 9 | 4.52 |
| 10 | 5.07 | 11 | 4.53 |
| 12 | 5.09 | 13 | 4.48 |
| 14 | 0.00 | 15 | 4.99 |
| 16 | 4.46 | 17 | 5.08 |
| 18 | 4.54 | 19 | 5.08 |
| 20 | 4.55 | 21 | 0.00 |
| 22 | 5.11 | 23 | 4.49 |
| 24 | 5.04 | 25 | 4.49 |
| 26 | 5.02 | 27 | 4.50 |
| 28 | 5.06 | 29 | 4.51 |
| 30 | 0.00 | 31 | 5.05 |
| 32 | 4.52 | 33 | 5.02 |
| 34 | 4.46 | 35 | 5.03 |
| 36 | 4.46 | 37 | 5.04 |
| 38 | 4.47 | 39 | 0.00 |
| 40 | 5.10 | 41 | 1.19 |
| 42 | 5.00 | 43 | 3.88 |
| 44 | 4.41 | 45 | 5.02 |
| 46 | 4.55 | 47 | 5.08 |
| 48 | 4.53 | 49 | 5.05 |
| 50 | 4.52 | 51 | 5.06 |
| 52 | 4.51 | 53 | 5.04 |
| 54 | 4.52 | 55 | 5.10 |

## Сводная таблица времени по типам модулей
| Тип | Кол-во | Суммарное время (мс) | Среднее (мс) |
|-----|--------|------------------------|---------------|
| Linear | 242 | 507.680 | 2.0979 |
| MambaRMSNormGated | 54 | 428.505 | 7.9353 |
| NemotronHRMSNorm | 114 | 82.111 | 0.7203 |
| Embedding | 2 | 59.321 | 29.6605 |
| ReLUSquaredActivation | 50 | 14.976 | 0.2995 |

## Самые медленные модули (20)
- 404.203 ms — `backbone.layers.0.mixer.norm` (MambaRMSNormGated)
- 328.343 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 59.195 ms — `backbone.embeddings` (Embedding)
- 58.245 ms — `backbone.layers.0.norm` (NemotronHRMSNorm)
- 13.090 ms — `lm_head` (Linear)
- 11.406 ms — `backbone.layers.41.mixer.norm` (MambaRMSNormGated)
- 11.321 ms — `backbone.layers.1.mixer.act_fn` (ReLUSquaredActivation)
- 5.274 ms — `lm_head` (Linear)
- 1.604 ms — `backbone.layers.43.mixer.in_proj` (Linear)
- 1.183 ms — `backbone.layers.1.mixer.down_proj` (Linear)
- 1.091 ms — `backbone.layers.0.mixer.in_proj` (Linear)
- 1.030 ms — `backbone.layers.4.mixer.in_proj` (Linear)
- 1.021 ms — `backbone.layers.2.mixer.in_proj` (Linear)
- 1.011 ms — `backbone.layers.4.mixer.in_proj` (Linear)
- 1.011 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 1.011 ms — `backbone.layers.7.mixer.in_proj` (Linear)
- 1.011 ms — `backbone.layers.44.mixer.in_proj` (Linear)
- 1.011 ms — `backbone.layers.16.mixer.in_proj` (Linear)
- 1.006 ms — `backbone.layers.38.mixer.in_proj` (Linear)
- 1.004 ms — `backbone.layers.41.mixer.in_proj` (Linear)
