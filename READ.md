Connexion au cluster (créé manuellement en amont sur azure) :
`az aks get-credentials --resource-group testbrief7rn --name mycluster`

Création des secrets :
`kubectl create secret generic redis-credentials --from-literal=username=mydbusername --from-literal=password=myinsanepassword`

Déploiement :
`kubectl apply -f infra.yml`
