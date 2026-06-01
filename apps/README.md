# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/marsu-p/echo-server
# cd into the cloned directory
git checkout ea409ca21a8c7ad2fc97cf86f99378cf82499722
helm template . --name-template test-dummy --namespace test-dummy --set clustername=ztst-sbx --values ./values/values-all.yaml --values ./values/values-test.yaml --include-crds
```
