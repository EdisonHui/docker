## 基于Docker构建Lnmp环境

#### 安装Docker 

- [install docker](https://docs.docker.com/install/linux/docker-ce/centos).
- [install docker compose](http://get.daocloud.io/#install-compose).

#### 加速源配置

```bash
sudo mkdir -p /etc/docker
sudo vim /etc/docker/daemon.json
# {"registry-mirrors": ["https://9nf6ad5h.mirror.aliyuncs.com"]}
sudo systemctl daemon-reload
sudo vim /etc/sysctl.conf
# net.ipv4.ip_forward=1
# vm.max_map_count=262144
sudo systemctl enable docker
sudo reboot
```

#### 添加.env文件
```bash
sudo cp .env.example .env
```