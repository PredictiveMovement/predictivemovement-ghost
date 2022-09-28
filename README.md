# Predictive Movement ghost

```bash
# Setup namespace.
kubectl create namespace predictivemovement-ghost
kubens predictivemovement-ghost # Select namespace.

# Create Ghost secret.
kubectl create secret generic ghost --from-literal=password=rawr

# Create MariaDB secret.
kubectl create secret generic mariadb --from-literal=root-password=meow --from-literal=password=purr

# Deploy Ghost + MariaDB.
skaffold run
```
