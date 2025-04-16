FROM node:22-slim

LABEL description="Node.js 22 with npm and pnpm"

WORKDIR /app

RUN apt-get update && apt-get install -y --no-install-recommends \
    curl \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN npm install -g pnpm

RUN node --version && npm --version && pnpm --version

CMD ["/bin/bash"]
