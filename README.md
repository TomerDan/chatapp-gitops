# chatapp-gitops

1. Install Argo CD
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

2. uder & password
password:
kubectl get secret argocd-initial-admin-secret -n argocd -o yaml > password.yaml
user:
admin

3. install application

kubectl apply -f application.yaml
