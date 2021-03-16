# Xdebug из docker контейнера

2021-03-16. PHP 8.0.3. Xdebug 3.0.3.

## Установка

1. В файл `/etc/hosts` прописать домен `exd.local`.
Домен указан в файле проекта `docker-files/dev/nginx/local.conf` в параметре `server_name`.

2. Скопировать файл `.env.local.distrib` в `env.local`. Заполнить настройки.

3. Настроить PHP Storm. Значения взять в `env.local`. Имя сервера и порт должны совпадать.
