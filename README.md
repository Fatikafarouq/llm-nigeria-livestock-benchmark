[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Fatikafarouq/llm-nigeria-livestock-benchmark/blob/main/nigeria_livestock_llm_benchmark.ipynb)

# LLM Nigeria Livestock Benchmark

Benchmarking LLM performance on Nigerian indigenous livestock management knowledge to surface geographic bias in large language models.

## What this is
A 420-question evaluation benchmark testing LLM knowledge gaps on Nigerian livestock management, ethnoveterinary practice, and tropical animal disease. Uses an LLM-as-judge scoring pipeline (0–2 scale) via the Groq API.

## Models evaluated
- Llama 3.1 8B (judge + evaluated model) — pilot complete
- Gemma2 9B — pilot complete
- Claude Sonnet, GPT-4o, Gemini 2.5 Pro, Llama 3.1 70B — Phase 2 (in progress)

## Question categories
- Breed Knowledge
- Ethnoveterinary Practice
- Tropical Disease Knowledge
- Local Treatment Context
- Terminology

## Why it matters
Most LLM benchmarks are Western-centric. This project investigates performance gaps for Global South agricultural contexts, with a focus on Nigerian indigenous livestock systems.

## How to run
1. Click the Open in Colab badge above
2. Paste your Groq API key when prompted (free tier works)
3. Upload your questions CSV with columns: `Question`, `Answer`, `Category`
4. The pipeline runs a 10-question pilot per model before full evaluation
5. Results export automatically as CSV

## Requirements
See `requirements.txt`
