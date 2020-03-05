FROM jenkins/jenkins

USER root

RUN curl -O https://bootstrap.pypa.io/get-pip.py  && \
    python get-pip.py && \
    pip install ansible --upgrade && \
    apt-get -y update && \
    apt-get -y upgrade && \
    mkdir /etc/ansible

COPY ansible.cfg /etc/ansible/ansible.cfg

USER jenkins
