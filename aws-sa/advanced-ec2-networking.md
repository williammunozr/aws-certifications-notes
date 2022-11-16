# Advanced EC2 Networking

## EC2 Networking

![EC2 Networking 1](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/0900-ELASTIC_COMPUTE_CLOUD(EC2)/00_LEARNINGAIDS/EC2networking-1.png)

![EC2 Networkin 2](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/0900-ELASTIC_COMPUTE_CLOUD(EC2)/00_LEARNINGAIDS/EC2networking-2.png)

- `Primary ENI` - EC2 Instances have a primary `ENI` created with the instance which `cannot be removed`.
- `Secondary ENI` - Additional `ENIs` can be added in and removed from other subnets (multi homed) but NOT in other AZs.
- Multi-ENI offers multiple security zones or traffic types.
- SGs attached to ENIs offer different protection rules.
- Each ENI can also be protected by a NACL around its subnet.
