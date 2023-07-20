ArgoCD Setup Minikube
## Installation

After Installing ArgoCD(Install it By Docs)

```bash
  kubectl get pods -n argocd

  kubectl get svc -n argocd

  kubectl edit svc argocd-server -n argocd
----------------------------------------------------------------
  ###Change Cluster Ip to NodePort and save :wq!
  ###To Port forward Or Tunnel
----------------------------------------------------------------
  minikube service argocd-server -n argocd
----------------------------------------------------------------
  ###Copy Paste the URL in the Browser
  ###To get The Password
----------------------------------------------------------------
  kubectl get secret -n argocd
  kubectl edit secret argocd-initial-admin-secret -n argocd
----------------------------------------------------------------
  ###copy the Password
----------------------------------------------------------------
  echo <paste> | base64 --decode

  ###Copy the password and Go to Browser
  ###USername:admin password:Paste


```
    
## Screenshots

![App Screenshot](https://drive.google.com/file/d/1QJeq87gN-7QtsFQWXauZLHWp1Dgo1tez/view?usp=sharing)

