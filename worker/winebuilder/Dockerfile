FROM jenkins/inbound-agent
USER root
RUN grep '^deb ' /etc/apt/sources.list | sed 's/deb /deb-src /' >> /etc/apt/sources.list
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get build-dep wine -y
