FROM node:22 AS frontend-builder

WORKDIR /app

COPY package*.json ./

RUN npm ci --ignore-scripts

COPY . .

FROM node:22-slim

WORKDIR /app

COPY --from=frontend-builder /app .

COPY .env.sample .env.local

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host"]

