# docker-maven
Shows how to use Maven with Docker
## Documentation
https://hub.docker.com/_/maven
## Usage on Windows 10
`cd` to a folder containing a `pom.xml` file and run the command `docker run -it --rm --name my-maven-project -v "%CD%":/usr/src/mymaven -w /usr/src/mymaven  maven:3.9-eclipse-temurin-17-alpine mvn install`
### Issues 
- Unable to delete `target` folder with `mvn clean` => fix : Manual deletion on host

