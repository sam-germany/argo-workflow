First go to folder in the argo-workflows service where Chart.yaml file is, after that we can executer "helm install" or "helm upgrade"
as defined below

> helm install argo-workflows . --namespace argo -f values-dev.yaml     <-- "argo-workflows" is the name defined in the Chart.yaml file
> helm upgrage argo-workflows . -f values-dev.yamöl

> helm list -all-namespaces     <-- here we can see the deployed chart

> kubectl -n argo port-forward deployment/argo-server 2746:2746         <-- like this we can make a port-forward
##############################################################################################

>  kubectl -n argo create -f 01-test-workflow.yaml          <-- go to "Workflow" folder then just try to create directly this Workflow


 