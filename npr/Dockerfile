FROM ubuntu:16.04

COPY . /app

run apt-get update && apt-get install -y \
    build-essential \
    cmake \
    curl \
    git \
    libcurl3-dev \
    libleptonica-dev \
    liblog4cplus-dev \
    libopencv-dev \
    libtesseract-dev \
    wget


RUN apt-get install -y openalpr openalpr-daemon openalpr-utils libopenalpr-dev
RUN  apt-get update -y && apt-get install -y default-jdk
RUN  apt-get install -y libavformat-dev libavcodec-dev libavutil-dev
ENTRYPOINT ["java", "-Djava.library.path=/app/lib", "-jar", "/app/anpr.jar"]

CMD [""]



