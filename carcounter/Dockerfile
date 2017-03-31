FROM ubuntu:16.04

COPY . /app

RUN  apt-get update -y && apt-get install -y default-jdk && apt-get install -y libopencv-dev
RUN  apt-get install -y libavformat-dev libavcodec-dev libavutil-dev

ENTRYPOINT ["java", "-Djava.library.path=/app/lib", "-jar", "/app/cars.jar"]

CMD [""]


