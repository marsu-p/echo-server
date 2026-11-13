# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 3455f22d289b89e85d91dfa2ae872b3b28dd9105
helm template . --name-template echo-server --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
