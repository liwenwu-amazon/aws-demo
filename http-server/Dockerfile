FROM amazonlinux:2
RUN yum update -y && \
    yum install -y iproute && \
    yum install -y iptables && \
    yum install -y iputils && \
    yum install -y net-tools && \
    yum install -y tcpdump && \
    yum clean all

WORKDIR /app

COPY http-servers /app

ENTRYPOINT /app/http-servers
