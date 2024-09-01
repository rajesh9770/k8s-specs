

CMDS:


kubectl create -f svc/go-demo-2-db-rs.yml
kubectl create -f svc/go-demo-2-db-svc.yml
kubectl create -f svc/go-demo-2-api-rs.yml
kubectl create -f svc/go-demo-2-api-svc.yml

kubectl delete -f svc/go-demo-2-db-rs.yml
kubectl delete -f svc/go-demo-2-db-svc.yml
kubectl delete -f svc/go-demo-2-api-rs.yml
kubectl delete -f svc/go-demo-2-api-svc.yml


RS:
To scale replica without modifying file.
kubectl scale --replicas=6 -f replicset.yaml
or kubectl scale --replicas=5 replicaset new-replica-set
