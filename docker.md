## 安装镜像（即mongo）

> docker pull mongo

## 开启mongo服务器主进程（开启容器）

> docker run --name mongo-server -d mongo

> -d: 		后台运行容器，返回容器ID

> --name: 	为容器指定一个名称

> docker run --name mongo-client --link mongo-server:mongo -d application-that-uses-mongo
