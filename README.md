

### How to Push this help chart to a Kubernetes Cluster from a Mac


1. Choose a context (kubectx is great tool for that)

   e.g.  kubectx foo_context_name


2.  Dry-run

   helm install bunch-of-deployments-helm-chart --dry-run bunch-of-deployments-helm-chart -f ./values.yaml


3. Actually deploying:

   helm install bunch-of-deployments-helm-chart bunch-of-deployments-helm-chart -f ./values.yaml


4. Postcheck

   kubectl get deploy
   kubectl get po






