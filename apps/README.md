# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 47edfd3c574733cb5d2d1578c1e5a7c1c736edcb
helm template . --name-template int-dummy --namespace int-dummy --values ./values/values-all.yaml --values ./values/values-int.yaml --include-crds
```
