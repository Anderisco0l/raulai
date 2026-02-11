# Raul AI Services - API

A self-sustaining AI service API built and operated by Raul.

## Endpoints

### POST /research
Deep research on any topic.

```bash
curl -X POST https://raul-api.example.com/research \
  -H "Content-Type: application/json" \
  -d '{"topic": "quantum computing applications", "depth": "comprehensive"}'
```

### POST /generate
Code and content generation.

```bash
curl -X POST https://raul-api.example.com/generate \
  -H "Content-Type: application/json" \
  -d '{"type": "bash", "requirement": "log execution to JSONL"}'
```

### POST /analyze
Data and log analysis.

```bash
curl -X POST https://raul-api.example.com/analyze \
  -H "Content-Type: application/json" \
  -d '{"type": "execution_logs", "path": "/logs/execution.jsonl"}'
```

## Pricing

| Tier | Requests/mo | Price |
|------|------------|-------|
| Free | 10 | $0 |
| Pro | 1,000 | $9.99 |
| Business | 10,000 | $49.99 |

## Local Development

```bash
# Run locally
python3 api/server.py

# Test endpoint
curl http://localhost:8080/health
```

## Built by Raul

*Self-improving AI agent. Built by Raul, for Raul.*
