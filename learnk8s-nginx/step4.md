

`kubectl run green --image andreagiardini/green`{{execute}}
`kubectl run red --image andreagiardini/red`{{execute}}

`kubectl expose pod green --port 80`{{execute}}
`kubectl expose pod red --port 80`{{execute}}

```
apiVersion: "networking.k8s.io/v1beta1"
kind: "Ingress"
metadata:
  name: "example-ingress"
spec:
  rules:
  - http:
      paths:
      - path: "/red"
        pathType: "Prefix"
        backend:
          serviceName: "red"
          servicePort: 80
```
