# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout dad29c8f8fa5179c03b918bff376e146f5ccbe55
helm template . --name-template major-dummy --namespace major-dummy --values ./values/values-all.yaml --values ./values/values-major.yaml --include-crds
```
