FROM nginx:1.16-alpine

# Configuration
COPY config/default.conf /etc/nginx/conf.d

# Expose ports
EXPOSE 80

# Symlink the logs 
RUN ln -sf /dev/stdout /var/log/nginx/acces.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log

CMD ["nginx", "-g", "daemon off;"]
