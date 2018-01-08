# RocketMQ Docker

## 配置hosts文件 (注意修改ip)(域名在.env文件中)(可有可无)

- `192.168.16.240 namesrv.rocketmq.com`
- `192.168.16.240 m.a.broker.rocketmq.com`
- `192.168.16.240 s.a.broker.rocketmq.com`
- `192.168.16.240 m.b.broker.rocketmq.com`
- `192.168.16.240 s.b.broker.rocketmq.com`
- 修改.env文件中的ROCKETMQ_HM_HOST的IP


## RocketMQ base 

- 可以根据需要调整RocketMQ 内存参数(base/Dockerfile)

## RocketMQ 4.0.0-incubating

- `docker-compose up -d`

## RocketMQ 4.2.0

- `docker-compose up -d`

## RocketMQ Console (注意修改ip)

- `docker run -d -e "JAVA_OPTS=-Drocketmq.namesrv.addr=192.168.16.240:9876 -Dcom.rocketmq.sendMessageWithVIPChannel=false" -p 8080:8080 -t styletang/rocketmq-console-ng`

## RocketMQ资料

- `https://dist.apache.org/repos/dist/release/rocketmq/`
- `https://github.com/jingxizheng/rocketmq-docker-sample` (参考此例子进行局部调整)
