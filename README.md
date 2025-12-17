# kubemind

## Installation

```sh
helm install kubemind oci://ghcr.io/mikolajsemeniuk/charts/kubemind \
  --version 0.1.0 \
  -n kubemind-system --create-namespace
```

## Installation Locally

```sh
helm install kubemind charts/kubemind -n kubemind-system --create-namespace
```
