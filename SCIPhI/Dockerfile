FROM continuumio/miniconda3

RUN apt-get update -y
RUN apt-get install build-essential -y
RUN conda install -c conda-forge boost seqan-library dlib zlib cmake -y
RUN git clone --recurse-submodules https://github.com/amcpherson/SCIPhI.git
WORKDIR SCIPhI
RUN mkdir build && cd build && cmake .. && cmake --build . --config Release

ENTRYPOINT ["/SCIPhI/build/sciphi"]

