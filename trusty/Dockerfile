# Speedus-lite container
From ubuntu:trusty
MAINTAINER Jorge Docampo <jorge.docampo@torusware.com>

ENV root_home /root

RUN apt-get -qqy update \
 && apt-get -qqy upgrade \
 && apt-get -qqy install wget unzip make gcc openjdk-7-jdk

ENV speedus_dir /opt/torusware/speedus
ENV netpipe_dir $speedus_dir/benchmarks/NetPIPE-C

WORKDIR /opt
RUN mkdir torusware \
 && cd torusware \
 && wget http://dl.torusware.com/speedus/release/speedus-lite-latest-linux.zip \
 && unzip speedus-lite-latest-linux.zip \
 && rm speedus-lite-latest-linux.zip \
 && ln -s speedus-lite-b* speedus \
 && cp speedus/README.txt $root_home/

COPY speedus /usr/bin/speedus

WORKDIR $netpipe_dir
RUN make
RUN cp NPtcp /usr/bin/NPtcp

WORKDIR $root_home
