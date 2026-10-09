# Students — ASYNCUA

**Project:** ASYNCUA  
**Category:** FACTORY_MANUFACTURING  
**Upstream:** see BENCH.json  
**Pinned commit:** `f77b01228dd5dc9bf9ed53887abc779f837f609a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d5d191a62c767e7c7be30ef377ddf8249c5b5ff9139691bfb6b39f600bd90b93`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `f77b01228dd5dc9bf9ed53887abc779f837f609a`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `d5d191a62c767e7c7be30ef377ddf8249c5b5ff9139691bfb6b39f600bd90b93`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
