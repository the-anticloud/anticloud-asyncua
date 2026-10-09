# Educators — ASYNCUA

**Project:** ASYNCUA  
**Category:** FACTORY_MANUFACTURING  
**Upstream:** see BENCH.json  
**Pinned commit:** `f77b01228dd5dc9bf9ed53887abc779f837f609a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d5d191a62c767e7c7be30ef377ddf8249c5b5ff9139691bfb6b39f600bd90b93`  
**Date:** October 2026

## Teaching with ASYNCUA

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `d5d191a62c767e7c7be30ef377ddf8249c5b5ff9139691bfb6b39f600bd90b93` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
