FROM node:14.21.3-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
COPY index.js /app/
EXPOSE 3003
RUN npm run build
CMD [ "node", "dist/index.js" ]



