# Llama.cpp Bench Results
Benchmarks of various open models (Qwen, Gemma, GLM, GPT-OSS, ...WIP) on home PC with 16GB dGPU.

Thought I could have it saved somewhere and maybe it's worth of sharing...

# TL;DR
GLM 4.7 Flash in llama-ui and claude code + mcp usage = balance of quality and tps.

Qwen +quality, -tps

GPT +tps, -quality

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
    -m models/Codestral-22B-v0.1-IQ4_XS.gguf \
    -m models/Devstral-Small-2-24B-Instruct-2512-Q3_K_M.gguf \
    -m models/Qwen2.5/qwen2.5-coder-14b-instruct-q4_k_m.gguf \
    -m models/Qwen2.5/qwen2.5-coder-7b-instruct-q4_k_m.gguf \
    -m models/Qwen3.5/Qwen3.5-9B-DeepSeek-V4-Flash-Q4_K_M.gguf \
    -m models/Qwen3.5/Qwen3.5-9B.Q4_K_M.gguf \
    -ngl 99 -fa on \
    -mmp 0,1 -t 1,4 -ctk q8_0 -ctv q8_0,q4_1 -fitc 65536 \
    -p 256,512 -n 128,256
```

## Result table

[📊 View interactive table](https://THX81.github.io/LlamaCppBenchResults/)
