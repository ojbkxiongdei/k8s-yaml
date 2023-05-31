# k8s-yaml
各种k8s服务的yaml

# k8s info(crete by sealos 4.1.7)

|	NAME		|	STATUS	|	ROLES			| AGE | VERSION | INTERNAL-IP | EXTERNAL-IP | OS-IMAGE                	 | KERNEL-VERSION                 |CONTAINER-RUNTIME |
|-----------------------|---------------|------------------------|-----|---------|-------------|-------------|--------------------------------|--------------------------------|------------------|
| k8s-master-01		| Ready		| control-plane		| 17d | v1.25.8 | 10.10.18.1   |<none>	      | CentOS Linux 7 (Core)      | 6.2.11-1.el7.elrepo.x86_64 | containerd://1.6.20 |
| k8s-worker-01		 | Ready		| worker			| 17d | v1.25.8 | 10.10.18.11 |<none>	  | CentOS Linux 7 (Core)      | 6.2.11-1.el7.elrepo.x86_64 | containerd://1.6.20 |
| k8s-worker-02		 | Ready		| worker			| 17d | v1.25.8 | 10.10.18.12 |<none> 	  | CentOS Linux 7 (Core)      | 6.2.11-1.el7.elrepo.x86_64 | containerd://1.6.20 |
| k8s-worker-03		 | Ready		| worker			| 17d | v1.25.8 | 10.10.18.13 |<none> 	  | CentOS Linux 7 (Core)      | 6.2.11-1.el7.elrepo.x86_64 | containerd://1.6.20 |

# 服务作用描述
## Observability （log、metrics、trace、event）
+ elasticsearch-cluster.yml   es集群
+ elasticsearch-single.yml    es单节点
+ event-exporter.yml          k8s事件收集器（推荐）
+ fluentbit.yml               日志事件采集器
+ jaeger.yml                  链路追踪
+ kibana.yml                  日志可视化分析平台
+ kube-eventer.yml            阿里开源k8s事件收机器
+ victoriametrics.yml         tsdb，监控指标远程存储

## CICD
+ code-server.yml      Cloud IDE
+ gitlab-redis.yml     gitlab redis
+ gitlab-postgre.yml   gitlab postgre
+ gitlab.yml           gitlab服务
+ jenkins.yml          jenkins服务
+ harbor.doc           hardor服务
