# EC2 Placement Groups

- `Cluster` - Pack instances close together
- `Spread` - Keep instances separated
- `Partition` - 

## Cluster Placement Group

- Can't span AZs - `ONE AZ ONLY` - locked when launching first instance
- Can span VPC peers - but impacts performance
- Requires a supported instance type
- Use the same type of instance (`not mandatory`)
- Launch at the same time (`not mandatory` ... `very recommended`)
- `10Gbps single stream performance`
- Use cases: `Performance`, `fast speeds`, `low latency`

![Cluster](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1100-ADVANCED_EC2/00_LEARNINGAIDS/PlacementGroups-1.png)

## Spread Placement Group

![Spread](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1100-ADVANCED_EC2/00_LEARNINGAIDS/PlacementGroups-2.png)

## Partition Placement Group

![Partition](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1100-ADVANCED_EC2/00_LEARNINGAIDS/PlacementGroups-3.png)

## Resources

- [Cluster Placement Groups](https://learn.cantrill.io/courses/895720/lectures/24043540)
