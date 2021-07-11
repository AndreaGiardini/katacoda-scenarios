# Deploy Yelb

Let's deploy our application by running:

`kubectl apply -f https://raw.githubusercontent.com/mreferre/yelb/master/deployments/platformdeployment/Kubernetes/yaml/yelb-k8s-minikube-nodeport.yaml`{{execute}}

Make sure that all the Pods are shown as `Running` before moving to the next step

Run the following command until all the pods are shown as `Running`:

`kubectl get pod`{{execute}}
