# Gateway Load Balancers (GWLB)

## Why do we need a GWLB?

- Help you `run` and `scale` `3rd party appliances`
- ..things like `firewalls`, `intrusion detection` and `prevention` systems
- `Inbound` and `Outbound` traffic (`transparent` inspection and protection)
- .. `GWLB endpoints` ... traffic enters/leaves via these endpoints
- .. the GWLB `balances` across `multiple backend appliances`
- Traffic and metadata is tunnelled using `GENEVE` protocol

![Why GWLB](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1500-HA_and_SCALING/00_LEARNINGAIDS/GWLB-1.png)

## GWLB 101 - How it works

![How it works](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1500-HA_and_SCALING/00_LEARNINGAIDS/GWLB-2.png)

## GWLB Architecture

![GWLB Architecture](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1500-HA_and_SCALING/00_LEARNINGAIDS/GWLB-3.png)

## Resources

- [Gateway Load Balancers](https://learn.cantrill.io/courses/895720/lectures/35110028)
