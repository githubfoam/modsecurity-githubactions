# https://hub.docker.com/_/ubuntu
FROM ubuntu:latest
LABEL org.opencontainers.image.authors="githubfoam"

WORKDIR /tmp

RUN apt-get update -qy && \ 
    apt-get dist-upgrade -yq && \
    apt-get purge unattended-upgrades && \
    apt-get clean all

# ModSecurity 3.0 (aka libmodsecurity)
# Nginx users should use ModSecurity 3
# Apache users should use ModSecurity the 2.9 branch 
# The ModSecurity module for Apache

# RUN apt-get install libapache2-mod-security2 -qy
# RUN apt-get install \ 
#         libapache2-mod-security2 -qy &&\
#         # enable this module
#         a2enmod security2

# RUN mkdir /home/vagrant && \
#     # create a user ‘builder‘ with home directory ‘/home/vagrant‘, 
#     # default shell /bin/bash and adds extra information about user
#     useradd -m -d /home/vagrant -s /bin/bash -c "builder" -U vagrant  && \
#     chown -R vagrant /home/vagrant

# USER vagrant