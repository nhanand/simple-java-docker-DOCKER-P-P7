# simple-java-docker
A simple java app that runs on docker 

# Dockerfile

FROM openjdk:17-alpine

WORKDIR /app

COPY src/Main.java /app/Main.java

RUN javac Main.java

CMD ["java", "Main"]

# docker build  $$  docker push

docker build -t dockeruser534/java-app1:latest .

docker push dockeruser534/java-app1:latest 

https://github.com/nhanand/simple-java-docker-DOCKER-P-P7/blob/main/images/dockerimages.png


