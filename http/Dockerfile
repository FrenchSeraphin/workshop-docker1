FROM httpd:alpine as imageTp1

EXPOSE 80

COPY htdocs/hello.html /usr/local/apache2/htdocs

CMD ["httpd", "-D", "FOREGROUND"]

FROM mysql:5.7 as imageTp2

EXPOSE 80

COPY mysql/bin/mysql.sh /usr/local/bin/

RUN ["chmod", "+x","/usr/local/bin/mysql.sh"]