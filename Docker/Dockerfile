FROM python:3.9.12-bullseye

RUN apt-get update && \
	apt-get install -y vim

WORKDIR /tmp

# アップデート： pip
RUN pip install --upgrade pip

# インストール：Ansible
COPY ./requirements.txt /tmp/
RUN if [ -f "requirements.txt" ]; then pip install -r requirements.txt && rm requirements.txt*; fi

# フォルダ作成
RUN mkdir /ansible
