# ArgoCD
ArgoCD

Step
1. Create a Git Repository

2. Connect ArgoCD to Git
    argocd repo add https://github.com/chakkaringit/ArgoCD.git --username <your-username> --password <your-password>

3. Create an Application in ArgoCD
argocd app create my-app \
    --repo https://github.com/chakkaringit/ArgoCD.git \
    --path app1 \
    --dest-server https://kubernetes.default.svc \
    --dest-namespace default
