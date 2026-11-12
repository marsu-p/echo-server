# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 31b3f4976eaa10eeafdef765fb5cbc0bd2d4f223
helm template . --name-template echo-server --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
