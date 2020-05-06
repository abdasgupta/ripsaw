FROM quay.io/abdasgupta/ansible-operator:0.16.0-dev

COPY group_vars/ ${HOME}/group_vars/
COPY roles/ ${HOME}/roles/
COPY watches.yaml ${HOME}/watches.yaml
COPY playbook.yml ${HOME}/playbook.yml
#Just a workaround
ENV HOME /opt/ansible

USER root
RUN yum install -y redis
USER 1001
