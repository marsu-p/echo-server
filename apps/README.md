# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout f3022515d2c8121f3ff9f5a4420f4f6073db8b0c
helm template . --name-template major-dummy --namespace major-dummy --values ./values/values-all.yaml --values ./values/values-major.yaml --include-crds
```
