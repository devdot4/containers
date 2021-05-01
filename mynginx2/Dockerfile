FROM ubuntu
LABEL maintainer="Mike Ahmedov (devdot4@protonmail.com)"
RUN apt-get update && apt-get install nginx -y
RUN ln -sf /dev/stdout /var/log/nginx/access.log && ln -sf /dev/stderr /var/log/nginx/error.log
EXPOSE 80
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
