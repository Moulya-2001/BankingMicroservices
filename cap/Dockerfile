FROM openjdk:alpine
RUN mkdir /mydata
ADD target/cap-1.0-SNAPSHOT.jar /mydata/cap-1.0-SNAPSHOT.jar
CMD java -cp /mydata/cap-1.0-SNAPSHOT.jar com.moulya.App
