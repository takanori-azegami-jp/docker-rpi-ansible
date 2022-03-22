FROM python:3.9.11-bullseye

RUN pip install pip --upgrade
RUN pip install ansible

RUN apt-get update -y && \
  DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
  sshpass

WORKDIR /work