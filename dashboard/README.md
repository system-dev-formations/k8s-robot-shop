# Utiliser le Dashboard
L'installation du dashboard est faite a partir du playbook ansible.  
[voir] (https://github.com/system-dev-formations/install-k8s-lunanode.git)  
Vous devez avoir l' alias k et la completion des commandes pour retrouver le port d'ecoute 
du dashboard dans votre cluster Kubernetes. 

## Obtenir le token de connexion 
```
kubectl -n kube-system describe secret $(kubectl -n kube-system get secret |
    grep admin-user | awk '{print $1}' )
```
## Dans votre navigateur firefox 
Tapez l'adresse IP de votre cluster et le port d'ecoute de votre dashboard.   
Comme vous n'avez pas de certificat SSL valide il faut forcer la connexion de votre nagivateur.


