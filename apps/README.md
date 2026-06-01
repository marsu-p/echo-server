# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 6c6b8ec821382a54c9f2d32254217fa0d7458493
helm template . --name-template int-dummy --namespace int-dummy --values ./values/values-all.yaml --values ./values/values-int.yaml --include-crds
```
