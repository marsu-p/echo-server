# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 88f35b788dc20f23ddfa3d95b088daa6e9621442
helm template . --name-template test-dummy --namespace test-dummy --values ./values/values-all.yaml --values ./values/values-test.yaml --include-crds
```
