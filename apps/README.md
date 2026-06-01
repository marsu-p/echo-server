# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 09eef1b2731053f10527c30c8d50d1c95039988f
helm template . --name-template test2-dummy --namespace test2-dummy --set clustername=zeng-sbx --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
