# fluxcd

> [!IMPORTANT]
> Use this repository as a template for your own FluxCD cluster setup!!!

## Install

Subsitute the variables with your own

```bash
flux bootstrap github \
    --owner $OWNER \
    --repository $REPOSITORY \
    --branch $BRANCH \
    --path ./clusters/$CLUSTER \
    --components-extra='image-reflector-controller,image-automation-controller' \
    --read-write-key
```

Example:

```bash
flux bootstrap github \
    --owner BestChinchilla \
    --repository fluxcd-example \
    --branch main \
    --path ./clusters/k3s \
    --components-extra='image-reflector-controller,image-automation-controller' \
    --read-write-key
```
