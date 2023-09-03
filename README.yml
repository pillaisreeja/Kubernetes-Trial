# Kubernetes-Trial
apiVersion: apps/v1
kind: ReplicaSet
metadata: 
 name: myrs
spec:
 replicas: 4
 selector: # This is used to query the cluster before creating the replicas
  matchLabels:
   type: webserver
 template: # this is pod template using which replicas will be created
  metadata:
   labels: # purpose of labels is to group replicas for quering in cluster
    type: webserver
    author: sonal
  spec: # this is specification of pod/replica
   containers:
    - name: c1
      image: nginx
