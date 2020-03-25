FROM sjojo/jenkins:base
COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN mkdir /var/jenkins_home/init.groovy.d
ENV ADMIN_USERNAME admin
ENV ADMIN_PASSWORD password
COPY admin.groovy /var/jenkins_home/init.groovy.d/admin.groovy
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
