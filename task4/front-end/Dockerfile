FROM nginx:latest

# Copier les fichiers front-end dans l'image
COPY . /var/www/html/softy-pinko-front-end


# Copier la configuration Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
