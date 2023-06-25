# eks-cluster
two node groups: 1 with t3a.small and t3.small spot instances   //  and 1 with t3a.small on-demand instances
each node group must be in a different subnet (the ones you created so far)
install the following addons: coredns, ebs csi driver, kube-proxy and vpc-cni
deploy traefik using helm_release, from terraform and use some custom ports like 30443 and 30080
Create a an ALB and a target group pointed to traefik ports (30443 if you used this one)
deploy an nginx in eks
