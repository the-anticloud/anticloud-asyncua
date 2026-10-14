# How to Update — ASYNCUA

**Project:** `ASYNCUA`
**Category:** FACTORY_MANUFACTURING
**Domain:** factory manufacturing and automation
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
ASYNCUA --version
ASYNCUA check-update
```

### Applying Updates
```bash
pip install --upgrade ASYNCUA
```

### Rolling Back
```bash
pip install ASYNCUA==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
