# week07/frontend/Dockerfile

FROM nginx:alpine

LABEL author="sit722"

COPY nginx.conf /etc/nginx/conf.d/default.conf

COPY . /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
