# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout d0006b77b02b00317cf861945847cd1cdc2d5d3c
helm template . --name-template echo-server --namespace echo-server --set clustername=zeng-sbx --values ./values/values-all.yaml --include-crds
```
