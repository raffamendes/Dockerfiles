FROM registry.access.redhat.com/ubi8/openjdk-17:1.16-1.1687182768

COPY apache-ftpserver-1.2.0-bin.zip .

USER root

RUN microdnf install unzip -y && microdnf clean all 

RUN mkdir ftp && unzip apache-ftpserver-1.2.0-bin.zip -d ftp

EXPOSE 2121

ENTRYPOINT ["./ftp/apache-ftpserver-1.2.0/bin/ftpd.sh", "res/conf/ftpd-typical.xml"] 
