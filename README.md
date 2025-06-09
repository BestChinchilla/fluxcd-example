# fluxcd

## Install

```bash
flux bootstrap github \
    --owner BestChinchilla \
    --repository fluxcd-example \
    --branch main \
    --path ./clusters/k3s \
    --components-extra='image-reflector-controller,image-automation-controller' \
    --read-write-key
```
