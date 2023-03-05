First go to folder in the argo-workflows service where Chart.yaml file is

> helm install argo-workflows . --namespace argoworkflow -f values-dev.yaml     <-- "argo-workflows" is the name defined in the Chart.yaml file
> helm upgrage argo-workflows . -f values-dev.yamöl

> helm list -all-namespaces     <-- here we can see the deployed chart

##############################################################################################

> https://localhost:2746