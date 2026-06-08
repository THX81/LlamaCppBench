| model                          |       size |     params | backend    | ngl | threads | type_k | type_v |  fa | mmap |        fitc |            test |                  t/s |
| ------------------------------ | ---------: | ---------: | ---------- | --: | ------: | -----: | -----: | --: | ---: | ----------: | --------------: | -------------------: |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        283.44 ± 1.48 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |      1496.75 ± 18.10 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         25.32 ± 0.05 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         23.97 ± 0.03 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        284.33 ± 0.40 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |       1501.63 ± 5.49 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         25.33 ± 0.02 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         23.98 ± 0.02 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        283.94 ± 0.70 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |       1496.37 ± 2.90 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         25.33 ± 0.04 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         23.95 ± 0.02 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        283.75 ± 0.43 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |      1491.17 ± 16.81 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         25.32 ± 0.05 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         23.95 ± 0.02 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        283.60 ± 0.76 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |      1483.66 ± 38.99 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         25.32 ± 0.06 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         23.97 ± 0.03 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        283.70 ± 0.77 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |      1489.21 ± 33.12 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         25.32 ± 0.05 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         23.97 ± 0.02 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        283.56 ± 0.74 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |      1489.51 ± 39.98 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         25.31 ± 0.06 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         23.95 ± 0.03 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        284.26 ± 0.59 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |      1490.58 ± 32.04 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         25.31 ± 0.07 |
| qwen3 14B Q4_K - Medium        |   8.38 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         23.95 ± 0.02 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        324.89 ± 0.97 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2368.13 ± 315.38 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         28.92 ± 0.09 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         28.77 ± 0.04 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        322.83 ± 1.43 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2362.63 ± 320.73 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         28.86 ± 0.07 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         28.74 ± 0.05 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        321.18 ± 0.91 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2358.68 ± 325.59 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         28.84 ± 0.08 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         28.75 ± 0.04 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        324.61 ± 1.42 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2381.96 ± 324.07 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         28.86 ± 0.08 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         28.77 ± 0.03 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        325.11 ± 0.50 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2367.22 ± 327.08 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         28.88 ± 0.10 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         28.77 ± 0.03 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        325.49 ± 0.74 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2354.55 ± 308.02 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         28.88 ± 0.06 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         28.78 ± 0.05 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        324.81 ± 1.31 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2341.32 ± 315.81 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         28.87 ± 0.07 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         28.76 ± 0.04 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        323.96 ± 1.23 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2342.35 ± 315.55 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         28.86 ± 0.06 |
| qwen35 9B Q6_K                 |   7.15 GiB |     9.20 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         28.77 ± 0.03 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |     1668.85 ± 256.59 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2605.93 ± 453.39 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         76.27 ± 2.82 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         91.17 ± 7.30 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |     1690.60 ± 288.08 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2596.14 ± 417.28 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         76.65 ± 2.60 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         91.02 ± 9.03 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |     1663.63 ± 273.81 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2595.75 ± 411.02 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         98.65 ± 6.53 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         92.86 ± 4.57 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |     1765.29 ± 316.36 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2582.44 ± 402.51 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         99.15 ± 6.16 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         91.24 ± 5.13 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |     1381.98 ± 267.76 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2607.62 ± 425.57 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         76.81 ± 2.80 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         92.85 ± 4.19 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |     1697.08 ± 287.06 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2621.52 ± 413.42 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         76.74 ± 2.68 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |        90.50 ± 10.12 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |     1680.98 ± 295.59 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2615.90 ± 429.52 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         98.95 ± 6.40 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         91.33 ± 6.52 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |     1682.87 ± 274.93 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2587.89 ± 384.61 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         98.25 ± 7.01 |
| gemma4 26B.A4B Q3_K - Medium   |  11.84 GiB |    25.23 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         92.35 ± 3.65 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |       737.39 ± 15.29 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |        770.56 ± 1.96 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         19.65 ± 0.20 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         22.08 ± 0.13 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |       737.33 ± 14.40 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |        769.80 ± 2.17 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         19.62 ± 0.21 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         22.08 ± 0.10 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |       738.98 ± 15.51 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |        775.87 ± 2.44 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         19.62 ± 0.19 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         22.08 ± 0.12 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |       737.07 ± 14.97 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |        774.18 ± 3.15 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         19.63 ± 0.21 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         22.04 ± 0.13 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       735.62 ± 15.97 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |        770.34 ± 1.83 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         19.63 ± 0.20 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         22.04 ± 0.15 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       727.18 ± 12.62 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |        759.24 ± 2.29 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         19.61 ± 0.20 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         21.97 ± 0.13 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        724.99 ± 9.94 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |        759.55 ± 4.14 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         19.59 ± 0.23 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         21.96 ± 0.17 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |       719.54 ± 15.96 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |        756.02 ± 3.63 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         19.60 ± 0.20 |
| gemma4 31B IQ3_XXS - 3.0625 bpw |  11.01 GiB |    30.70 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         21.90 ± 0.14 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        239.06 ± 1.31 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2053.48 ± 211.79 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |        114.77 ± 9.14 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         86.62 ± 2.24 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        238.04 ± 1.27 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2044.37 ± 229.86 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |        114.49 ± 9.75 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         86.68 ± 2.03 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        238.78 ± 0.94 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2059.63 ± 229.58 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |       115.00 ± 10.04 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         86.68 ± 2.48 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        239.40 ± 1.42 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2065.48 ± 221.09 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |        114.61 ± 9.36 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         86.64 ± 2.43 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        239.37 ± 2.05 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2046.33 ± 220.67 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |        114.52 ± 9.46 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         86.66 ± 2.42 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        239.04 ± 1.32 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2049.00 ± 215.67 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |        114.80 ± 9.31 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         86.82 ± 2.23 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        239.33 ± 0.51 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2052.98 ± 211.04 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |        114.89 ± 9.40 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         86.54 ± 2.69 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        239.31 ± 0.33 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2048.65 ± 216.86 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |        114.70 ± 9.34 |
| deepseek2 30B.A3B Q2_K - Medium |  10.63 GiB |    29.94 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         86.80 ± 2.40 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        252.33 ± 1.99 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2070.36 ± 226.21 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |        115.93 ± 9.74 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         88.21 ± 2.39 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        252.94 ± 1.18 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2065.12 ± 222.50 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |        116.13 ± 9.42 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         88.10 ± 2.23 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        253.12 ± 0.59 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2066.95 ± 223.37 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |        116.16 ± 9.37 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         88.04 ± 2.44 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        253.13 ± 1.37 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2061.54 ± 232.95 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |        116.69 ± 9.26 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         88.34 ± 2.46 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        252.75 ± 1.16 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2070.47 ± 223.97 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |        116.32 ± 9.69 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         88.06 ± 2.48 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        254.57 ± 0.81 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2062.14 ± 221.24 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |        116.18 ± 9.65 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         88.12 ± 2.24 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        252.73 ± 1.57 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2061.73 ± 219.45 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |        116.08 ± 9.96 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         88.32 ± 2.20 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        252.49 ± 1.27 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2059.39 ± 219.75 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |        116.25 ± 9.68 |
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         88.16 ± 2.31 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        373.41 ± 1.62 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2813.06 ± 514.16 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |       164.51 ± 14.06 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |        138.08 ± 3.93 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        372.74 ± 1.53 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2848.89 ± 484.74 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |       165.54 ± 13.48 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |        137.11 ± 4.40 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        373.44 ± 1.53 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2903.01 ± 613.98 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |       164.89 ± 13.00 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |        137.08 ± 3.81 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        372.96 ± 2.14 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2715.28 ± 435.24 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |       164.01 ± 13.89 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |        136.86 ± 4.24 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        371.08 ± 5.61 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2917.21 ± 532.22 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |       165.30 ± 12.65 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |        137.67 ± 4.31 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        374.48 ± 1.73 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2974.23 ± 585.48 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |       164.08 ± 13.42 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |        137.32 ± 3.76 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        375.76 ± 2.49 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2675.45 ± 322.27 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |       164.12 ± 13.49 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |        137.59 ± 3.79 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        374.85 ± 1.05 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     3003.44 ± 508.47 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |       163.28 ± 12.49 |
| gpt-oss 20B Q4_K - Medium      |  10.81 GiB |    20.91 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |        137.51 ± 5.39 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        288.66 ± 0.70 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2527.69 ± 405.58 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         30.32 ± 0.15 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         30.44 ± 0.07 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        288.46 ± 1.32 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2488.32 ± 394.54 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         30.34 ± 0.15 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         30.48 ± 0.09 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        288.52 ± 0.63 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2510.21 ± 390.11 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         30.34 ± 0.17 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         30.43 ± 0.08 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        288.70 ± 0.52 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2498.84 ± 380.28 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         30.36 ± 0.16 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         30.43 ± 0.07 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       282.22 ± 15.58 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2483.00 ± 374.69 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         30.31 ± 0.12 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         30.52 ± 0.09 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        288.83 ± 0.84 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2494.72 ± 387.18 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         30.35 ± 0.15 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         30.46 ± 0.10 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        288.23 ± 0.81 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2482.18 ± 376.43 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         30.35 ± 0.17 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         30.43 ± 0.06 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        288.19 ± 0.92 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2509.24 ± 373.76 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         30.33 ± 0.16 |
| qwen35moe 35B.A3B IQ2_M - 2.7 bpw |  10.72 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         30.44 ± 0.07 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        253.60 ± 2.53 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2144.80 ± 283.94 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         29.40 ± 0.08 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         23.04 ± 0.35 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        254.56 ± 2.37 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2140.47 ± 276.38 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         29.40 ± 0.16 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         23.77 ± 0.42 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        252.88 ± 2.11 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2123.33 ± 268.79 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         29.37 ± 0.14 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         23.27 ± 0.60 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        253.81 ± 1.81 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2128.22 ± 294.20 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         29.37 ± 0.10 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         23.41 ± 0.28 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        248.60 ± 4.31 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |      1158.55 ± 84.64 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         26.74 ± 4.88 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         21.76 ± 2.75 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       211.33 ± 61.53 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |      1112.21 ± 85.27 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         26.53 ± 6.34 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         21.21 ± 3.44 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |       219.75 ± 32.91 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |      1178.76 ± 28.32 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         26.33 ± 5.69 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         21.23 ± 3.10 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |       239.54 ± 20.86 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     1137.45 ± 113.68 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         26.18 ± 5.66 |
| qwen35moe 35B.A3B Q3_K - Medium |  15.45 GiB |    34.66 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         21.57 ± 3.28 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |       1074.08 ± 2.20 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |        123.99 ± 0.20 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         36.62 ± 0.78 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |          3.63 ± 0.00 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |       581.21 ± 20.55 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |        181.89 ± 0.25 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |          8.35 ± 0.04 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |          8.28 ± 0.02 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |       570.67 ± 21.86 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |        182.40 ± 0.34 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |          3.66 ± 0.00 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |          3.64 ± 0.00 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |       570.28 ± 18.18 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |        182.45 ± 0.31 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |          8.33 ± 0.03 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |          8.31 ± 0.01 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |      312.81 ± 114.05 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |        184.79 ± 0.65 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |          3.67 ± 0.00 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |          6.31 ± 0.01 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        295.99 ± 0.34 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |        182.79 ± 0.35 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |          8.21 ± 0.04 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         12.03 ± 0.04 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        362.02 ± 0.87 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |        151.25 ± 0.77 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         36.18 ± 0.78 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |          6.31 ± 0.00 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        294.80 ± 1.37 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |        182.40 ± 0.35 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |          8.19 ± 0.01 |
| llama ?B IQ4_XS - 4.25 bpw     |  11.11 GiB |    22.25 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         12.09 ± 0.07 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |       857.46 ± 53.36 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |        936.70 ± 2.95 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         37.06 ± 1.67 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         36.76 ± 1.00 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |       856.49 ± 49.12 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |        937.86 ± 2.62 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         37.00 ± 2.14 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         36.78 ± 0.89 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |       856.83 ± 49.85 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |        937.17 ± 2.51 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         36.90 ± 2.12 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         37.11 ± 0.87 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |       857.93 ± 50.95 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |        937.40 ± 2.42 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         36.89 ± 1.81 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         36.94 ± 0.81 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       856.76 ± 52.70 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |        936.95 ± 2.19 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         36.82 ± 1.72 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         36.64 ± 0.91 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       849.79 ± 43.93 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |        928.50 ± 2.44 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         36.66 ± 1.71 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         36.50 ± 1.23 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |       846.31 ± 43.39 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |        926.06 ± 2.23 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         36.63 ± 1.91 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         36.55 ± 1.01 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |       844.93 ± 43.40 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |        923.21 ± 2.55 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         36.84 ± 1.82 |
| mistral3 14B Q3_K - Medium     |  10.68 GiB |    23.57 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         36.42 ± 1.13 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        260.05 ± 0.43 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |      1732.82 ± 94.54 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         50.87 ± 0.46 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         50.85 ± 0.32 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        260.68 ± 0.16 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |      1737.00 ± 91.02 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         50.70 ± 0.52 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         50.78 ± 0.26 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        260.36 ± 0.29 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |      1743.49 ± 91.92 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         50.55 ± 0.43 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         50.74 ± 0.16 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        260.97 ± 0.26 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |      1740.87 ± 93.08 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         50.59 ± 0.37 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         50.74 ± 0.30 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       254.65 ± 12.32 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |      1733.49 ± 94.95 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         50.61 ± 0.49 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         50.77 ± 0.26 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        260.14 ± 0.28 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |      1718.25 ± 87.73 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         50.62 ± 0.52 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         50.73 ± 0.30 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        260.22 ± 0.30 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |      1720.22 ± 82.95 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         50.44 ± 0.39 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         50.62 ± 0.18 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        260.98 ± 0.11 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |      1715.84 ± 82.38 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         50.51 ± 0.52 |
| qwen2 14B Q4_K - Medium        |   8.37 GiB |    14.77 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         50.68 ± 0.28 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        490.60 ± 1.84 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     3112.93 ± 536.50 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         91.87 ± 2.56 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         93.43 ± 1.39 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        490.25 ± 2.26 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     3153.60 ± 574.50 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         93.64 ± 2.85 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         93.80 ± 1.38 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        490.19 ± 1.39 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     3123.64 ± 555.21 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         93.64 ± 2.36 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         93.80 ± 0.98 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        490.66 ± 1.42 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     3090.97 ± 510.68 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         94.46 ± 1.91 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         93.55 ± 1.16 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |       453.92 ± 63.12 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     3124.26 ± 529.91 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         93.21 ± 1.70 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         93.77 ± 1.65 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        490.00 ± 1.65 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     3090.31 ± 500.49 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         94.13 ± 1.84 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         94.03 ± 1.42 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        490.01 ± 2.04 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     3135.87 ± 588.59 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         92.54 ± 3.28 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         94.20 ± 1.42 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        489.83 ± 1.78 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     3066.91 ± 533.98 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         94.19 ± 2.26 |
| qwen2 7B Q4_K - Medium         |   4.36 GiB |     7.62 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         93.74 ± 0.95 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        354.03 ± 0.76 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2598.00 ± 409.23 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         31.64 ± 0.09 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         31.47 ± 0.07 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        354.44 ± 1.08 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2612.05 ± 419.85 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         31.60 ± 0.13 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         31.55 ± 0.07 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        353.22 ± 0.97 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2604.63 ± 409.38 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         31.63 ± 0.13 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         31.50 ± 0.07 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        354.21 ± 0.85 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2618.05 ± 418.59 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         31.56 ± 0.14 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         31.51 ± 0.08 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        354.88 ± 0.56 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2610.85 ± 415.49 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         31.52 ± 0.12 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         31.58 ± 0.11 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        354.69 ± 0.61 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2600.70 ± 400.53 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         31.59 ± 0.10 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         31.48 ± 0.09 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        354.50 ± 0.91 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2588.64 ± 394.90 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         31.61 ± 0.08 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         31.52 ± 0.14 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        354.10 ± 0.59 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2594.59 ± 399.42 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         31.60 ± 0.14 |
| qwen35 9B Q4_K - Medium        |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         31.47 ± 0.09 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        352.07 ± 1.57 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2600.05 ± 412.75 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         31.64 ± 0.07 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         31.54 ± 0.11 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp256 |        354.35 ± 0.58 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           pp512 |     2605.97 ± 412.31 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg128 |         31.60 ± 0.12 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    0 |       65536 |           tg256 |         31.55 ± 0.04 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        353.81 ± 1.45 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2609.55 ± 416.85 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         31.66 ± 0.09 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         31.54 ± 0.05 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp256 |        354.21 ± 1.22 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           pp512 |     2599.15 ± 402.89 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg128 |         31.62 ± 0.14 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    0 |       65536 |           tg256 |         31.51 ± 0.05 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        352.25 ± 0.53 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2597.64 ± 408.60 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         31.58 ± 0.10 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         31.51 ± 0.06 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp256 |        354.25 ± 0.47 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           pp512 |     2595.19 ± 405.95 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg128 |         31.63 ± 0.18 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q8_0 |   1 |    1 |       65536 |           tg256 |         31.46 ± 0.11 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        354.44 ± 0.67 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2587.35 ± 399.83 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         31.56 ± 0.14 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       1 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         31.54 ± 0.08 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp256 |        354.49 ± 0.61 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           pp512 |     2580.18 ± 388.23 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg128 |         31.57 ± 0.10 |
| qwen35 9B Q4_K - Flash-Medium  |   5.23 GiB |     8.95 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         31.51 ± 0.13 |

build: 65ab1f7 (9437)