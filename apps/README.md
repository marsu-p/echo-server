# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 782b2657a9077bd5fc2d8928b54d7cd078ea5564
helm template . --name-template test2-echo-server --namespace test2-echo-server --set clustername=zeng-sbx --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
