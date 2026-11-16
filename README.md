# Kubernetes Administrator (CKA) Lab
Scenario. You are the new platform administrator at a small online retailer. The development team is moving its "shop" application to Kubernetes. You will stand up a multi-node cluster and run the shop on it, and along the way you will: grant developers least-privilege access,
schedule workloads correctly,
expose the application,
lock down the network,
provide persistent storage,
perform node maintenance,
back up and restore etcd,
diagnose a broken cluster under pressure.
What you will build. A three-node Kubernetes v1.30 cluster with kind on Ubuntu 24.04: one control-plane node and two workers, Calico as the CNI (so NetworkPolicy is enforced), ingress-nginx, metrics-server (Helm), and a two-tier application (nginx frontend plus HTTP echo backend) with RBAC, quotas, autoscaling, network policies and persistent volumes.
