# Dockerfile to set up a contianer with ansible

FROM python:3.9-alpine

RUN adduser -D ansible 
USER ansible 
WORKDIR /home/ansible

RUN python -m pip install --user --no-cache-dir  ansible 

ENV PATH=.local/bin:$PATH

ENTRYPOINT ["/bin/sh"]