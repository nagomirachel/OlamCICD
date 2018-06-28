# Start with a base image containing Java runtime
FROM openjdk:8-jdk-alpine

# Add Maintainer Info
#MAINTAINER Rajeev Kumar Singh <callicoder@gmail.com>

# Add a volume pointing to /tmp
VOLUME /tmp

# Make port 8080 available to the world outside this container
EXPOSE 8080

# The application's jar file
ARG JAR_FILE=target/SpringBootHelloWorld-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container
ADD ${JAR_FILE} helloworld_demo.jar

# Run the jar file 
ENTRYPOINT ["java","-jar","/helloworld_demo.jar"]

#FROM openjdk:8-jdk-alpine
#COPY ./target/SpringBootHelloWorld-0.0.1-SNAPSHOT.jar /home/jenkins/
#WORKDIR /home/jenkins/
#EXPOSE 8080
#CMD ["java", "-jar", "SpringBootHelloWorld-0.0.1-SNAPSHOT.jar"]

