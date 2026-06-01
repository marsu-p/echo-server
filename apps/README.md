# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 499dd4541fd7343d43bf97af4289658f828a3596
helm template . --name-template test-dummy --namespace test-dummy --values ./values/values-all.yaml --values ./values/values-test.yaml --include-crds
```
