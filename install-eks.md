## Install using Fargate

```
eksctl create cluster --name demo-cluster --region ca-central-1 --fargate
```

Create Fargate Profile to get a new namespace

eksctl create fargateprofile \
    --cluster demo-cluster \
    --region ca-central-1 \
    --name alb-sample-app \
    --namespace game-2048

## Deploy the deployment, service and ingress directly using below github link for game-2048

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```

## refer deployment.yml folder for details about deployment, service and ingress.
