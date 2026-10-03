# PAX Benchmark Suite — 27B on Commodity Hardware, With Receipts

**Lois-Kleinner Alpasan, 23 · Anticloud FZ LLE · 0-1.gg**

Every number below is measured, with corrections published alongside wins. No cherry-picking: the lows ship in the same tables.

## Headliners (from `PAX_RESULTS.md`, H100 + 2x3090 + T4 runs)
| Benchmark | Score | Standing |
|---|---|---|
| GSM8K (SymPy-PoT + self-consistency) | **100%** | SOTA-class (saturated) |
| MuSR (0-shot) | **41.33%** | above leaderboard max (38.7%) |
| ARC-1 eval | **51.75%** | at open non-LLM SOTA (321 detectors, zero LLM) |
| ARC-2 train | **33.90%** | above best pure-symbolic (16.1%) |
| ft09 (ARC-3) | **6/6 FULL WIN** | 10x human efficiency on L1 |
| MMLU | **84.28%** | near-SOTA for 27B class |
| Millennium-20 (T4) | 20/20 @ 4.1–4.2 tok/s | zero failures, hashed |

## Honest lows (same doc, same tables)
BBH 17.78% · TruthfulQA MC1 32% · ARC-2 eval 1.67% · GAIA 40% — first-iteration gaps of a 27B without frontier APIs.

## Economics (measured, corrected)
- $0.43/1M output tokens self-hosted (240.7 tok/s sustained); T4 research run $0.013 electricity
- 610W measured rig draw; $1.01–1.52 full marathon — v9 estimate corrected in-doc

## Files
- `PAX_RESULTS.md` — full tables v1–v11 with corrections (RHAE formula, mmlu_pro, energy)
- `summary.csv` / `hash_manifest.json` / `RANKING.md` — Kaggle v52/v54 runs
- `BENCHMARK_RESULTS.csv` — 26-framework compliance suite (MITRE 100/100, NIST 88%, TRL 7/9)

Apache-2.0 + Enterprise commercial dual (Anticommons 0.1.0). Issues/discussions disabled — read-only mirror; contact lois@0-1.gg.
