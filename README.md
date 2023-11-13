# Prod, Staging, QA, Dev

L'application utilise les namespaces Kubernetes pour déployer différents environnements.

Les namespaces sont créés lors de l'exécution de la commande "helm upgrade ... --namespace ... --create-namespace" dans le Jenkinsfile.

Chaque namespace fait alors appel à son propre fichier de valeurs, dev-values.yaml, qa-values.yaml...