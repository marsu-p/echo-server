# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout f139884369f8d8a8506238c7d1460c6628ff0c58
helm template . --name-template demo-dummy --namespace demo-dummy --values ./values/values-all.yaml --values ./values/values-demo.yaml --include-crds
```
