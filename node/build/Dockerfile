FROM registry.redhat.io/openshift3/jenkins-slave-base-rhel7:latest

USER root

RUN cd /tmp && \
    curl -O https://nodejs.org/dist/v15.4.0/node-v15.4.0-linux-x64.tar.xz && \
    tar -xvf node-v15.4.0-linux-x64.tar.xz && \
    cp node-v15.4.0-linux-x64/bin/node /usr/local/bin


RUN chown -R 1001:0 $HOME && \
    chmod -R g+rw $HOME
    
USER 1001