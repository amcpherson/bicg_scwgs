FROM rocker/tidyverse:4.1.0

RUN apt-get update -y
RUN apt-get install git -y
RUN git clone https://github.com/amkozlov/cellphy
WORKDIR cellphy
RUN bash ./install.sh
RUN bash ./cellphy.sh -h

