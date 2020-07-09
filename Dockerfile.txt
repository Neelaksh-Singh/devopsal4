FROM centos
WORKDIR /root/jen_task4
COPY . /var/www/html
RUN yum install httpd -y
CMD [ "/usr/sbin/httpd", "-D", "FOREGROUND" ]
EXPOSE 80