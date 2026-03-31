# cluster-cd

Helm chart for the **backend** EKS cluster (this folder at **repository root**): catalogue, user, ratings, dispatch, mongodb, mysql, shipping, and shared namespace/quotas/policies.

Includes **placeholder Services** for `cart`, `payment`, `rabbitmq`, `redis` (cluster-ab workloads) for DNS + Istio cross-cluster traffic.

See [`K8s/clusters/README.md`](../K8s/clusters/README.md) for multi-cluster context and install commands.

Options mirror the original Robot Shop chart (`values.yaml`: `image`, `psp`, per-workload `affinity` / `nodeSelector` / `tolerations`, etc.).
