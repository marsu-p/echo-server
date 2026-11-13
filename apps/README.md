# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 335f4ce60a710598c5a7a5f552dd05bd96ea4bff
helm template . --name-template echo-server --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
