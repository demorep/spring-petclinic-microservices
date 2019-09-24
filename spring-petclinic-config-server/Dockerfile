FROM openjdk:8-jre-alpine
VOLUME /tmp
ENV SPRING_PROFILES_ACTIVE docker

ADD target/spring-petclinic-config-server-2.1.4.jar /app.jar
ENTRYPOINT ["java", "-XX:+UnlockExperimentalVMOptions", "-XX:+UseCGroupMemoryLimitForHeap", "-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
