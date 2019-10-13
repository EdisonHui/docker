## 基于Docker构建Lnmp环境

#### 安装Docker 

- [install docker](http://get.daocloud.io/#install-docker).
- [install docker compose](http://get.daocloud.io/#install-compose).

#### 开机自启动

```bash
sudo vim /etc/docker/daemon.json
# {"registry-mirrors": ["https://9nf6ad5h.mirror.aliyuncs.com"]}
sudo systemctl daemon-reload
sudo systemctl enable docker
sudo reboot
```

#### 添加.env文件
```bash
sudo cp .env.example .env
```