# Jupyter Notebook Deployment Instructions

Once all these yaml files have been deployed you will need to exec into the pod. Run kubectl get pods -n jupyter to show the pod name list. Copy the pod name and use it in the command below.
'''
kubectl exec -it jupyter-notebook-5ddb76d6d5-j8gzc -n jupyter -- /bin/bash
'''
Then run the following command:
'''
jupyter server list
'''
Copy the token from the URL and type exit.

Run the following command to port forward the web interface:
'''
kubectl port-forward deployment/jupyter-notebook -n jupyter 8888:8888
'''
In your web browser go to localhost:8888 and enter the token you just copied.