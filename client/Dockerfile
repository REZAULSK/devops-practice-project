FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
RUN npm install @rollup/rollup-linux-x64-musl
COPY . .
EXPOSE 3000
CMD ["npm", "run", "dev", "--", "--host"]