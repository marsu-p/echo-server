# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout 5ec31a06aa06e5ebc35b7578034891f1e4855091
helm template . --name-template pat-dummy --namespace pat-dummy --values ./values/values-all.yaml --values ./values/values-pat.yaml --include-crds
```
