# DockerBuild-RaspberryPi-Ansible
RaspberryPi(64bit)にDockerでAnsibleを構築

```shell
$ docker build ./
$ docker run -v "${PWD}":/work:ro -v ~/.ansible/roles:/root/.ansible/roles -v ~/.ssh:/root/.ssh:ro --rm satken2/ansible ansible-playbook playbook.yml
```

## 参考サイト
[AnsibleをDockerコンテナで動かす](https://qiita.com/satken2/items/f0ae21b9fb6e784e7ae8)
