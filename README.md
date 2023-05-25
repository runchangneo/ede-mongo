# Easy Development Environment - MongoDB
容易搭建的开发环境 - MongoDB
- Docker
- MongoDB

| 版本 | 支持 |
| -- | -- |
| 6 | &check; |

## 使用说明
### 先创建一个 `dev` 网络，所有服务都加入同一网络下便于容器互通
```
docker network create dev
```

### 配置文件
复制 `.env.example` 命名为 `.env`
```
cp .env.example .env
```
根据需要修改 `.env` 里的配置

### 启动容器
启动一个容器 mongo v6.x
```
docker compose up -d mongo6
```
启动所有容器
```
docker compose up -d
```

### 连接mongodb
默认连接URL
```
mongodb://mongoadmin:mongosecret@localhost:27017/
```
