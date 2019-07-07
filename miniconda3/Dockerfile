FROM debian
LABEL maintainer=@garyli
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update --fix-missing && \
apt-get install -y \
wget bzip2 ca-certificates \
libglib2.0-0 libxext6 libsm6 libxrender1
RUN echo 'export PATH=/opt/conda/bin:$PATH' > /etc/profile.d/conda.sh && \
wget --quiet \
https://repo.continuum.io/miniconda/Miniconda3-4.3.11-Linux-x86_64.sh -O ~/miniconda.sh && \
/bin/bash ~/miniconda.sh -b -p /opt/conda && \
rm ~/miniconda.sh
 
