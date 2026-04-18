# fluxcd

FluxCD bootstrap staging cluster
```
flux bootstrap github \
    --token-auth --owner=gustavoscheffer \
    --repository=fluxcd \
    --branch=main \
    --path=clusters/staging \
    --personal \
    --components-extra=source-watcher
```
```
k -n flux-system get ArtifactGenerator
```
```
k -n flux-system get Gitrepository
```
```
k -n flux-system get kustomizations.kustomize.toolkit.fluxcd.io
```