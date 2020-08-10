# parity
1. Parity in statefulset
kubectl -f parity-stfset.yml

2. ConfigMaps for nodes

kubectl create configmap demo-cpec --from-file demo-spec.json
kubectl create configmap node0/1 --from-file node0/1.toml
kubectl create configmap nodepwds --from-file node.pwds
