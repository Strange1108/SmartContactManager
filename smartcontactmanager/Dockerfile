# FROM ubuntu:latest AS build

# RUN apt-get update
# RUN apt-get install openjdk-21-jdk -y
# COPY . .

# RUN ./gradlew bootJar --no-daemon

# FROM maven:3.8-openjdk-17 AS build

# EXPOSE 8080

# COPY --from=build /build/libs/demo-1.jar app.jar

# ENTRYPOINT ["java", "-jar", "app.jar"]


# Use an official Maven image as the base image
FROM maven:3.8-openjdk-17 AS build

# Set the working directory in the container
WORKDIR /app

# Copy the Maven project file
COPY pom.xml .

# Download dependencies
RUN mvn dependency:go-offline

# Copy the application source code
COPY src ./src

# Build the application
RUN mvn package

# Create a new image with only the JRE
FROM openjdk:17-jdk-slim

# Set the working directory in the container
WORKDIR /app

# Copy the JAR file from the build stage
COPY --from=build /app/target/demo-1.jar app.jar

# Expose the port the app runs on
EXPOSE 8080

# Define the command to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
