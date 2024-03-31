# Code Server Deployment Instructions

Once all these yaml files have been deployed, run the following command to port forward the web interface:
```
kubectl port-forward deployment/code-server -n codeserver 8080:8080
```
In your web browser go to localhost:8080