# Technical Architecture — ASYNCUA

**Upstream:** [https://github.com/opcua-asyncio/asyncua](https://github.com/opcua-asyncio/asyncua)
**License:** MIT
**Category:** FACTORY_MANUFACTURING
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

OPC-UA industrial protocol client/server

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local predictive maintenance on edge PLC hardware
2. AIOSS tamper-evident production log for every part and batch
3. AES-256 encryption for proprietary process parameters
4. Single-binary MES executable for locked-down factory floor PCs
5. Zero-cloud: all analytics and inference run on local industrial servers
6. GPU/CPU equalizer: vision inspection on GPU, telemetry on CPU
7. Offline OEE calculation replacing cloud analytics dashboards
8. Open OPC-UA/Modbus integration replacing proprietary SCADA middleware

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_asyncua.spec` or `go build -o asyncua`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |