# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout a8463d3926d16cc259f54a5b42360e72072abf64
helm template . --name-template test2-echo-server --namespace test2-echo-server --set clustername=zeng-sbx --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
