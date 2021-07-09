# Installing ingress-nginx

You can now install ingress-nginx with: `kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.41.2/deploy/static/provider/baremetal/deploy.yaml`{{execute}}

Even in this case, the deployment might take a couple of minutes.

Monitor the status of the applications by running `kubectl get po -n ingress-nginx`.
When all of them are marked as `Running` or `Completed`, you can proceed to the next step.


