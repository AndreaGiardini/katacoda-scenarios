# Exposing the applications to the internet

Now that the applications are running, let's expose them to the internet.

Run `kubectl apply -f /tmp/ingress-green.yml`{{execute}} to expose the
`green` application.

Refresh the page, what do you see?

Run `kubectl apply -f /tmp/ingress-red.yml`{{execute}} to expose the `red`
application.

Refresh the page, what do you see?

It is also possible to create more complex forwarding rules...

Run `kubectl apply -f /tmp/ingress-mix.yml`{{execute}}

Refresh the page, what do you see?
What happens if you access the `/red` path?
What happens if you access the `/green` path?
