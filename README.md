# docker_learn
docker使用学习

## dns配置

```vi /etc/defaults/docker```
在文件中写入
```
DOCKER_OPTS="--dns 8.8.8.8 --dns 8.8.4.4"
```
