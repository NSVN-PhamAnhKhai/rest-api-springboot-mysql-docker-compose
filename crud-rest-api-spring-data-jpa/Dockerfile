FROM openjdk:8-alpine
WORKDIR /app
COPY .mvn/ .mvn
COPY mvnw pom.xml ./
#RUN ./mvnw dependency:go-offline
COPY src ./src
CMD ["./mvnw", "spring-boot:run"]

# docker build --platform linux/amd64 -t spring-docker-demo .
# docker-compose -f docker-compose.dev.yml up --build