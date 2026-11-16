# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 01af00727d071f6ce395a676301fc89176c54984
helm template . --name-template echo-server --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
