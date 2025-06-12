#frontend
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --omit=dev --legacy-peer-deps
COPY . .
EXPOSE 5173
CMD ["npm", "run", "dev"]

