#FROM openjdk:8-jdk-alpine
FROM maven
#RUN apt-get install maven
RUN mkdir /app  
COPY . /app
WORKDIR /app 
RUN mvn verify
CMD java -Xmx8m -Xms8m -jar target/words.jar