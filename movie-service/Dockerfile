FROM openjdk:17-alpine

WORKDIR /app

COPY ./build/libs/movie-service-0.0.1-SNAPSHOT.jar .

RUN mv movie-service-0.0.1-SNAPSHOT.jar movie-service.jar

EXPOSE 8080

CMD ["java", "-jar", "movie-service.jar"]