FROM nginx

COPY nginx.conf /etc/nginx/template.conf

RUN envsubst < /etc/nginx/template.conf > /etc/nginx/nginx.conf
