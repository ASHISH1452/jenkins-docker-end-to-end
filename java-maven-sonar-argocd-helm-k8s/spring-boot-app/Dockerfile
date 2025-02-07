# Use an ARM-compatible base image
FROM openjdk:11-jre-slim

# Define the artifact path (ensure the path is correct)
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the application JAR to the container
COPY ${artifact} app.jar

# Set the entry point to run the Spring Boot application
ENTRYPOINT ["java", "-jar", "app.jar"]
