FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install -y --no-install-recommends apt-utils build-essential sudo git ca-certificates
RUN git clone https://github.com/mkazhdan/ConformalizedMCF.git && cd ConformalizedMCF && make || true 
RUN mv /ConformalizedMCF/Bin/Linux/ConformalizedMCF /usr/bin
