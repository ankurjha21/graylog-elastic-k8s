# graylog-elastic-k8s
Deploying Graylog and Elastic search on kubernetes
# Single-pod-graylog-with-PVC
single Statefulset graylog cluster kubernetes setup with PVC


All deployment are stateful set with PVC.

```
kubectl create -f .
```

Table of content 

| Statefulsets        | Image version           | PVC mountpath  |
| ------------- |:-------------:| -----:|
| Elasticsearch      | elasticsearch:6.5.0 | /usr/share/elasticsearch/data |
| Graylog      | graylog/graylog:3.0.1      |   /usr/share/graylog/data/journal |
| MongoDB | mongo:3      |    /data/db |
