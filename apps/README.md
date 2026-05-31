# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout cf701a3833a91ddc23356b1de3545d1ec52964b4
helm template . --name-template major-dummy --namespace major-dummy --values ./values/values-all.yaml --values ./values/values-major.yaml --include-crds
```
