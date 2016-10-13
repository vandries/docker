FROM centos:7
MAINTAINER Valentin Andriès <valentin.andries@music-story.com>

RUN yum -y update
RUN yum -y install epel-release
RUN yum -y install nginx
RUN yum clean all

EXPOSE 80 443
VOLUME ["/etc/nginx/sites", "/var/log/nginx"]

CMD ["nginx", "-g", "daemon off;"]
