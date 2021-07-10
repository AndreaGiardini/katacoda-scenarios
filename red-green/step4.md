# Let's deploy two applications

Use the following commands to deploy the `green` application:

`kubectl run green --image andreagiardini/green`{{execute}}

And the `red` application:

`kubectl run red --image andreagiardini/red`{{execute}}

Then make sure that both applications are shown as `Running`:

`kubectl get pod`{{execute}}

Let's expose the applications:

`kubectl expose pod green --port 80`{{execute}}

and

`kubectl expose pod red --port 80`{{execute}}
