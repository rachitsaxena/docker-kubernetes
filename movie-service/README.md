# Setup and running application

### Docker commands
Starting the container from image using one of the following commands:
* docker run -p 8080:8080 --add-host=host.docker.internal:host-gateway --name movie-service --rm --env="app.movies.mysql.host=host.docker.internal" --env="app.movies.mysql.port=3306" --env="app.movies.mysql.schema=movie_service" --env="app.movies.mysql.username=root" --env="app.movies.mysql.password=mysecret" rachits/movie-service
* docker run -p 8080:8080 --env-file movie-service.env --rm --add-host=host.docker.internal:host-gateway --name movie-service rachits/movie-service
