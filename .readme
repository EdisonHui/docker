## 基于Docker构建Lnmp环境

#### 安装Docker 

- [install docker](https://docs.docker.com/install/linux/docker-ce/centos).
- [install docker compose](https://docs.docker.com/compose/install).

#### 加速源配置

- json配置
```bash
# 创建目录
sudo mkdir -p /etc/docker
# 写入{"registry-mirrors": ["https://9nf6ad5h.mirror.aliyuncs.com"]}
sudo vim /etc/docker/daemon.json
# 重新载入
sudo systemctl daemon-reload
# 重启服务
sudo systemctl restart docker
# 开机自启
sudo systemctl enable docker
```