## 机器评估

测试环境，只支持 Centos7.5+ 的系统版本

| 分布名称     | 服务简介                                    | 机器数量    | 配置要求  |
| :----------- | -------------------------------------------| ----------- | --------- |
| bcs-web      | bcs 配置，监控，导航，thanos，Harbor 等服务  | 2-3 台       | 8C 16G 1T   |
| bcs-server   | bcs 后台服务，etcd，mongodb，zk 等服务      | 3-5 台(奇数) | 8C 16G 300G |
| K8S 集群     | 业务集群，可以将业务进程运行在该 K8S 集群中   | 3+N         | 4C 8G 300G  |
| Mesos 集群   | 业务集群，可以将业务进程运行在该 mesos 集群中 | 3+N         | 4C 8G 300G  |

> 生产环境，建议根据实际情况增加主机数量。
