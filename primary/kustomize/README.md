# Kustomize Simple Project (ksp)

Our simple kustomize project are included three environments:
development, test, and production. Based on their features and
requirements, we changed its functionality, like font color,
custom header message, and numner of replicas.


Files and directories structure:
```
.
├── base
│   ├── deployment.yml
│   ├── kustomization.yml
│   └── service.yml
├── overlays
│   ├── dev
│   │   ├── config.properties
│   │   ├── kustomization.yml
│   │   └── replicas.yml
│   ├── prod
│   │   ├── config.properties
│   │   ├── kustomization.yml
│   │   └── replicas.yml
│   └── test
│       ├── config.properties
│       ├── kustomization.yml
│       └── replicas.yml
└── README.md
```
