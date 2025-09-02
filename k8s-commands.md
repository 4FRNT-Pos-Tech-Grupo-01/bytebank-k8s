# Create local cluster (optional)

`kind create cluster --name bytebank`

# Load image into kind (optional)

`kind load docker-image bytebank:latest --name bytebank`

# Apply manifests

`kubectl apply -f k8s/`

# NGINX ingress

`kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.13.0/deploy/static/provider/kind/deploy.yaml`

  ### Test to see if it is running (optional)
  `kubectl get pods -n ingress-nginx`

# Force port foward (optional)

`kubectl port-forward svc/frontend-a-svc 3001:3000`

