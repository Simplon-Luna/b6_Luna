# Plan d'action présentation  

# Plan d'action

00. **Scrum quotidien**
Réflexion personnelle quotidiennes avec compte-rendu immédiat et désignation des premières tâches du jour.
Réunions fréquente avec d'autres co-apprenants pour étudier des solutions aux problèmes rencontrés à plusieurs.

1.  **Création Kanban**

2.  **Lecture des documentations Kubernetes en Azure CLI & Powershell**

3.  **Topologie de l'infrastructure**
Infrastructure Plannifiée


```mermaid
flowchart LR

    subgraph AZ [Azure]
    lb(Load Balancer)
    conf(configuration <br> file)

        subgraph KT [Kubernetes Controller]
            subgraph KTVT [KT Vote Template]
            ktd1(Kubelet)
            dd1(Docker Daemon)
            vote1(Voting App Container)
            red1(Redis Container)
            end
        
        subgraph n1 [Node 1]
        cont1(containers)
        end

        subgraph n2 [Node 2]
        cont2(containers)
        end

        end

    end 

    

    classDef rouge fill:#faa,stroke:#f66,stroke-width:4px,color:#fff,stroke-dasharray: 5 5;
    class n1,n2, rouge;
    classDef sec fill:#aff,stroke:#025,stroke-width:2px,color:#003;
    class AZ, sec;
    classDef ter fill:#f0f,stroke:#025,stroke-width:2px,color:#003;
    class KTVT,vmadmin, ter;
    classDef vert fill:#af0,stroke:#025,stroke-width:2px,color:#003;
    class lb, vert;
    classDef blanc fill:#fff,stroke:#025,stroke-width:2px,color:#003;
    class Web, blanc;

```

0.   **Liste tâches à faire sur le [Board](https://github.com/users/Simplon-Luna/projects/1/views/1)**
Création et gestion des tâches dans l'ordre du plan d'action. Attribution des tâches aux membres du groupe au fur et à mesure.

# **Commandes utilisées**


### list services
kubectl get service 

### list pods
kubectl get pods

### describe running and failed pod
kubectl describe pods [name]


### Create AKS Cluster

az aks create -g b6luna -n AKSClusterLuna --enable-managed-identity --node-count 2 --enable-addons monitoring --enable-msi-auth-for-monitoring  --generate-ssh-keys

### Connect to the cluster

az aks get-credentials --resource-group b6luna --name AKSClusterLuna

### Deploy the application
[link](https://learn.microsoft.com/en-us/azure/aks/learn/quick-kubernetes-deploy-cli#code-try-7)

voting.yml

kubectl apply -f voting.yml

### Determine the networking service type

kubectl get service votingapp-azure --watch

### Create KT auth & pwd secret
kubectl create secret generic reddb-pass --from-file=./username.txt --from-file=./password.txt

kubectl create secret generic reddb-pass --from-literal=username=devuser --from-literal=password=password_redis_154

## Volumes

links :

[Persistent Volume](https://kubernetes.io/docs/concepts/storage/persistent-volumes/)
[Configure PV](https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage/)
[Multiple Nodes](https://stackoverflow.com/questions/54845025/does-kubernetes-support-persistent-volumes-shared-between-multiple-nodes-in-a-cl)
