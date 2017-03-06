FROM ubuntu:16.04

COPY . /app

RUN  apt-get update -y && apt-get install -y default-jdk && apt-get install -y libopencv-dev

CMD java -Djava.library.path="/app/lib" -jar /app/cars.jar 1 2000
