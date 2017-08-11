## mysql 

#### Server 

> docker run --name mysql-server -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mysql

#### Client

> 



## mongo

>

## redis

#### Server

> docker run --name redis-server -p 6379:6379 -v $PWD/data:/data  			 -d redis 	redis-server --appendonly yes
> docker run --name redis-server -v $PWD/conf/redis.conf:/usr/local/etc/redis/redis.conf    redis 	redis-server /usr/local/etc/redis/redis.conf

#### Client

> docker run -it --name redis-client redis 					redis-cli -h 172.17.0.1
> docker run -it --name redis-client --link redis-server:redis --rm redis 	redis-cli -h redis -p 6379
