#Start with a base image containing Java runtime
FROM maven:3.9-eclipse-temurin-17 AS build

# MAINTAINER instruction is deprecated in favor of using label
# MAINTAINER eazybytes.com
#Information around who maintains the image
LABEL "org.opencontainers.image.authors"="eazybytes.com"

# Add the application's jar to the image
COPY target/gatewayserver-0.0.1-SNAPSHOT.jar gatewayserver-0.0.1-SNAPSHOT.jar

# execute the application
ENTRYPOINT ["java", "-jar", "gatewayserver-0.0.1-SNAPSHOT.jar"]