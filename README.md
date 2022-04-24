# DockerBuild-RaspberryPi-Ansible
RaspberryPi(64bit)にDockerでAnsibleを構築

## Dockerビルド
Dockerfileのあるフォルダに移動して
```shell
$ docker-compose up -d --build
```

## Playbook実行
Playbookのあるフォルダに移動して
```shell
$ docker exec [コンテナid] ansible-playbook helloworld.yml
```

## 参考サイト
[AnsibleをDockerコンテナで動かす](https://qiita.com/satken2/items/f0ae21b9fb6e784e7ae8)
