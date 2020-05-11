# structure-tf-modules

### Shell script that creates Terraform modules structure with files.

.
├── example
│   └── test
│       └── integration
│           └── default
└── modules
    ├── module1
    │   └── example
    │       └── test
    │           └── integration
    │               └── default
    └── module2
        └── example
            └── test
                └── integration
                    └── default
  
### How to use
- edit structure.sh and update the variables on top
- project, is the name of the project, ie test
- modules, are the list of modules you want to include, ie s3 db r53 vpc
- files, the list of files each project should have, ie provider.tf main.tf variables.tf terraform.tfvars

```
#!/usr/bin/env bash
# name of this project
project="ecommerce"
modules="module1 module2 module3"
files="provider.tf main.tf variables.tf terraform.tfvars"
run ./structure.sh

```

review the structure
