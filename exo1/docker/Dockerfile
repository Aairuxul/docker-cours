FROM node:22-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

RUN npm run build && npm cache clean --force

EXPOSE 4321
CMD ["npm", "run","preview"]