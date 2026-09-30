# Tomcat & Java Application Interview Notes

## What is Apache Tomcat?
Tomcat is a Java servlet container used to run Java web applications.

## Spring Boot and Tomcat
Spring Boot applications using the servlet web stack commonly use embedded Tomcat by default. The application can be packaged as an executable JAR and started with java -jar without installing a separate Tomcat server.

## Standalone Tomcat
Traditional Java web applications can be packaged as WAR files and deployed to a separately managed Tomcat server. This differs from a typical Spring Boot executable JAR with embedded Tomcat.

## Interview questions
1. Embedded Tomcat vs standalone Tomcat?
2. JAR vs WAR?
3. How do you configure the application port?
4. How do you investigate HTTP 500 errors?
5. How do you investigate slow requests?
6. How do you inspect JVM memory usage?
7. What causes OutOfMemoryError?
8. How do readiness/liveness checks work for Java containers?
9. How would you expose Spring Boot through Kubernetes?
10. How would you safely roll out a new Java version?

## Production path
Client → Load Balancer/Ingress → Service → Pod → Spring Boot + embedded Tomcat → database/downstream services

For a 5xx error, correlate load-balancer metrics, application logs, traces, JVM metrics and downstream latency before deciding whether the problem is application, infrastructure or dependency related.
