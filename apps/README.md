# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 8ecc0c2b38ad5b59b45695f7538728f8bceb0c76
helm template . --name-template echo-server --namespace echo-server --set clustername=zeng-sbx --values ./values/values-all.yaml --include-crds
```
