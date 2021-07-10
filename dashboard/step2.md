# Deploy guestbook

Let's deploy our application by running:

`kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.2.0/aio/deploy/recommended.yaml`{{execute}}

End expose the dashboard:

`kubectl patch svc -n kubernetes-dashboard kubernetes-dashboard -p '{"spec": {"type": "NodePort"}}'`{{execute}}

Make sure that all the Pods are shown as `Running` before moving to the next step

