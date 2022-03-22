# DockerBuild-RaspberryPi-Ansible
RaspberryPi(64bit)にDockerでAnsibleを構築

## Dockerビルド
Dockerfileのあるフォルダに移動して
```shell
$ docker image build -t helloworld/ansible ./
```

## Playbook実行
Playbookのあるフォルダに移動して
```shell
$ docker run -v "${PWD}":/work:ro -v ~/.ansible/roles:/root/.ansible/roles -v ~/.ssh:/root/.ssh:ro --rm helloworld/ansible ansible-playbook helloworld.yml
```

## 参考サイト
[AnsibleをDockerコンテナで動かす](https://qiita.com/satken2/items/f0ae21b9fb6e784e7ae8)
