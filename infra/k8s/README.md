#important kubernetes commands
`kubectl apply -f <CONFIG FILE NAME.yml>` -> create pod
`kubectl get pods` -> list pods
`kubectl exec -it <pod> <cmd>` -> run command inside pod
`kubectl logs <pod>` -> log
`kubectl delete pod <pod>` -> delete
`kubectl describe pod <pod>` -> describe for debug info
replace `pod` with `deployments` for deployments options `service` for services
Docker runs individual container, k8s does all

#updating image used by a deployment
`deployment must use latest tag`
`update code`
`build image`
`push in docker hub`
`kubectl rollout restart deployment [depl_name]`

#Type of services
`ClusterIP` (default type)
`NodePort`
`Load Balancer`
`External Name`
