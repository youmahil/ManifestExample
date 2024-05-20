# ManifestExample
## Structure
```
├── base
│   ├── dep-echo-demo.yaml
│   ├── svc-echo-demo.yaml
│   ├── ing-echo-demo.yaml
│   ├── kustomization.yaml
└── overlays
    └── dev
        └── kustomization.yaml
```
## build
```sh
kustomize build overlay/dev/
```

## apply kubernetes
```sh
kustomize build overlay/dev/ | kubectl apply -f -
```