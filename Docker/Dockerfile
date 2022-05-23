FROM python:3.9.12-bullseye

RUN apt update && \
    apt install -y vim && \
    apt clean

# アップデート： pip
RUN pip install --upgrade pip

WORKDIR /tmp

# インストール：Ansible
COPY ./requirements.txt /tmp/
RUN if [ -f "requirements.txt" ]; then pip install -r requirements.txt && rm requirements.txt*; fi

# フォルダ作成
RUN mkdir /opt/ansible
