#Docker file for apache for demoapp
FROM centos:7
MAINTAINER omkarmate431@gmail.com
RUN yum -y update
ADD scripts /opt/
RUN chmod 777 opt/*
RUN /opt/packages
ADD code /var/www/html
#COPY code/* /var/www/html
ENV MY_DB_HOST_WRITE=test
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]
