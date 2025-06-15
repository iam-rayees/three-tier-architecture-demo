#
# Build
#
FROM maven:3.8.8-eclipse-temurin-11 AS build

WORKDIR /opt/shipping

COPY pom.xml .
RUN mvn dependency:resolve

COPY src ./src
RUN mvn package
