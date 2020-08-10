# parity
1. Parity in statefulset
kubectl -f parity-stfset.yml

2. ConfigMaps for nodes

kubectl create configmap demo-cpec --from-file demo-spec.json

kubectl create configmap node0/1 --from-file node0/1.toml

kubectl create configmap nodepwds --from-file node.pwds


Log запуска ноды:

Loading config file from /home/parity/config/node0.toml

2020-08-10 07:47:41 UTC Starting Parity-Ethereum/v2.5.13-stable-253ff3f-20191231/x86_64-linux-gnu/rustc1.40.0

2020-08-10 07:47:41 UTC Keys path /tmp/parity0/keys/DemoPoA

2020-08-10 07:47:41 UTC DB path /tmp/parity0/chains/DemoPoA/db/d0678730db7ea493

2020-08-10 07:47:41 UTC State DB configuration: fast

2020-08-10 07:47:41 UTC Operating mode: active

Consensus signer account not found for the current chain. You can create an account via RPC, UI or `parity account new --chain /home/parity/chain/demo-spec.json --keys-path /tmp/parity0/keys`.


При попытке добавить команду создания эккаунта, ругается на путь к ключам, даже если путь существует
