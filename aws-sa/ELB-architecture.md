# Elastic Load Balancer Architecture (ELB)

## ELB Architecture

![ELB Architecture - Part 1](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/ELBArchitecture1.png)

![ELB Architecture - Part 2](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/ELBArchitecture2.png)

## Cross-Zone LB

![ELB Architecture - Part 3](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/ELBArchitecture3.png)

## ELB Architecture Points

- ELB is a `DNS A` Record pointing a `1+` Nodes per AZ.
- Nodes (in one subnet per AZ) can scale.
- `Internet-facing` means nodes have `public IPV4 IPs`.
- `Internal` is `private only IPs`.
- EC2 `doesn't need to public` to work with a LB.
- `Listerner` Configuration controls `WHAT` the LB does.
- `8+` Fee IPs per subnet, and `/27` subnet to allow scaling.

## Resources

- [ELB Architecture - Part 1](https://learn.cantrill.io/courses/895720/lectures/22009428)
- [ELB Architecture - Part 2](https://learn.cantrill.io/courses/895720/lectures/22009458)

