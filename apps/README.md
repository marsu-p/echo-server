# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 896aa103230e05424b68addb09432d15cf83438f
helm template . --name-template major-dummy --namespace major-dummy --values ./values/values-all.yaml --values ./values/values-major.yaml --include-crds
```
