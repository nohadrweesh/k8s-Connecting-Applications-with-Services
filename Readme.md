# Description

Following this K8S tutorial
https://kubernetes.io/docs/tutorials/services/connect-applications-service/

- K apply -f nginx_deployment.yaml
- k get pods -l run=my-nginx -o custom-columns=POD_IP:.status.podIPs
- kubectl expose deployment/my-nginx
- kubectl scale deployment my-nginx --replicas=0; kubectl scale deployment my-nginx --replicas=2;