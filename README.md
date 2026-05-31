# LlamaCppBench
Benchmarks of various open models (Qwen, Gemma, GLM, GPT-OSS) on home PC with 16GB dGPU.

Tought I could have it saved somewhere and maybe it's worth of sharing...

## PC:
* i3-9100F
* 16GB DDR4
* XFX RX 9070
* Archlinux - Kernel 7.0.10-arch1-1
* vulkan-radeon 1:26.1.1-1
* llama.cpp-vulkan b9437-1

## bench.sh
``` bash
llama-bench \
    -m models/Qwen3-14B-Q4_K_M.gguf \
    -m models/Qwen3.5-9B-Q6_K_MTP.gguf \
    -m models/gemma-4-26B-A4B/gemma-4-26B-A4B-it-UD-Q3_K_M.gguf \
    -m models/gemma-4-31B/gemma-4-31B-it-UD-IQ3_XXS.gguf \
    -m models/GLM-4.7-Flash/GLM-4.7-Flash-Q2_K_L.gguf \
    -m models/GLM-4.7-Flash/GLM-4.7-Flash-REAP-23B-A3B-Q3_K_M.gguf \
    -m models/gpt-oss-20b-Q4_K_M.gguf \
    -m models/Qwen3.6-35B-A3B/Qwen3.6-35B-A3B-UD-IQ2_M.gguf \
    -m models/Qwen3.6-35B-A3B/Qwen3.6-35B-A3B-UD-Q3_K_M.gguf \
    -ngl 99 -fa on \
    -mmp 0,1 -t 1,4 -ctk q8_0 -ctv q8_0,q4_1 -fitc 65536 \
    -p 256,512 -n 128,256
```

## Result table

[📊 View interactive table](https://THX81.github.io/LlamaCppBench/)

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
| deepseek2 30B.A3B Q3_K - Medium |  10.49 GiB |    23.00 B | Vulkan     |  99 |       4 |   q8_0 |   q4_1 |   1 |    1 |       65536 |           tg256 |         88.16 ± 2.31 |⏎
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
