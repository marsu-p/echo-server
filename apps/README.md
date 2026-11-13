# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server.git
# cd into the cloned directory
git checkout 2d337155eb2376d83afae4c79e4f233436fb2fd5
helm template . --name-template echo-server-renderer --namespace echo-server --set clustername=ztst-sbx --values ./values/values-all.yaml --include-crds
```
