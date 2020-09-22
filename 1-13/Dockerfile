FROM openjdk:8
RUN apt update && apt install -y git
RUN git clone https://github.com/docker-hy/spring-example-project.git
WORKDIR /spring-example-project

EXPOSE 8080
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar