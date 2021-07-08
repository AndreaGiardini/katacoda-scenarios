# Installing ingress-nginx

You can now install ingress-nginx with: `kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.41.2/deploy/static/provider/baremetal/deploy.yaml`{{execute}}

At this point, our cluster is installed and exposed to the internet.

Try opening: https://[[HOST_SUBDOMAIN]]-[[KATACODA_HOST]].environments.katacoda.com/

To enter the right port, execute `kubectl get svc -A | grep NodePort | cut -f2 -d':' | cut -f1 -d'/'`{{execute}} and paste it on the webpage

If everything went well, you should see a "404 not found!" message


