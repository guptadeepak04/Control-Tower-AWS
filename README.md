Control-Tower-AWS/
│
├── README.md
│
├── docs/
│   ├── architecture.md
│   ├── account-strategy.md
│   ├── networking.md
│   └── security.md
│
├── organizations/
│   ├── organization-structure.yaml
│   ├── ou-structure.yaml
│   └── account-config.yaml
│
├── lza-config/
│   ├── global-config.yaml
│   ├── organization-config.yaml
│   ├── accounts-config.yaml
│   ├── network-config.yaml
│   ├── security-config.yaml
│   └── customizations-config.yaml
│
├── terraform/
│   ├── modules/
│   │
│   ├── networking/
│   │   ├── main.tf
│   │   ├── variables.tf
│   │   └── outputs.tf
│   │
│   ├── shared-services/
│   │   ├── main.tf
│   │   ├── variables.tf
│   │   └── outputs.tf
│   │
│   ├── workloads/
│   │   ├── dev/
│   │   ├── test/
│   │   ├── uat/
│   │   └── prod/
│   │
│   └── backend.tf
│
├── policies/
│   ├── scp/
│   │   ├── deny-root.json
│   │   ├── deny-public-s3.json
│   │   └── region-restriction.json
│   │
│   └── iam/
│       ├── admin-policy.json
│       └── readonly-policy.json
│
├── cloudformation/
│   ├── audit-account.yaml
│   └── logarchive-account.yaml
│
├── pipelines/
│   ├── terraform-plan.yaml
│   ├── terraform-apply.yaml
│   └── deployment.yaml
│
└── .github/
    └── workflows/
        ├── terraform-plan.yml
        ├── terraform-apply.yml
        ├── lint.yml
        └── security-scan.yml 