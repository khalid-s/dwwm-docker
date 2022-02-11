FROM nginx:alpine

LABEL author="Khalid Sookia"

COPY ./dwwm.conf /etc/nginx/conf.d/default.conf

EXPOSE 80

ENTRYPOINT ["nginx", "-g", "daemon off;"]