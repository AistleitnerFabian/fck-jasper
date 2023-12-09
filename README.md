# PDF Gen using Nuxt3 and Gotenberg

## Setup for Docker

```bash
docker compose up -d
```

```bash
POST http://localhost:3200/forms/chromium/convert/url 
--form 'url="http://host.docker.internal:3100/installation-report"'
```

## Development Server (Nuxt)

```bash
npm run dev
```

Start the development page on `http://localhost:3000?dev=true`:
