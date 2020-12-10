FROM nginx
RUN echo '这是一个本地构建的nginx镜像' \
 && apt-get update \
 && apt-get install openssl \
 && apt-get install libssl-dev --assume-yes \
 && apt-get install vim --assume-yes \
 && apt-get install procps --assume-yes \
 && apt-get install yum --assume-yes

COPY conf/nginx.conf  /etc/nginx/nginx.conf

EXPOSE 80 8080 443

#ENTRYPOINT ["/usr/sbin/nginx", "-c", "/etc/nginx/nginx.conf"]
