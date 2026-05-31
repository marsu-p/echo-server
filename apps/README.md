# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout b057f3f684b62a62c23b477b9b67eac367ee9694
helm template . --name-template pat-dummy --namespace pat-dummy --values ./values/values-all.yaml --values ./values/values-pat.yaml --include-crds
```
