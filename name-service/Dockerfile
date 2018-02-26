FROM java:8-jre

ADD ./target/name-service-0.0.1.jar /app/

ENTRYPOINT ["java", "-Xmx200m", "-jar", "/app/name-service-0.0.1.jar"]
EXPOSE 8090