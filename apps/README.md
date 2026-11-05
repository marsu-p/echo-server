# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 85b3ebf71c7f19a67880b8d0f39e672337b95d61
helm template . --name-template echo-server --namespace echo-server --set clustername=zeng-sbx --values ./values/values-all.yaml --include-crds
```
