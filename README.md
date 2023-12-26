# docker-maven
Shows how to use Maven with Docker
## Use on Windows 10
docker run -it --rm --name my-maven-project -v "%CD%":/usr/src/mymaven -w /usr/src/mymaven  maven:3.9-eclipse-temurin-17-alpine mvn clean install
