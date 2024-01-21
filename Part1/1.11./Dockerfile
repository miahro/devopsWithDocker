#install Java &
FROM openjdk:8

EXPOSE 8080
WORKDIR /usr/src/app

COPY . .

#build project
RUN ./mvnw package

#command to run app
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]