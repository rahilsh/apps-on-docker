FROM debian:9

RUN echo "deb http://10.47.4.220:80/repos/oracle-java/8 /" >> /etc/apt/sources.list
RUN DEBIAN_FRONTEND=noninteractive apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y procps vim
RUN DEBIAN_FRONTEND=noninteractive apt-get -y install mysql-client
RUN DEBIAN_FRONTEND=noninteractive apt-get -y install curl
RUN DEBIAN_FRONTEND=noninteractive apt-get -y install dnsutils

CMD ["sleep", "infinity"]
