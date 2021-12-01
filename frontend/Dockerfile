FROM ubuntu
RUN apt-get update
RUN apt-get install -y nginx
COPY fundoo.conf /etc/nginx/sites-available/fundoo
RUN ln -s /etc/nginx/sites-available/fundoo /etc/nginx/sites-enabled
RUN rm -rf /etc/nginx/sites-enabled/default
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

