# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout f3022515d2c8121f3ff9f5a4420f4f6073db8b0c
helm template . --name-template test2-dummy --namespace test2-dummy --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
