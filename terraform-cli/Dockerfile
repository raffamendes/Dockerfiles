FROM registry.access.redhat.com/ubi8/ubi

RUN yum install wget zip -y && \
    wget https://releases.hashicorp.com/terraform/0.12.13/terraform_0.12.13_linux_amd64.zip && \
    unzip terraform_0.12.13_linux_amd64.zip -d /usr/local/bin


USER 1001

CMD tail -f /dev/null





