FROM openshift4/ose-jenkins-agent-base:v4.7

USER root

RUN yum install podman buildah skopeo -y && yum clean all && echo "1001:100000:65536" > /etc/subuid && echo "1001:100000:65536" > /etc/subgid

USER 1001

ENTRYPOINT ["/usr/bin/go-init", "-main", "/usr/local/bin/run-jnlp-client"]

