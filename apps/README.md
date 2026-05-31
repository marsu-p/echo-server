# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout cc19a593989e6ea49a07d90e451c6cda1a97b978
helm template . --name-template test2-dummy --namespace test2-dummy --values ./values/values-all.yaml --values ./values/values-test2.yaml --include-crds
```
