FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install -y --no-install-recommends apt-utils build-essential sudo git ca-certificates python3 python3-pip
RUN pip install trimesh 
RUN git clone https://github.com/mkazhdan/ConformalizedMCF.git && cd ConformalizedMCF && make || true 
RUN mv /ConformalizedMCF/Bin/Linux/ConformalizedMCF /usr/bin
