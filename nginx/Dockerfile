# Стартовый образ
FROM nginx:1.25

# Автор
LABEL authors="AD-158"

# Удалить дефолтный конфиг
RUN rm /etc/nginx/conf.d/default.conf

# Заменить кастомным
COPY nginx.conf /etc/nginx/conf.d/