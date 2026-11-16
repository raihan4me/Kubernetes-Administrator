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

Learning Objectives
By the end of this lab you will be able to:

Build a multi-node cluster, install a CNI plugin, and inspect control-plane components, static pods and certificates.

Authenticate a new user with the CertificateSigningRequest API and authorise users and ServiceAccounts with Roles, ClusterRoles and bindings.

Deploy workloads with ConfigMaps, Secrets, probes and resource limits, and enforce ResourceQuota and LimitRange.

Perform rolling updates and rollbacks.

Control placement with taints, tolerations and node affinity.

Install add-ons with Helm and configure a HorizontalPodAutoscaler.

Expose applications with ClusterIP, NodePort and Ingress, and verify service discovery through CoreDNS.

Write ingress and egress NetworkPolicies, including the DNS egress exception.

Provide static (local PV) and dynamic (StorageClass) persistent storage, including StatefulSet volume claim templates.

Drain and uncordon nodes with PodDisruptionBudgets in place.

Back up etcd with etcdctl and restore it with etcdutl.

Troubleshoot node, control-plane and application failures using kubectl, crictl, systemctl and journalctl.

