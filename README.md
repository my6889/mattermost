# MatterMost

克隆项目

```
git clone https://github.com/my6889/mattermost.git
```

创建挂载目录

```
cd mattermost
mkdir -pv ./volumes/app/mattermost/{data,logs,config,plugins,client-plugins}
chown -R 2000:2000 ./volumes/app/mattermost/
```

修改docker-compose.yml文件

```
vim docker-compose.yml
```

* 修改数据库密码 **line12 & line42**
* 修改端口（非必须）
* 修改SSL（非必须）

启动服务

```
docker-compose up -d
```



官方文档：[ https://docs.mattermost.com/install/prod-docker.html#production-docker-setup-on-ubuntu ]( https://docs.mattermost.com/install/prod-docker.html#production-docker-setup-on-ubuntu )

