FROM node:20-slim

RUN npm i -g pnpm

WORKDIR /app

COPY . .

RUN pnpm install

RUN pnpm build

ENTRYPOINT ["node", "/app/dist/index.js"]