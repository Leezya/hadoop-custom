docker compose up -d 
docker compose up -d master
docker compose up -d worker

docker compose down master
docker compose down worker

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
docker logs hadoop-worker


nc -zv 10.68.71.113 8020

