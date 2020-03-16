1. 查看docker容器内存、cpu等状态
   ```shell script
   docker stats $(docker ps --format={{.Names}})
   ```
2. 进入容器
   ```shell script
   docker exec -i -t 容器名称/容器ID /bin/bash
   ``` 
3. 查看容器日志
   ```shell script
   docker logs 容器名/容器ID
   ``` 