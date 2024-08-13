FROM openjdk:17.0.1-buster

ENV APP_HOME /usr/src/app

EXPOSE 8082

ARG JAR_FILE=gateway-0.0.1-SNAPSHOT.jar

COPY target/${JAR_FILE} $APP_HOME/app.jar

WORKDIR $APP_HOME

ENTRYPOINT ["java","-jar","/app.jar"]
