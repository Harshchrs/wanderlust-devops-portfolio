# Stage 1
FROM node:22 AS backend-builder

WORKDIR /app

COPY . .

RUN npm i

# Stage 2
FROM node:22-slim

WORKDIR /app

# Copy the above stage as compressed
COPY --from=backend-builder /app .
 
COPY .env.sample .env

EXPOSE 5000

CMD ["npm", "start"] 
