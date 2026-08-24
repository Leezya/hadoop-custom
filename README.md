docker compose up -d 
docker compose up -d master
docker compose up -d worker1

docker compose down master
docker compose down worker1

docker compose down -v master

```js
hadoop-master
 ├── NameNode
 └── ResourceManager

hadoop-worker1
 ├── DataNode
 └── NodeManager

hadoop-worker2
 ├── DataNode
 └── NodeManager
```



docker logs hadoop-master
docker logs hadoop-worker1


labsit12@labsit12:~/Documents/hadoop-custom$ nc -zv 192.168.80.227 8020
Connection to 192.168.80.227 8020 port [tcp/*] succeeded!
