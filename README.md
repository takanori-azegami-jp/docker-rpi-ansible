# DockerBuild-RaspberryPi-Ansible
RaspberryPi(64bit)にDockerでAnsibleを構築

## Dockerビルド
```shell
$ docker image build -t test ./
```

## Playbook実行
```shell
$ docker run -v "${PWD}":/work:ro -v ~/.ansible/roles:/root/.ansible/roles -v ~/.ssh:/root/.ssh:ro --rm test ansible-playbook helloworld.yml
```

## 参考サイト
[AnsibleをDockerコンテナで動かす](https://qiita.com/satken2/items/f0ae21b9fb6e784e7ae8)
