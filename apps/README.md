# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 839a3b00acb518303ffa9c9923f3263d24f3c9b0
helm template . --name-template test2-dummy --namespace test2-dummy --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
