FROM node:18-alpine

WORKDIR /app/frontend

RUN npm install -g pnpm

COPY package.json pnpm-lock.yaml ./
RUN pnpm install

COPY . .

CMD ["pnpm", "run", "dev"]
