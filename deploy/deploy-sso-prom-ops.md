# Deploy SSO Prom Ops

File `helm-prom-ops.yaml` for deploying Prometheus Operator.

## Prometheus instance running in master node for monitoring Etcd

- Create separate rules with Labels that `prom-ops-master` can select.
- Create Prometheus object `prom-ops-master`.
- Create Ingress and Service for `prom-ops-master` (file `ingress-prom-etcd`)