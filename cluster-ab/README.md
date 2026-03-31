# cluster-ab

Helm chart for the **edge** EKS cluster (this folder at **repository root**): web, cart, payment, redis, rabbitmq, Wallarm ingress, and shared namespace/quotas/policies.

Includes **placeholder Services** (`remote-services-placeholder.yaml`) for `catalogue`, `user`, `ratings`, `shipping` so `rs-web` nginx can resolve DNS at startup; Istio supplies remote endpoints on cluster-cd.

See [`K8s/clusters/README.md`](../K8s/clusters/README.md) for multi-cluster context and install commands.

Options mirror the original Robot Shop chart (`values.yaml`: `image`, `psp`, `eum`, per-workload `affinity` / `nodeSelector` / `tolerations`, etc.).
