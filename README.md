# simple-java-docker
A simple java app that runs on docker 

# Dockerfile

FROM openjdk:17-alpine

WORKDIR /app

COPY src/Main.java /app/Main.java

RUN javac Main.java

CMD ["java", "Main"]

# docker build 

docker build -t dockeruser534/java-app1:latest .

# docker push

docker push dockeruser534/java-app1:latest 

\\wsl.localhost\Ubuntu-20.04\home\ubuntu\project_repo\simple-java-docker-DOCKER-P-P7\images\dockerimages.png

