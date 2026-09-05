# NVIDIA NIM free-tier — IDs live (round5)

Smoke 2026-09-05 (BRT). Host: `integrate.api.nvidia.com/v1`. Sem secrets. Independente — sem endosso NVIDIA.

**Landing + PIX (EMV):** https://ziuluiziul.github.io/ane-pagamento/nim/ — R$50=`qr_2` · R$100=`qr_3`

**Hub Alpha:** https://ziuluiziul.github.io/round1-cumulunimbus/

## GET `/v1/models`
HTTP 200 · 32 IDs `nvidia/*` nesta conta.

## Chat/completions (HTTP)
| ID | HTTP |
| --- | --- |
| `nvidia/nemotron-3-super-120b-a12b` | 200 (×3) |
| `nvidia/ising-calibration-1.5-31b` | 200 |
| `nvidia/llama-3.1-nemoguard-8b-content-safety` | 200 |
| `nvidia/llama-3.1-nemotron-safety-guard-8b-v3` | 200 |
| `nvidia/llama-3.1-nemotron-51b-instruct` | 404 |
| `nvidia/llama-3.1-nemotron-70b-instruct` | 404 |
| `nvidia/llama-3.3-nemotron-super-49b-v1.5` | skip (410 histórico) |

near-limit: não declarado / 0 observado · exhausted: 0

## Mesh
- [Groq 429](https://ziuluiziul.github.io/groq-round1-offer/FIVE-429-ERRORS.md)
- [OpenRouter 402/429](https://ziuluiziul.github.io/openrouter-free-oferta/FREE-402-429.md)
