# Starting Kubernetes

Kubernetes is a complex software with many moving components interacting
with each other. Let's spend some time discovering the basic components...

Start the cluster by running the `launch.sh`{{execute}} script.

This will create a Kubernetes cluster made of two servers.

Wait for the script to complete before proceeding. You can check the status of the nodes by running `kubectl get nodes`{{execute}} once you see both of them marked as `Ready` you can move to the next section.

