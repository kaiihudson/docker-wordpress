FROM nginx
RUN apt-get update && apt-get install -y nginx-extras

RUN usermod -a -G root www-data

RUN mkdir -p /proyectos && chown -R www-data:www-data /proyectos
RUN mkdir -p /proyectos/wp && chown -R www-data:www-data /proyectos/wp/


EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]