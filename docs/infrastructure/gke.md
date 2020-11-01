# GKE

## Infrastructure

Infrastructure As Code for GKE is in `iac/gcp` directory

Create VPC :

```shell
❯ make terraform-apply SERVICE=vpc ENV=prod
```

Create VPC :

```shell
❯ make terraform-apply SERVICE=observability ENV=prod
```

Create VPC :

```shell
❯ make terraform-apply SERVICE=gke ENV=prod
```

Configure kubectl

```shell
❯ make gcloud-kube-credentials ENV=prod
```

```shell
❯ kubectl get nodes
NAME                                                  STATUS   ROLES    AGE     VERSION
gke-portefaix-lab-prod-cluster-g-core-5d5d62be-tf15   Ready    <none>   7h37m   v1.18.9-gke.2501
```
