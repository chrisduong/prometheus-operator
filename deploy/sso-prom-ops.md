# Deploy SSO Prom Ops

File `helm-prom-ops.yaml` for deploying Prometheus Operator.

## Prometheus instance running in master node for monitoring Etcd

- Create separate rules with Labels that `etcd-prometheus` can select.
- Create Prometheus object `etcd-prometheus`.
- Create Ingress and Service for `etcd-prometheus` (file `ingress-prom-etcd`)

## TODOs

- Check Grafana's readiness.
- Integrate BasicAuth.
- Where does the default Scraping come from
  - Rule can affect the Scrapping also.
- How to aggregate Alerts between 2 Prom instances.
