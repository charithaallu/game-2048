# game-2048

This explains how to create a EKS cluster with fargate. 
This include deploying a game in the EKS cluster called game-2048. It has depoly, service and ingress (ALB) manifests.
ALB controller is the ingress controller deployed using helm charts.
For ALB controller to talk to the ingress created inside EKS, IAM open ID connect (OIDC) is configured and associated with the cluster.
ALB controller specified IAM policy was downloaded and attached to the service account that was created inside the EKS cluster.

