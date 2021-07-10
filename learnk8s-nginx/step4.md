# Let's deploy two applications

Use the following commands to deploy the `green` and `red` application:

`kubectl run green --image andreagiardini/green`{{execute}}
`kubectl run red --image andreagiardini/red`{{execute}}

Then make sure that both applications are `Running`:

`kubectl get pod`{{execute}}

Let's expose the applications:

`kubectl expose pod green --port 80`{{execute}}
`kubectl expose pod red --port 80`{{execute}}
