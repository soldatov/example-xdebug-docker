FROM nginx:1.19
ADD ./local.conf /etc/nginx/conf.d/default.conf
COPY ./docker-entrypoint.sh /docker-entrypoint.d/100-docker-entrypoint.sh
WORKDIR /app