# Linkwarden

## Setup

Copy `.env.example` to `.env` and fill in the values. The required environment variables are:

```
NEXTAUTH_SECRET=VERY_SENSITIVE_SECRET
MEILI_MASTER_KEY=VERY_SENSITIVE_MEILI_MASTER_KEY
POSTGRES_PASSWORD=CUSTOM_POSTGRES_PASSWORD
```

The only thing you MUST change here is `NEXTAUTH_SECRET`, `POSTGRES_PASSWORD`, and `MEILI_MASTER_KEY`, they all should be different secret phrases. The phrase should be wrapped in single or double quotes if any special characters are used.

## Deploy

**Production**
```
docker compose up -d
```

**Development**
```
docker compose -f docker-compose.yml -f docker-compose.dev.yml up -d
```
