# Estúdio Lunae em construção

## Run Locally

**Prerequisites:** Node.js

1. Install dependencies:

```bash
npm install
```

2. Run the app:

```bash
npm run dev
```

## Deploy

Production deploy runs automatically from GitHub Actions on every push to `main`.
The workflow builds the Vite app and uploads only `dist/` to Hostinger via SSH.

Required repository secrets:

- `HOSTINGER_SSH_HOST`: SSH host from Hostinger
- `HOSTINGER_SSH_PORT`: SSH port from Hostinger
- `HOSTINGER_SSH_USER`: SSH username from Hostinger
- `HOSTINGER_SSH_PRIVATE_KEY`: private key allowed in Hostinger SSH access
- `HOSTINGER_TARGET_DIR`: absolute path to `public_html`
