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

CMD java -Djava.library.path="/app/lib" -jar /app/npr.jar eu /etc/openalpr/openalpr.conf /usr/share/openalpr/runtime_data /app/npr/stills 1 LM55KVG



