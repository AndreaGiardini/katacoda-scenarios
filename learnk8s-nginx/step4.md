

`kubectl run green --image andreagiardini/green`{{execute}}
`kubectl run red --image andreagiardini/red`{{execute}}

`kubectl expose pod green --port 80`{{execute}}
`kubectl expose pod red --port 80`{{execute}}

