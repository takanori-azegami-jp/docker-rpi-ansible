# docker-rpi-ansible
RaspberryPi(64bit)にDockerでAnsibleを構築

## 環境
- kernel：Linux ホスト名 5.15.32-v8+ #1538 SMP PREEMPT Thu Mar 31 19:40:39 BST 2022 aarch64 GNU/Linux
- OS：Debian GNU/Linux 11 (bullseye)

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
