# GPT-5.6 Terra API (gpt-5.6-terra / gpt5.6terra) — llm guide with published pricing

> **input $1.6; cached_input $0.16; cache_write $2** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-9d99d0)** · **[Get an API key](https://go.apimart.ai/k-d6e05e)**

Everything here refers to **gpt-5.6-terra** — also written **gpt5.6terra** or **gpt 5.6 terra**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $1.6 |
| `cached_input` | $0.16 |
| `cache_write` | $2 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $160 |
| 1,000 | $1,600 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"gpt-5.6-terra","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
