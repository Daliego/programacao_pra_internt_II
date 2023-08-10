FROM ubuntu:latest
LABEL authors="diego"

ENTRYPOINT ["top", "-b"]

# Use an official OpenJDK image as the base image
FROM openjdk:20

# Set the working directory
WORKDIR /app

# Copy the packaged Spring Boot JAR file into the container
COPY build/libs/demo1-0.0.1-SNAPSHOT-plain.jar app/app.jar

# Expose the port that your Spring Boot application uses
EXPOSE 8080

# Command to run the Spring Boot application
CMD ["java", "-jar", "app.jar"]
