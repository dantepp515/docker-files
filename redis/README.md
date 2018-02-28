##Redis Docker

1. 根据需要编辑目录下的redis.conf;

2. 通过Docker命令生成Docker Image；
````
	docker build -it redis .

````

3. 运行：
````
	docker run -p 6379:6379 -v /Users/dante/idea.workspace/dante/docker-files/redis/redis.conf:/usr/local/etc/redis/redis.conf --name myredis -d my-simple-redis redis-server /usr/local/etc/redis/redis.conf
````


