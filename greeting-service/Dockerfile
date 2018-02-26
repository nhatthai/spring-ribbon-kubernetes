FROM java:8-jre

ADD ./target/greeting-service-0.0.1.jar /app/

ENTRYPOINT ["java", "-Xmx200m", "-jar", "/app/greeting-service-0.0.1.jar"]
EXPOSE 8899