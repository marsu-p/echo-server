# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout cf749fa2c08347f7177bb6b41a1825cc012a2d6e
helm template . --name-template echo-server-renderer --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
