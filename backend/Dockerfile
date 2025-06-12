FROM node:18-alpine
WORKDIR /app
COPY package.json ./
RUN npm install --legacy-peer-deps
#RUN npm install -g nodemon
COPY . .
ENV PORT=3001
EXPOSE 3001
RUN adduser --disabled-password --gecos '' appuser
USER  appuser
CMD ["npm", "run", "dev"]


