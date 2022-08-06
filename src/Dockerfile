FROM node:16.15.0
WORKDIR /app
RUN apt update && \
    apt-get install npm --yes
COPY ./package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]