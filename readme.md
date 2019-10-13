## 基于Docker构建Lnmp环境

#### 安装Docker 

- [install docker](http://get.daocloud.io/#install-docker).
- [install docker compose](http://get.daocloud.io/#install-compose).
- [config mirrors](https://www.daocloud.io/mirror#accelerator-doc).

#### 开机自启动

```bash
sudo systemctl daemon-reload
sudo systemctl enable docker
sudo reboot
```

#### 添加.env文件
```bash
sudo cp .env.example .env
```