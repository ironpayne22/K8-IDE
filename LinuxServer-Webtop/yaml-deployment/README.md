# Webtop Deployment Instructions

Once all these yaml files have been deployed, run the following command to port forward the web interface:
'''
kubectl port-forward deployment/webtop -n webtop 3000:3000
'''
In your web browser go to localhost:3000