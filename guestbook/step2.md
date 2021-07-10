# Deploy guestbook

Let's deploy our application by running:

`kubectl apply -f https://raw.githubusercontent.com/kubernetes/examples/master/guestbook/all-in-one/guestbook-all-in-one.yaml`{{execute}}

Then check the status of the application with:

`kubectl get po -A`{{execute}}

Make sure that all the Pods are shown as `Running` before moving to the next step

