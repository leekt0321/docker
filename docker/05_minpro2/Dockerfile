FROM centos:7

RUN yum -y install httpd php && yum clean all

ADD src.tar /var/www/html

VOLUME ["/var/www/html", "/var/log/httpd"]
EXPOSE 80/tcp

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
# ENTRYPOINT /usr/sbin/httpd -D FOREGROUND
