**Install Argocd Using operator**

- [Pre-requisites](#pre-requisites)
- [What](#what)
- [How](#how)
  
# Pre-requisites
 
 1. Helm binary installed
 2. Openshift Cluster
   
# What

Installs argocd instance to your openshift Cluster using helm

Creates the following

1.  New project called argocd
2.  Operator group
3.  Subscription
4.  Installs argocd operator
5.  New argocd application with Openshift auth enabled.

# How

```
helm upgrade --install argocd ./argocd --namespace argocd --create-namespace --wait
Release "argocd" has been upgraded. Happy Helming!
NAME: argocd
LAST DEPLOYED: Fri May 14 13:15:17 2021
NAMESPACE: argocd
STATUS: deployed
REVISION: 1
```




