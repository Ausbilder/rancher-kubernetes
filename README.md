# rancher-kubernetes
Production ready RancherHA-GaleraHA-KubernetesHA Setup


#installation
Step 0: Create NFS Cluster
Requirements: 3VMs - 1C/2GB/xGB SSD - 10G Network - Ubuntu 18
Hostnames: nfs1 / nfs2 / nfs3

// Only required as Rancher backend if setup without RKE. With RKE Rancher will use k8s etcd backend. 
Step 1: Create Galera Cluster 
Requirement: 3 VMs - 2C/4GB/xGB SSD - 10G Network - Ubuntu 18
Hostnames: galera1 / garlera2 / galera3
Install based on http://galeracluster.com/documentation-webpages/docker.html

Step 2: Rancher HA Cluster
Requirement: 3 VMs - 1C/8GB/20GB HDD - RancherOS
Install based on https://rancher.com/docs/rancher/v2.x/en/installation/ha/kubernetes-rke/
