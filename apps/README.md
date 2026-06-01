# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 09eef1b2731053f10527c30c8d50d1c95039988f
helm template . --name-template test-dummy --namespace test-dummy --set clustername=ztst-sbx --values ./values/values-all.yaml --values ./values/values-test.yaml --include-crds
```
