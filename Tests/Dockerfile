FROM mysql:8
# MAINTAINER JoseCarlosPerejonEscobar josecarlos@medac.es
WORKDIR /var/lib/mysql
COPY C:\docker\mysqldb .
RUN apt-get update && apt-get -y upgrade
EXPOSE 3306

FROM drupal:9.0-apache
# MAINTAINER JoseCarlosPerejonEscobar josecarlos@medac.es
WORKDIR /drupal
COPY . .
RUN apt-get update && apt-get -y upgrade
EXPOSE 81