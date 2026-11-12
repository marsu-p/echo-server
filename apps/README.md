# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 98628cff1e2fefa2da79efc21ab560490a839763
helm template . --name-template echo-server --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
