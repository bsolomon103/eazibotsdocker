FROM nginx:latest

RUN mkdir -p /etc/nginx/ssl

COPY ./ssl_certificates/bundle.cer /etc/nginx/ssl/bundle.cer
COPY ./ssl_certificates/_.eazibots.com_private_key.key /etc/nginx/ssl/private_key.key
COPY ./ssl_certificates/_.eazibots.com_ssl_certificate_INTERMEDIATE.cer /etc/nginx/ssl/intermediate.cer


COPY ./default.conf /etc/nginx/conf.d/default.conf
