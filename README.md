## Install flux cd in cluster

 curl -s https://fluxcd.io/install.sh | sudo bash

flux --version

flux install

we can also install flux with flux helm chart
```
helm repo add fluxcd-community https://fluxcd-community.github.io/helm-charts
helm repo update

helm install flux2 fluxcd-community/flux2 \
  --namespace flux-system \
  --create-namespace \
  --set someOption1=… \
  --set someOption2=…
```
