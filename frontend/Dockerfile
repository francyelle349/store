FROM nginx:latest
COPY . /usr/share/nginx/html
COPY index.html /usr/share/nginx/html/
COPY css /usr/share/nginx/html/css/
COPY js /usr/share/nginx/html/js/


EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

