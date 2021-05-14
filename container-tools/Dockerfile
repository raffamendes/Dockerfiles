FROM quay.io/centos/centos:stream8

MAINTAINER Raffael Mendes (rmendes@redhat.com)

USER root

RUN yum install podman buildah skopeo -y && rm -rf /var/cache/yum

USER 1001
