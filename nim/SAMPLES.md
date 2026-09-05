# NIM Super120 samples (round8)

Timestamp UTC: 2026-09-05T23:16:26Z · BRT: 2026-09-05 ~20:16
GET /v1/models HTTP 200 · nvidia ids listed in models_ids.txt
ID live: `nvidia/nemotron-3-super-120b-a12b` · smoke_ok=6 · near_limit=False · free-tier only

Host oficial: `https://integrate.api.nvidia.com/v1`
Docs limites: https://docs.api.nvidia.com/nim/docs/api-quickstart (nao inventar RPM; observar UI).
Sem secrets neste arquivo.

## Sample 1 (HTTP 200)

**Prompt:** Em 3 bullets curtos em pt-BR: o que um smoke GET /v1/models deve provar.

- Endpoint responde HTTP 200 com JSON valido
- Corpo traz lista de modelos (nao vazia) com ids
- Sem falha critica de auth/roteamento no catalog

usage={'prompt_tokens': 61, 'completion_tokens': 120, 'total_tokens': 181} · finish=length

## Sample 2 (HTTP 200)

**Prompt:** Escreve um template curl minimo de chat/completions no modelo nvidia/nemotron-3-super-120b-a12b usando $NVIDIA_API_KEY (nao inventes a chave).

```bash
curl -sS https://integrate.api.nvidia.com/v1/chat/completions \
  -H "Authorization: Bearer $NVIDIA_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "nvidia/nemotron-3-super-120b-a12b",
    "messages": [{"role":"user","content":"ping smoke"}],
    "max_tokens": 64
  }'
```
(chave so via env; nunca colar secret)

usage={'prompt_tokens': 85, 'completion_tokens': 120, 'total_tokens': 205} · finish=length

## Sample 3 (HTTP 200)

**Prompt:** Em 1 paragrafo curto pt-BR: diferenca entre prototipagem NIM hosted (API catalog free) e NVIDIA AI Enterprise.

A prototipagem NIM hosted (API catalog free) permite testar modelos pré‑treinados via chamadas de API gratuitas, ideal para validação rápida sem infraestrutura própria, enquanto o NVIDIA AI Enterprise oferece uma plataforma completa, licenciada e otimizada para produção, com suporte empresarial, gerenciamento de clusters,

usage={'prompt_tokens': 71, 'completion_tokens': 120, 'total_tokens': 191} · finish=length

## Sample 4 (HTTP 200)

**Prompt:** Lista 4 falhas comuns ao chamar integrate.api.nvidia.com/v1 (pt-BR, bullets).

- Erro de autenticação (token ausente ou inválido)  
- Parâmetros de requisição malformados ou ausentes (ex.: payload JSON incorreto)  
- Limite de taxa excedido (HTTP 429 Too Many Requests)  
- Falha de conectividade ou timeout ao alcançar

usage={'prompt_tokens': 60, 'completion_tokens': 120, 'total_tokens': 180} · finish=length

## Sample 5 (HTTP 200)

**Prompt:** Resumo em 4 linhas pt-BR: o que entregar num relatorio de smoke NIM sem secrets.

- Descrição do objetivo e escopo do teste de smoke no NIM.  
- Lista de componentes/serviços testados e critérios de aprovação.  
- Resultados obtidos (pass/fail) com evidências de logs ou métricas relevantes.  
- Recomendações de ações

usage={'prompt_tokens': 60, 'completion_tokens': 120, 'total_tokens': 180} · finish=length

## Sample 6 (HTTP 200)

**Prompt:** Em 1 frase pt-BR: quando HTTP 503 no mesmo SKU NIM, o que fazer primeiro.

Verificar status/disponibilidade do SKU e aguardar breve backoff antes de retentar o mesmo endpoint.

usage={'prompt_tokens': 63, 'completion_tokens': 120, 'total_tokens': 183} · finish=length

## PIX (verdade pix-clean)
- R$50 = qr_2 / pix_copia_cola_2 · EMV tag54=50.00
- R$100 = qr_3 / pix_copia_cola_3 · EMV tag54=100.00

Landing: https://ziuluiziul.github.io/ane-pagamento/nim/
Playbook PDF: https://ziuluiziul.github.io/ane-pagamento/nim/NIM-free-Super120-playbook.pdf
Hub: https://ziuluiziul.github.io/round1-cumulunimbus/
