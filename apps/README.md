# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 51452e6a03f477244f618887ddda7b0faed1ffc4
helm template . --name-template test2-dummy --namespace test2-dummy --set clustername=zeng-sbx --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
