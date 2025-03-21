Key|Value|Description|
---|-----|-----------|
replicaCount|1|Number of replicas|
container.port|8080|Port number|
extraEnv[0].name|REDIS_HOST|Redis host|
extraEnv[0].value|qod-redis-master|Value for Redis host|
extraEnv[1].name|REDIS_PORT|Redis port|
extraEnv[1].value|6379|Value for Redis port|
image.repository|qod|Repository for the image|
image.pullPolicy|IfNotPresent|Image pull policy|
image.tag||Image tag|
service.type|ClusterIP|Service type|
service.port|80|Service port|
ingress.enabled|true|Enable ingress|
ingress.className|nginx|Ingress class name|
ingress.hosts[0].host|chart-example.local|Ingress host|
ingress.hosts[0].paths[0].path|/qod|Ingress path|
ingress.hosts[0].paths[0].pathType|ImplementationSpecific|Ingress path type|
autoscaling.enabled|false|Enable autoscaling|
autoscaling.minReplicas|1|Minimum replicas for autoscaling|
autoscaling.maxReplicas|100|Maximum replicas for autoscaling|
autoscaling.targetCPUUtilizationPercentage|80|Target CPU utilization percentage|
autoscaling.targetMemoryUtilizationPercentage|80|Target memory utilization percentage|
redis.auth.enabled|false|Enable Redis authentication|
redis.replica.replicaCount|2|Number of Redis replicas|


