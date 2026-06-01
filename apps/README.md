# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 219ce646e6b09f3a046f98e3e22ef784fbec5d54
helm template . --name-template test2-dummy --namespace test2-dummy --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
