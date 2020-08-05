# v2ray-docker

### 安装 docker 和 docker-compose
```
curl -fsSL https://get.docker.com | bash

curl -L "https://github.com/docker/compose/releases/download/1.25.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

chmod a+x /usr/local/bin/docker-compose
```

###安装 git

yum -y install git

### Clone docker 和配置文件
```
git clone https://github.com/ymlsn/v2-v2b.git

cd v2-v2b

# 配置
修改 config.json 中的 poseidon 下面的 nodeId, webapi, 和 token

# 启动docker
systemctl start docker

# 启动v2ray
docker-compose up -d
```
###  说明

- 仅适配 [v2board](https://github.com/v2board/v2board) 面板平台
- 仅适用于v2Ray Ws 模式
