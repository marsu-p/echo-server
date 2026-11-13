# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout db9d5b29c489f50bae6043e2bc714de8b7f025bd
helm template . --name-template echo-server-renderer --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
