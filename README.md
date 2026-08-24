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