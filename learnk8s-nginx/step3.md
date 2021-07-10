# Access our Ingress online

At this point, our cluster is installed and exposed to the internet.

Open this URL in a new tab: https://[[HOST_SUBDOMAIN]]-[[KATACODA_HOST]].environments.katacoda.com/

This will be our `live` tab. It allows us to access our cluster from the
internet. The `live` page is asking you now to specify a port number...

Execute `kubectl get svc -A | grep NodePort | cut -f2 -d':' | cut -f1 -d'/'`{{execute}}

After executing the command, the terminal will print a number: that is the
port number that we need. Copy the number in the `live` tab and press
"Display port"

If everything went well, you should see a "404 not found" message

That's not very exciting right? Let's see if we can do better.
