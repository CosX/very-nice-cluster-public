# Karls Home Lab K3s Cluster using Recycled Laptops

See my blog post on setting up this cluster: https://blog.solgard.solutions/posts/create-a-low-power-home-lab-using-k3s-and-old-laptops. This README provides an overview of setting up and managing a home lab Kubernetes (K3s) cluster with the following services:

- **AdGuard**: DNS server with ad blocking capabilities.
- **Blog**: A personal blog running on a lightweight platform.
- **Cloudflare Daemon**: Cloudflare Tunnel for secure external access.
- **Grafana**: Dashboard for visualizing metrics.
- **Home Assistant**: Home automation platform.
- **Immich**: Open-source, self-hosted photo and video backup solution.
- **Kepler**: Kubernetes-based energy consumption monitoring.
- **Longhorn**: Distributed block storage for Kubernetes.
- **MetalLB**: Load balancer for bare-metal Kubernetes.
- **NFS**: Network File System for shared storage.
- **Prometheus**: Monitoring and alerting toolkit.
- **Prometheus Blackbox Exporter**: Probes endpoints over HTTP, HTTPS, DNS, TCP, ICMP, and more.

## Prerequisites

Before setting up the cluster, ensure the following:

- **K3s Installed**: [K3s](https://k3s.io/) is a lightweight Kubernetes distribution. Follow the official documentation for installation.
- **Helm Installed**: [Helm](https://helm.sh/) is used to manage Kubernetes applications.
- **GitOps Setup**: Using [Flux](https://fluxcd.io/) for GitOps is recommended but optional.
- **NFS Server**: An existing NFS server setup if using NFS for persistent volumes.
