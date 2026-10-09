# Ethics — ASYNCUA

**Project:** ASYNCUA  
**Category:** FACTORY_MANUFACTURING  
**Upstream:** see BENCH.json  
**Pinned commit:** `f77b01228dd5dc9bf9ed53887abc779f837f609a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d5d191a62c767e7c7be30ef377ddf8249c5b5ff9139691bfb6b39f600bd90b93`  
**Date:** October 2026

## Position

ASYNCUA is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
