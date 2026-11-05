# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout e7c1bd343176e0f2616fcb1f8fcf981c68274a92
helm template . --name-template echo-server --namespace echo-server --set clustername=zeng-sbx --values ./values/values-all.yaml --include-crds
```
