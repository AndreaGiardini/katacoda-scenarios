# Exposing the applications to the internet

Now that the applications are running, let's expose them to the internet.

Expose the `green` application with:

`kubectl apply -f /tmp/ingress-green.yml`{{execute}}

Refresh the `live` tab, what do you see?

Expose the `red` application with:

`kubectl apply -f /tmp/ingress-red.yml`{{execute}}

Refresh the `live` tab, what do you see?

It is also possible to create more complex forwarding rules...

Let's expose both applications with:

`kubectl apply -f /tmp/ingress-mix.yml`{{execute}}

Refresh the page, what do you see?

What happens if you access the `/red` path?

What happens if you access the `/green` path?
