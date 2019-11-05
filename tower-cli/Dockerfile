FROM registry.access.redhat.com/ubi7/ubi  

RUN yum install wget -y && \
    wget https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm && \
    yum install ./epel-release-latest-*.noarch.rpm -y && \
    yum update -y && \
    yum install python-pip -y && \
    pip install --upgrade pip && \
    pip install ansible-tower-cli

USER 1001

CMD tail -f /dev/null

