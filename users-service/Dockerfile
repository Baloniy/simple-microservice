FROM node:10

# Создать директорию app
WORKDIR /usr/src/users-service

# Используется символ подстановки для копирования как package.json, так и package-lock.json
COPY package*.json ./

RUN npm install

# Скопировать исходники приложения
COPY . .

# Port
EXPOSE 8081

# Запуск проекта
CMD ["node", "server.js"]