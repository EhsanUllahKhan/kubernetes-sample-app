# kubernetes-sample-app
Demo apps for kubernetes clusters

For openshift applications. 
1. pacman application and socks shop

oc adm new-project <project_name>
---
oc create serviceaccount <sa_name>
---
oc adm policy add-scc-to-user privileged -n <project_name> -z <sa_name>
---


# Forcefully delete PVC 

kubectl patch pvc {PVC_NAME} -p '{"metadata":{"finalizers":null}}'

