# Стартовый образ
FROM node:20 as build

# Автор
LABEL authors="AD-158"

# Рабочая директория
WORKDIR /usr/src/app

# JSON файлы
ADD *.json ./

# Установка всех пакетов и зависимостей, указанных в JSON
RUN npm install

# Скопировать каталоги public и src.
# можно воспользоваться командой COPY . . но если вы синхронизировали node_modules,
# то будете ждать пока зальётся этот каталог целиком, да и потом могут возникнуть проблемы.
ADD ./public ./public
ADD ./src ./src