#FROM java:8-jre
#VOLUME /tmp
#ADD config_server.jar app.jar
#RUN bash -c 'touch /app.jar'
#EXPOSE 9988
#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

#FROM openjdk:8-jre-alpine
#EXPOSE 9988
#ADD config_server.jar /app.jar
#CMD ["java", "-jar", "/app.jar"]

FROM openjdk:8-jre-alpine
EXPOSE 9988
ADD *.jar /app.jar
CMD ["java", "-Xmx200m", "-jar", "/app.jar"]


#ADD ./target/config.jar /app/
#CMD ["java", "-Xmx200m", "-jar", "/app/config.jar"]
#
#EXPOSE 8888