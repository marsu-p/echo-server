# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout c267620d5190c9fe6d03df662961764fa38b3f0e
helm template . --name-template zeng-echo-server --namespace promoter-system --values ./values/values-all.yaml --values ./values/values-zeng-sbx.yaml --include-crds
```
