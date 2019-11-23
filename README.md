microservice 微服务架构

通信层

网络传输

HTTP + RESTFUL
GET POST PUT DELETE
#### RPC（rpc客户端和rpc服务端） RPC（远程过程调用）
TPC RPC调用
Thrift
Dubbox
gRpc
#### 消息传递
Json
Thrift
protobuf
服务发现&服务注册

分布式存储

Consul
Etcd 注册中心

Zookeeper

etcd注册中心

分布式一致性

基于raft一致性协议

etcd使用场景

服务注册和发现

共享配置

分布式锁

Leader选举

服务注册和发现思考

- 一定需要一致性吗
- EUREKa 是一个ap系统， netflix开发，用来做高可用的注册中心
- 一般cp就可以了
CAP原理
C：consistency，每次总是能够读到最近写入的数据或者失败
A：avaiable，每次请求都能读到数据
P: partition tolerance，系统能够继续工作，不管任意哥消息由于网络原因失败
#### 负载均衡

