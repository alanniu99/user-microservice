FROM java:8
VOLUME /tmp
ADD user-microservice-0.1.0.jar app.jar
ADD users.csv /data/
RUN bash -c 'touch /app.jar'
EXPOSE 9000
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
