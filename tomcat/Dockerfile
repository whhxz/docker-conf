FROM centos
COPY ./jdk8 /usr/local/share/jdk8
COPY ./tomcat9 /usr/local/share/tomcat9

ENV JAVA_HOME /usr/local/share/jdk8
ENV PAHT $JAVA_HOME/bin:$PATH

EXPOSE 8080
ENTRYPOINT /usr/local/share/tomcat9/bin/startup.sh && tail -F /usr/local/share/tomcat9/logs/catalina.out
